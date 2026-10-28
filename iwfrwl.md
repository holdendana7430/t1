代发 wailian999

TS:   process.cwd()
来源：http://hz.birdmap.top/gtquknincx.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.birdmap.top/gtqqjoojgk.html

Go:   os.Getwd()
来源：http://hz.hnqzz.top/gtxlecwfbm.html

Ruby: Dir.pwd
来源：http://hz.dashuyun.cn/gtpclqhaiq.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zhengqikj.top/gtmmqdsars.html

[M05] 设置退出码
来源：http://hz.ybcxt.top/gtrsiwjqut.html

Py:   sys.exit(1)
来源：http://hz.shangyingyoupin.top/gtnmqfhmip.html

PHP:  exit(1);
来源：http://hz.hfpthk.cn/gtvgershzj.html

JS:   process.exit(1)
来源：http://hz.chenjidiqi.icu/gtqpysoppz.html

TS:   process.exit(1)
来源：http://hz.jinghuilouyu.cn/gtjzaykyah.html

Java: System.exit(1)
来源：http://hz.yj202588.top/gteinxotvo.html

Go:   os.Exit(1)
来源：http://hz.guannengcc.top/gtdxdoyfuq.html

Ruby: exit 1
来源：http://hz.iojbl.cn/gtxgyflhtg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.meibo888.top/gtjspblojj.html

[M06] 向标准错误输出
来源：http://hz.snrcjt.cn/gtvordepvj.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yuanzhike.top/gthedcklct.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.gotoacloud.top/gthvfnjwwe.html

JS:   console.error("err")
来源：http://hz.smart0.xyz/gtqxyviqsh.html

TS:   console.error("err")
来源：http://hz.jianghu66.top/gtctqevqdn.html

Java: System.err.println("err")
来源：http://hz.xuetiantiany.cn/gtydoazrzd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zycfv.cn/gtntvpenrc.html

Ruby: warn "err"
来源：http://hz.yuxming.cn/gtwrkyyabr.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.pengpengdd.cyou/gtolligvfm.html

[M07] 判断是否为主入口
来源：http://hz.tianlin.xyz/gtkweeiiyc.html

Py:   if __name__ == "__main__":
来源：http://hz.yonumen.top/gtwivspjih.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.xingfuxueyuan.xyz/gthepbctai.html

JS:   require.main === module
来源：http://hz.jlsjyb.cn/gtpfiyhgdv.html

TS:   require.main === module
来源：http://hz.zhixingplan.top/gtorldnoco.html

Java: public static void main(String[] args)
来源：http://hz.dashuyun.cn/gtlwnmbivn.html

Go:   func main()
来源：http://hz.yj202588.top/gtlmitizia.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.birdmap.top/gttnubwwbj.html

C#:   static void Main(string[] args)
来源：http://hz.hammf.cn/gtmeqmvapc.html

[M08] 获取系统与运行时信息
来源：http://hz.ivvv.top/gteccagrue.html

Py:   platform.system();  platform.python_version()
来源：http://hz.fzhhl.top/gthztylyiz.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.nanxinkj.top/gtdikptnqq.html

JS:   process.platform;  process.version
来源：http://hz.yangfankeji.com/gtkeclmtdk.html

TS:   process.platform;  process.version
来源：http://hz.cqqwz.cn/gtfjvpjpeq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.ivvv.top/gtddeuuzbf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yvedp.cn/gtzjbedhyc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.fzhhl.top/gtfkuquhvq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.zhaomingkeji.xyz/gtanfsmgcl.html

================================================================================
来源：http://hz.gaohongyu789.top/gtaudhbfnb.html

N. 数据结构与算法
来源：http://hz.zhijiandao.cn/gtccbgcrnt.html

================================================================================
来源：http://hz.smart0.xyz/gtfjlauqpi.html

[N01] 二分查找（有序数组）
来源：http://hz.shzxlz.cn/gtcfhnzngb.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.fengsongda.top/gtjtzbtqrx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yj20258888.top/gtlnsfmqwm.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jinqigufen.top/gtpjlczldr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.nwbrower.top/gtdvqqbtlp.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.tanke756.top/gtxypjlqhu.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jinghuilouyu.cn/gtfafsmmvw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.birdmap.top/gtswauobxo.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.nanxinkj.top/gtybqstwnp.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.gzhubu.top/gtwytvnsqc.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.chenjidiqi.icu/gtpqvowjfe.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yongpay.top/gtqbgpvene.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.snrcjt.cn/gtqrjwvclv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zycfv.cn/gtoozeoidr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.tianlin.xyz/gtxgzodhro.html

Go:   slices.Sort(arr)
来源：http://hz.cheryme.top/gtlnzsxqud.html

Ruby: arr.sort
来源：http://hz.yueranfly.top/gtjbdssmce.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.316326.xyz/gtzewbcpwf.html

[N03] 快速排序（分治示例）
来源：http://hz.jinyuanbaomall.cn/gtkypacnuw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jinyuanbaomall.cn/gtzytujbsu.html

PHP:  // 递归实现，或用 usort
来源：http://hz.hammf.cn/gtvilqthjm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hnxiangtu.top/gtlreceoso.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.316326.xyz/gtfmewoeni.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.smart0.xyz/gtvbdgcxhx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.ppjwa.cn/gtsrqgrotk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.xinyue.icu/gtiqycoiay.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.tianlin.xyz/gthohcjlqm.html

[N04] 斐波那契数列
来源：http://hz.yanxiufei.cn/gtulpsvoye.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.gaohongyu789.top/gtmadewtrb.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.tian-w.cn/gttlovozfp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.redwolf501.top/gtwffbaaww.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xinyue.icu/gtctewocbw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.nanxuanxn.top/gtmiqkxcof.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.birdmap.top/gtmmtfbqgg.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.hnxiangtu.top/gtpcisckuk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.snrcjt.cn/gtzqsncvuy.html

[N05] 最大公约数
来源：http://hz.dianchejie.cn/gtedduhhlt.html

Py:   math.gcd(a, b)
来源：http://hz.birdmap.top/gtjknkasfi.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.cucudq.cn/gtdsjfzzec.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zycfv.cn/gtdczqvhyp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jiagoushi.top/gtjriwmqdy.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.shanyushiyangkeji.top/gtzfhkilpk.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.hywenlv.cn/gtdtdsfwhx.html

Ruby: a.gcd(b)
来源：http://hz.gotoacloud.top/gthshnebfg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.guowangkeji.top/gtwhrcdsuu.html

[N06] 判断回文字符串
来源：http://hz.chenlongwang.top/gtjkxcgchl.html

Py:   s == s[::-1]
来源：http://hz.jqgfzy.top/gtmxfsqnty.html

PHP:  $s === strrev($s);
来源：http://hz.yj20258.top/gtxxclsbuk.html

JS:   s === [...s].reverse().join("")
来源：http://hz.gaohongyu789.top/gtvvfyztiw.html

TS:   s === [...s].reverse().join("")
来源：http://hz.wangdashe.top/gtiidihitw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.xylfe.cn/gtrzcegeix.html

Go:   // 双指针从两端比较
来源：http://hz.jyoumei.cn/gtomugaiep.html

Ruby: s == s.reverse
来源：http://hz.52xcode.cn/gthsffdfva.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.xuetiantiany.cn/gtfdjyondg.html

[N07] 两数之和（返回下标）
来源：http://hz.jinqigfzy.top/gtlpfjkrlb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.snrcjt.cn/gtacygxuwx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.gaohongyu789.top/gtznzsmynk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.yj20258.top/gtzqyvnnxy.html

TS:   // 手写 Map<string, number>
来源：http://hz.hywenlv.cn/gtrmuzofox.html

Java: // 手写 HashMap
来源：http://hz.fengsongda.top/gtwtafiaii.html

Go:   // 手写 map[int]int
来源：http://hz.c1oappe.top/gtilcmerss.html

Ruby: // 手写 Hash
来源：http://hz.aibaodan.cn/gtzlknkote.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.c1oappe.top/gtfkgygzkq.html

[N08] 生成全排列
来源：http://hz.haohaochexian.top/gtyrwtkvuu.html

Py:   itertools.permutations(arr)
来源：http://hz.tanke756.top/gtpovuiryx.html

PHP:  // 手写递归交换
来源：http://hz.pengpengdd.cyou/gtdevnffwe.html

JS:   // 手写回溯递归
来源：http://hz.redwolf501.top/gtuxinkncc.html

TS:   // 手写回溯递归
来源：http://hz.meibo888.top/gtjvoqfdju.html

Java: // 手写回溯递归
来源：http://hz.52xcode.cn/gtaccsinby.html

Go:   // 手写回溯递归
来源：http://hz.yongpay.top/gtinqwioju.html

Ruby: arr.permutation.to_a
来源：http://hz.yanxiufei.cn/gtwwqlrchd.html

C#:   // 手写回溯递归
来源：http://hz.zycfv.cn/gtuibviiuz.html

[N09] 栈与队列
来源：http://hz.xuetiantiany.cn/gtbskxcbga.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.hfpthk.cn/gtyvhgbcdl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.sysykeji.top/gtfpoqczyh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.tianlin.xyz/gtouwkyoqe.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yuxming.cn/gtotbfdlio.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.gogol.net.cn/gtuokojatt.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.pengpengdd.cyou/gtbxviuakz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.hongshengwenyu.top/gtonukzocg.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yonumen.top/gtolclcpqs.html

[N10] 链表节点定义
来源：http://hz.xylfe.cn/gtkzlruthz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.ydzc1.top/gtqzlnjkmb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.sysykeji.top/gtimhlzvml.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yonumen.top/gtkncftcit.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.redwolf501.top/gtwinpmcqr.html

Java: class Node { int v; Node next; }
来源：http://hz.redwolf501.top/gtbjpguvyx.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.cdnleiting.top/gtqjywpqbv.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.nanxuanxn.top/gtbuarutxr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.zhijiandao.cn/gtjsfyicfi.html

[N11] 二叉树中序遍历
来源：http://hz.tian-w.cn/gtglhhdidy.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.xuetiantiany.cn/gtoyvrfiuy.html

PHP:  // 手写递归函数
来源：http://hz.cucudq.cn/gtesgbyduk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hywenlv.cn/gttuywqftb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.guannengcc.top/gtutrerlua.html

Java: // 手写递归
来源：http://hz.dianchejie.cn/gtbroqzucm.html

Go:   // 手写递归
来源：http://hz.wangshuangyany.cn/gtkotwzyxm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.ehwqpu.com/gtfbytlgfy.html

C#:   // 手写递归
来源：http://hz.ivvv.top/gtctfazlsy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.hywenlv.cn/gtjeqtjmnj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.wangshuangyany.cn/gtpumobltt.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.havefunace.top/gtdmulyljt.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.sweek.top/gtxrrkbzew.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yongpay.top/gtyeeltxzo.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.redwolf501.top/gtscqmjujl.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.zycfv.cn/gtvztnppkq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.iojbl.cn/gtplxdsbhl.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.cucudq.cn/gtguwrqjmk.html

================================================================================
来源：http://hz.havefunace.top/gtcxpfuzya.html

O. 并发与异步
来源：http://hz.nwbrower.top/gtuqbpmfto.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtlsjkbggm.html

[O01] 启动一个线程
来源：http://hz.cheryme.top/gtfessdfcb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.jinghuilouyu.cn/gtsuvwzabl.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yuanzhike.top/gtlyujntov.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.snrcjt.cn/gtrwuxgadl.html

TS:   // 同 JS
来源：http://hz.dianchejie.cn/gtstlqptdu.html

Java: new Thread(() -> f()).start()
来源：http://hz.hfpthk.cn/gtawwdvakq.html

Go:   go f()
来源：http://hz.pengpengdd.cyou/gtiwurkmzw.html

Ruby: Thread.new { f }
来源：http://hz.xuanzx.com/gtnlnsaoms.html

C#:   Task.Run(() => F());
来源：http://hz.tianlin.xyz/gtruejgdsb.html

[O02] 使用线程池
来源：http://hz.cucudq.cn/gtcgdmxoep.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.chenjidiqi.icu/gtytpgunew.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.nanxinkj.top/gtljiyjeof.html

JS:   // worker_threads 线程池
来源：http://hz.hywenlv.cn/gtkjgmeaze.html

TS:   // worker_threads 线程池
来源：http://hz.jqgufenzy.top/gtoqriuwme.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.chenzaomai.com/gthxtizrar.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.ppjwa.cn/gtxjrhwjmh.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.cdnleiting.top/gtjevagywq.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.havefunace.top/gtxhknuokb.html

[O03] 加锁保护共享数据
来源：http://hz.nanxuanxn.top/gtrbwfwmco.html

Py:   with lock: shared += 1
来源：http://hz.jinghuilouyu.cn/gtluauwzgs.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.shangyingyoupin.top/gtpourwguc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.chenzaomai.com/gtxmkgkety.html

TS:   // 同 JS
来源：http://hz.snrcjt.cn/gtwqnhmrld.html

Java: synchronized (this) { shared++; }
来源：http://hz.shanyushiyangtech.top/gtrlhhgkwq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.ppjwa.cn/gtvwtjsels.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.cheryme.top/gtxlagumof.html

C#:   lock (gate) { shared++; }
来源：http://hz.tian-w.cn/gtmrxnvraj.html

[O04] 定义异步函数并等待
来源：http://hz.zhiwuduotai.top/gtezeunaiz.html

Py:   async def f():⏎    await g()
来源：http://hz.jinqigfzy.top/gteaxhcxxx.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.feifeiyinyue.top/gtqbnhpmcf.html

JS:   async function f() { await g(); }
来源：http://hz.zhoulong.xyz/gtjhuroxrp.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.zhixingplan.top/gtqwtartlk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.jlsjyb.cn/gtjaalovmq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.nwbrower.top/gtumcpaqgr.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yongpay.top/gttprembvt.html

C#:   async Task F() { await G(); }
来源：http://hz.jianghu66.top/gtotykqlkd.html

[O05] 并发执行并等待全部完成
来源：http://hz.316326.xyz/gtuetpbiua.html

Py:   asyncio.gather(*tasks)
来源：http://hz.gotoacloud.top/gtvldcukxj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.9152youxi.cn/gtpleloylh.html

JS:   await Promise.all(tasks)
来源：http://hz.mhx1999.top/gtrpzicapr.html

TS:   await Promise.all(tasks)
来源：http://hz.zhixingplan.top/gtqtwbgxxe.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.hnxiangtu.top/gtwvvfbddg.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.sweek.top/gtqaptqqed.html

Ruby: threads.map(&:join)
来源：http://hz.pengpengdd.cyou/gtotaawbqa.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.jinqigfzy.top/gtfahdlwmt.html

[O06] 使用进程池
来源：http://hz.xuetiantiany.cn/gtgwivglfj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.9152youxi.cn/gtorsehfmt.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.hnxiangtu.top/gtscsjernb.html

JS:   // child_process / cluster 模块
来源：http://hz.ehwqpu.com/gtltlnzhoc.html

TS:   // child_process / cluster 模块
来源：http://hz.xylfe.cn/gtwmjiyxhl.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jinqigufen.top/gtzzcfmkya.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.shanyushiyangtech.top/gtsgehakvp.html

Ruby: // fork 块
来源：http://hz.sysykeji.top/gtioxlyert.html

C#:   Parallel.For
来源：http://hz.yj20258888.top/gtxvrulpac.html

================================================================================
来源：http://hz.kuanghao11.cn/gtuqybkukg.html

P. 常用工具函数
来源：http://hz.smart0.xyz/gtlwrnsxcd.html

================================================================================
来源：http://hz.jinqigfzy.top/gtevworqne.html

[P01] 生成 UUID
来源：http://hz.zhijiandao.cn/gttqrosixq.html

Py:   str(uuid.uuid4())
来源：http://hz.nwbrower.top/gtxtccpknz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.c1oappe.top/gtqdaearcg.html

JS:   crypto.randomUUID()
来源：http://hz.9152youxi.cn/gtpschlnru.html

TS:   crypto.randomUUID()
来源：http://hz.guannengcc.top/gtbmpwyyoc.html

Java: UUID.randomUUID().toString()
来源：http://hz.nanxinkj.top/gtmvbutjih.html

Go:   // 用 github.com/google/uuid
来源：http://hz.wangshuangyany.cn/gtdzhtlqzi.html

Ruby: SecureRandom.uuid
来源：http://hz.fzhhl.top/gtmrwkwmzs.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.xinyue.icu/gtichrwvpk.html

[P02] MD5 / SHA256 摘要
来源：http://hz.yueranfly.top/gtzbtztclm.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.guowangkeji.top/gtdzzuayrq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.tanke756.top/gtecholsqi.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.aizwys.cn/gtvseqkyoz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.gaohongyu789.top/gtxqcbooyi.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.zhijiandao.cn/gtoejanmli.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.ywan-chungtsiang.top/gtajugrhxz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.xziqi.cn/gtqagxmzft.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.fengsongda.top/gtohpchkmw.html

[P03] 生成短随机字符串
来源：http://hz.shangyingyoupin.top/gtjitgwalq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.yueranfly.top/gtpnxzhdub.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.wangshuangyany.cn/gtmiqawtpx.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jinghuilouyu.cn/gtrlkyljwn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.gotoacloud.top/gtzhvxraql.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.haohaochexian.top/gtwcmkxyiw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.snrcjt.cn/gtlxzvwpox.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.hnqzz.top/gtlojgxbhw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.hongshengwenyu.top/gtqbulshcv.html

[P04] 求长度
来源：http://hz.quarkkingdee.top/gteyfuohxt.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.daxiang520.top/gtjnxutxxk.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.cqqwz.cn/gtfshgvymq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.sxryk.cn/gtubxmpzmv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.cashguo.top/gtokpivioj.html

Java: list.size();  map.size();  s.length()
来源：http://hz.yj202588.top/gtsxtriodf.html

Go:   len(arr);  len(m)
来源：http://hz.cdnleiting.top/gthtzdzyqu.html

Ruby: x.length;  x.size
来源：http://hz.ydzc1.top/gtmmgzgpgb.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.sxryk.cn/gteseumvve.html

[P05] 判断两个对象内容是否相等
来源：http://hz.aizwys.cn/gtfdvsvwsi.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.ivvv.top/gtfzaegkqs.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.sufxvd.cn/gtjdlbtdcs.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.haohaochexian.top/gtvbvndoep.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.316326.xyz/gtyzxcomog.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.zhongyouzk.top/gtqybrfzpx.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.wangshuangyany.cn/gtgkafcqmd.html

Ruby: a == b
来源：http://hz.zhengqikj.top/gtdplmbtdq.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.xziqi.cn/gtkklbnhuc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.meibo888.top/gtqytcpkmn.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.bjfxy.top/gtiwokohdt.html

PHP:  if (empty($x)) {}
来源：http://hz.hongshengwenyu.top/gtglomxnsf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.yj202588.top/gtherxweib.html

TS:   if (x == null) {}
来源：http://hz.tanke756.top/gtptyolbdg.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.hnqzz.top/gtwmcbfnmr.html

Go:   if x == nil {}
来源：http://hz.gotoacloud.top/gtdstloavl.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.hammf.cn/gttdkcyktw.html

C#:   if (x is null) {}
来源：http://hz.iojbl.cn/gtpmkvwxzr.html

[P07] 防抖与节流
来源：http://hz.9152youxi.cn/gtcujftiep.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.xziqi.cn/gtmyqwfeto.html

PHP:  // 手写时间戳比较
来源：http://hz.ydjk.org.cn/gttavqjjim.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.bjfxy.top/gtrxjjjwuf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.guowangkeji.top/gtbcktenpy.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.daria6918.cn/gtdafrjcji.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.aizwys.cn/gtyrtjcabs.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.feifeiyinyue.top/gtbtguoeuh.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.yanxiufei.cn/gtkpxmutvi.html

[P08] 处理浮点精度问题
来源：http://hz.svipenyu.cn/gtvbmazvov.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jinqigfzy.top/gthwobvggv.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.nwbrower.top/gtqqjslxnu.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.fzhhl.top/gtbdnaqsaz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.yangfankeji.com/gtsuhqdjwb.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.jqgufenzy.top/gtrskaxral.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.c1oappe.top/gtrwjwcxst.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.snrcjt.cn/gtsynikgmg.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.0kj1m.cn/gtewqiafmd.html

================================================================================
来源：http://hz.jqgufenzy.top/gtvsowbmcl.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.ydjk.org.cn/gtbjwndite.html

================================================================================
来源：http://hz.gogol.net.cn/gtinshqthf.html

[Q01] 创建表
来源：http://hz.jlsjyb.cn/gtdyvirzay.html

CREATE TABLE users (
来源：http://hz.hammf.cn/gtxsfvpibd.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.sxryk.cn/gtqasoutbr.html

name VARCHAR(50) NOT NULL,
来源：http://hz.xuetiantiany.cn/gtittalimo.html

email VARCHAR(100) UNIQUE,
来源：http://hz.yanxiufei.cn/gtvdndroye.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.jinqigufen.top/gtirhtglnu.html

);
来源：http://hz.yj20258888.top/gtrpnmtsix.html

[Q02] 创建带外键的表
来源：http://hz.birdmap.top/gtjhhwhrxr.html

CREATE TABLE orders (
来源：http://hz.daxiang520.top/gtaqxwfbsn.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.9152youxi.cn/gtcskmisfx.html

user_id INT NOT NULL,
来源：http://hz.hysaishi.cn/gtroymfwqf.html

amount DECIMAL(10, 2),
来源：http://hz.quarkkingdee.top/gtwloruljf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.iojbl.cn/gtadjvzxvl.html


<!-- 参考信息 -->