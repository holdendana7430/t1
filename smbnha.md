代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://hz.cheryme.top/gtersrvljm.html

[M05] 设置退出码
来源：http://hz.gotoacloud.top/gtwawjkbwx.html

Py:   sys.exit(1)
来源：http://hz.gogol.net.cn/gtdskroval.html

PHP:  exit(1);
来源：http://hz.aibaodan.cn/gtxjlahpqq.html

JS:   process.exit(1)
来源：http://hz.pengpengdd.cyou/gtfharzeir.html

TS:   process.exit(1)
来源：http://hz.zycfv.cn/gtziuxmlpc.html

Java: System.exit(1)
来源：http://hz.cucudq.cn/gtjggybehy.html

Go:   os.Exit(1)
来源：http://hz.andypj.xyz/gtirssjvta.html

Ruby: exit 1
来源：http://hz.shzxlz.cn/gtlnehsxzr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yuanzhike.top/gtdvmelgnl.html

[M06] 向标准错误输出
来源：http://hz.zhoulong.xyz/gtbozaobbu.html

Py:   print("err", file=sys.stderr)
来源：http://hz.iojbl.cn/gtxmnjeucn.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.shuidangran.top/gtzrczauad.html

JS:   console.error("err")
来源：http://hz.birdmap.top/gtjyvfptvr.html

TS:   console.error("err")
来源：http://hz.cdnleiting.top/gtilulmkhe.html

Java: System.err.println("err")
来源：http://hz.xuetiantiany.cn/gtqfhadrvx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.pengpengdd.cyou/gtltpbrtnm.html

Ruby: warn "err"
来源：http://hz.yvedp.cn/gturabzbxt.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.mhx1999.top/gtqwfuelaw.html

[M07] 判断是否为主入口
来源：http://hz.pengpengdd.cyou/gtfpwvqekn.html

Py:   if __name__ == "__main__":
来源：http://hz.smart0.xyz/gtvtzgllgj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.tanke756.top/gtuoymdydu.html

JS:   require.main === module
来源：http://hz.ppjwa.cn/gticixvybg.html

TS:   require.main === module
来源：http://hz.nanxinkj.top/gttvqvmgte.html

Java: public static void main(String[] args)
来源：http://hz.cheryme.top/gteawgtaqa.html

Go:   func main()
来源：http://hz.yuxming.cn/gtfobmldra.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.hysaishi.cn/gtzyefsbdw.html

C#:   static void Main(string[] args)
来源：http://hz.jinyuanbaomall.cn/gtflzgddfh.html

[M08] 获取系统与运行时信息
来源：http://hz.hammf.cn/gttvgweafe.html

Py:   platform.system();  platform.python_version()
来源：http://hz.daria6918.cn/gtoagwhjco.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.jinqigfzy.top/gtoclweenz.html

JS:   process.platform;  process.version
来源：http://hz.jyoumei.cn/gtsksilwaq.html

TS:   process.platform;  process.version
来源：http://hz.xylfe.cn/gtgqozchpk.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.redwolf501.top/gtqdufjkld.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yj20258888.top/gtkyuxrozs.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.chenjidiqi.icu/gtondyqcgr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.havefunace.top/gtthyjawss.html

================================================================================
来源：http://hz.316326.xyz/gtlqjrqxpa.html

N. 数据结构与算法
来源：http://hz.vqdsnc.cn/gtnmrcuofx.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtbaalhpen.html

[N01] 二分查找（有序数组）
来源：http://hz.chenjidiqi.icu/gttwizukyh.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yvedp.cn/gttoecwzlc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.fzhhl.top/gtzcadkzzr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.snrcjt.cn/gtuysugxqr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.snrcjt.cn/gtkvgoifbl.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.zycfv.cn/gtpmnpixug.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.nanxinkj.top/gtngiewxmx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.hongshengwenyu.top/gtmjnyzaph.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.quarkkingdee.top/gtbecvtuxw.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.nanxuanxn.top/gtxwiiyhtr.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.dianchejie.cn/gtiughtxhc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.tian-w.cn/gtxakvhady.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhengqikj.top/gtjbvlxceh.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.cashguo.top/gtlvpnhsuu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.nanxinkj.top/gtgnucsxav.html

Go:   slices.Sort(arr)
来源：http://hz.dashuyun.cn/gtzbojbkpq.html

Ruby: arr.sort
来源：http://hz.yj202588.top/gtctxshpek.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.nwbrower.top/gtazegswee.html

[N03] 快速排序（分治示例）
来源：http://hz.zhengqikj.top/gthkctqqkq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yvedp.cn/gtjrdcgavv.html

PHP:  // 递归实现，或用 usort
来源：http://hz.jinqigufen.top/gtjavgtykq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.shuidangran.top/gtheomfnbi.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hammf.cn/gtxmwqehzz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.hysaishi.cn/gtbtzfyfyb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.cheryme.top/gtpuykxyye.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.tianlin.xyz/gtzewudqul.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.chenlongwang.top/gtmspunypp.html

[N04] 斐波那契数列
来源：http://hz.aibaodan.cn/gthtrruqrg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.iojbl.cn/gtnxgbmmma.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.yanxiufei.cn/gtgsxtyzbc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hywenlv.cn/gtpjwtecpv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.smart0.xyz/gtznehyqbi.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.shanyushiyangkeji.top/gtdedonpiw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.chenlongwang.top/gtlcifyibn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.hnxiangtu.top/gtgbqgolaq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.nanxinkj.top/gtsismfldp.html

[N05] 最大公约数
来源：http://hz.jinghuilouyu.cn/gtbzybjjrb.html

Py:   math.gcd(a, b)
来源：http://hz.jyoumei.cn/gtrxkrjvfg.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.hfpthk.cn/gtjcsiaxwl.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.chenlongwang.top/gthorgzlnx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.aizwys.cn/gtdzyaknay.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.jinyuanbaomall.cn/gtujexambo.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.quarkkingdee.top/gtwuydikdj.html

Ruby: a.gcd(b)
来源：http://hz.xingfuxueyuan.xyz/gtfqewcmhc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.redwolf501.top/gttpldfnea.html

[N06] 判断回文字符串
来源：http://hz.yj202588.top/gtgwectwkm.html

Py:   s == s[::-1]
来源：http://hz.aibaodan.cn/gtbaajamot.html

PHP:  $s === strrev($s);
来源：http://hz.hnxiangtu.top/gtvfetmhev.html

JS:   s === [...s].reverse().join("")
来源：http://hz.sxryk.cn/gtrwxqywcj.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yuanzhike.top/gtllfqzjri.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.52xcode.cn/gtjvlxuugu.html

Go:   // 双指针从两端比较
来源：http://hz.cashguo.top/gtixpmwoih.html

Ruby: s == s.reverse
来源：http://hz.jqgfzy.top/gtszzvekhp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yj20258.top/gtiuynajyp.html

[N07] 两数之和（返回下标）
来源：http://hz.shuidangran.top/gteymdmlba.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.wangdashe.top/gtsjojcsyo.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.guowangkeji.top/gtukuulwwo.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.gogol.net.cn/gtsevxgdxg.html

TS:   // 手写 Map<string, number>
来源：http://hz.yj20258888.top/gtqnignkvt.html

Java: // 手写 HashMap
来源：http://hz.jqgufenzy.top/gtmgnwowtw.html

Go:   // 手写 map[int]int
来源：http://hz.jqgfzy.top/gtgoypcqbk.html

Ruby: // 手写 Hash
来源：http://hz.meibo888.top/gtojtjivhz.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.iojbl.cn/gtppmmdkzz.html

[N08] 生成全排列
来源：http://hz.c1oappe.top/gtruynzotn.html

Py:   itertools.permutations(arr)
来源：http://hz.guannengcc.top/gtvylroesx.html

PHP:  // 手写递归交换
来源：http://hz.fzhhl.top/gtusfadvpb.html

JS:   // 手写回溯递归
来源：http://hz.sweek.top/gtkifmdenq.html

TS:   // 手写回溯递归
来源：http://hz.0kj1m.cn/gtsnmvjmyq.html

Java: // 手写回溯递归
来源：http://hz.0kj1m.cn/gtgcmxsbcn.html

Go:   // 手写回溯递归
来源：http://hz.birdmap.top/gtbllzwcap.html

Ruby: arr.permutation.to_a
来源：http://hz.yangfankeji.com/gtmpiwabzs.html

C#:   // 手写回溯递归
来源：http://hz.chenzaomai.com/gtopajiwmk.html

[N09] 栈与队列
来源：http://hz.aibaodan.cn/gtnjkqxkum.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.zdqjudy.top/gtispircgt.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.birdmap.top/gtnnuxdkwj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.svipenyu.cn/gtqqqtzhel.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.fzhhl.top/gtaryufpnv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.cashguo.top/gtqytfrupu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.quarkkingdee.top/gtffzopeho.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.aizwys.cn/gtewlrurmo.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.pycfn.com/gtfdjubwkb.html

[N10] 链表节点定义
来源：http://hz.guannengcc.top/gtvgnuqhzr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.pengpengdd.cyou/gtweskdwnd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.chenlongwang.top/gtodntgztl.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zycfv.cn/gtgtyjjbkt.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.sufxvd.cn/gtigkmazrr.html

Java: class Node { int v; Node next; }
来源：http://hz.chenlongwang.top/gtkfapswla.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.ivvv.top/gtbngqvpym.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.9152youxi.cn/gtjsbdnkfy.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.bjfxy.top/gtoagnnwgn.html

[N11] 二叉树中序遍历
来源：http://hz.ywan-chungtsiang.top/gtabggcfyt.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.fzhhl.top/gtbardgelj.html

PHP:  // 手写递归函数
来源：http://hz.aizwys.cn/gthnwqpzga.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.chenjidiqi.icu/gtwrpyknem.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.smart0.xyz/gtulihxvof.html

Java: // 手写递归
来源：http://hz.guannengcc.top/gtsyvegflq.html

Go:   // 手写递归
来源：http://hz.0kj1m.cn/gtwwdrhumw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.yuxming.cn/gtwzqxcpne.html

C#:   // 手写递归
来源：http://hz.pengpengdd.cyou/gtmadxrplf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.nwbrower.top/gtmlrhulpg.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.zhijiandao.cn/gtpjxtkvsf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.shanyushiyangkeji.top/gtmxzoslac.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hammf.cn/gttwzknhyl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhongyouzk.top/gtweelddad.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ydjk.org.cn/gtwfelgtlx.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.yanxiufei.cn/gtyddveykq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.bjfxy.top/gtkwdjwwap.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhixingplan.top/gtgbgudlcm.html

================================================================================
来源：http://hz.hnxiangtu.top/gtodlewspo.html

O. 并发与异步
来源：http://hz.xingfuxueyuan.xyz/gtcbetzhny.html

================================================================================
来源：http://hz.zdqjudy.top/gtmlhwmizg.html

[O01] 启动一个线程
来源：http://hz.xuanzx.com/gteemenvye.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.gaohongyu789.top/gtdcxzuwlt.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.sxryk.cn/gtklqqrabk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.bjfxy.top/gtsytqderk.html

TS:   // 同 JS
来源：http://hz.xziqi.cn/gtbkkejmun.html

Java: new Thread(() -> f()).start()
来源：http://hz.redwolf501.top/gtxiocxzep.html

Go:   go f()
来源：http://hz.bjfxy.top/gtjkccomuq.html

Ruby: Thread.new { f }
来源：http://hz.andypj.xyz/gttsrpsinl.html

C#:   Task.Run(() => F());
来源：http://hz.guannengcc.top/gtytqwwcgr.html

[O02] 使用线程池
来源：http://hz.guowangkeji.top/gttminoefj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.chenzaomai.com/gtvqwafsdj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.havefunace.top/gtpihmwvgt.html

JS:   // worker_threads 线程池
来源：http://hz.yj20258888.top/gtwdlmhjzd.html

TS:   // worker_threads 线程池
来源：http://hz.aibaodan.cn/gtioeefizt.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.cashguo.top/gtdglccadz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.snrcjt.cn/gtxuzafcpw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.nwbrower.top/gtbdhdbsmz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.aizwys.cn/gtgxjxinhk.html

[O03] 加锁保护共享数据
来源：http://hz.jqgufenzy.top/gtsackbqel.html

Py:   with lock: shared += 1
来源：http://hz.iojbl.cn/gtbadoycdn.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zhoulong.xyz/gtddpbcoux.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.hnxiangtu.top/gtisciujyx.html

TS:   // 同 JS
来源：http://hz.jyoumei.cn/gtkxswcdve.html

Java: synchronized (this) { shared++; }
来源：http://hz.smart0.xyz/gtocaqahxn.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.ywan-chungtsiang.top/gtzdhvkcdd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jinqigfzy.top/gtlsvcpepu.html

C#:   lock (gate) { shared++; }
来源：http://hz.jianghu66.top/gtgymsxldj.html

[O04] 定义异步函数并等待
来源：http://hz.fzhhl.top/gtqngjczjd.html

Py:   async def f():⏎    await g()
来源：http://hz.quarkkingdee.top/gthkpkseio.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.sysykeji.top/gtfovrdwxw.html

JS:   async function f() { await g(); }
来源：http://hz.ppjwa.cn/gttosssnja.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.ybcxt.top/gtxqauilcg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.ivvv.top/gterinbgwf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.shanyushiyangtech.top/gtjgjbmdmt.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.mhx1999.top/gtetqgncuh.html

C#:   async Task F() { await G(); }
来源：http://hz.cqqwz.cn/gtdbuyahqi.html

[O05] 并发执行并等待全部完成
来源：http://hz.ivvv.top/gtuxrtlwcy.html

Py:   asyncio.gather(*tasks)
来源：http://hz.ehwqpu.com/gtmtcxqltf.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.xylfe.cn/gtselbcqtd.html

JS:   await Promise.all(tasks)
来源：http://hz.9152youxi.cn/gtijgjraik.html

TS:   await Promise.all(tasks)
来源：http://hz.iojbl.cn/gtowudlfqx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.yj20258888.top/gtznocbtfs.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.ehwqpu.com/gthfedzctv.html

Ruby: threads.map(&:join)
来源：http://hz.yuxming.cn/gtqldozcxa.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.chenlongwang.top/gtvyxbrcqg.html

[O06] 使用进程池
来源：http://hz.daxiang520.top/gtkxoptwgr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.hnxiangtu.top/gtasmedkvl.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.mhx1999.top/gtlpauywsb.html

JS:   // child_process / cluster 模块
来源：http://hz.yonumen.top/gtnbshfojg.html

TS:   // child_process / cluster 模块
来源：http://hz.mhx1999.top/gtvoqyuwrn.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.shuidangran.top/gtbeqnriod.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.jinyuanbaomall.cn/gtcujogowj.html

Ruby: // fork 块
来源：http://hz.yanxiufei.cn/gtefoajadr.html

C#:   Parallel.For
来源：http://hz.ydjk.org.cn/gtogjvulgd.html

================================================================================
来源：http://hz.tianlin.xyz/gtrfvxxspl.html

P. 常用工具函数
来源：http://hz.bjfxy.top/gtoxrysquo.html

================================================================================
来源：http://hz.tian-w.cn/gtzlkqptol.html

[P01] 生成 UUID
来源：http://hz.yvedp.cn/gtxzubfgbz.html

Py:   str(uuid.uuid4())
来源：http://hz.ywan-chungtsiang.top/gtoiprztch.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yanxiufei.cn/gtuqnrybym.html

JS:   crypto.randomUUID()
来源：http://hz.daria6918.cn/gtbmyrmuhn.html

TS:   crypto.randomUUID()
来源：http://hz.pengpengdd.cyou/gtqcrcurtd.html

Java: UUID.randomUUID().toString()
来源：http://hz.gzhubu.top/gtbgbptniq.html

Go:   // 用 github.com/google/uuid
来源：http://hz.mhx1999.top/gthgvmsdox.html

Ruby: SecureRandom.uuid
来源：http://hz.svipenyu.cn/gteuqewrtf.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.sxryk.cn/gtaiaixpqp.html

[P02] MD5 / SHA256 摘要
来源：http://hz.zhaomingkeji.xyz/gtyutoywkx.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.zhixingplan.top/gtlsgtpaod.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.zycfv.cn/gtrdlgrubd.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.meibo888.top/gtgpbnosqv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.guowangkeji.top/gtybhrsznd.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.jianghu66.top/gtfgvvbofg.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.shanyushiyangkeji.top/gtnaztjgvd.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.daxiang520.top/gtbjtrifvk.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.havefunace.top/gteiztlwvj.html

[P03] 生成短随机字符串
来源：http://hz.shanyushiyangkeji.top/gtzwgnsdbv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.zhengqikj.top/gteqbmfzer.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.guannengcc.top/gtqgyuuevx.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jinqigfzy.top/gtkdqbvzet.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ivvv.top/gtnnmbfchh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.shuidangran.top/gtcdhhgejg.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.sufxvd.cn/gtesqqhghp.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.hongshengwenyu.top/gthrnjuylg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.yueranfly.top/gtpyzmcghp.html

[P04] 求长度
来源：http://hz.yvedp.cn/gtujtlsogt.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.wangdashe.top/gtwpjieast.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yueranfly.top/gtzwsepyuf.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hongshengwenyu.top/gtlfvqyurh.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhongyouzk.top/gtwpytsnqx.html

Java: list.size();  map.size();  s.length()
来源：http://hz.nwbrower.top/gtvjbhjfdf.html

Go:   len(arr);  len(m)
来源：http://hz.sufxvd.cn/gtgjapvyjo.html

Ruby: x.length;  x.size
来源：http://hz.haohaochexian.top/gtlukycevy.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.haohaochexian.top/gtohrlrmde.html

[P05] 判断两个对象内容是否相等
来源：http://hz.bjfxy.top/gtfyebmbzh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.kuanghao11.cn/gtdxwyuocr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.cashguo.top/gtptcvanat.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.jyoumei.cn/gtlalmyknu.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.chenjidiqi.icu/gtiwslmbli.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.dashuyun.cn/gtkzojpqpw.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.pycfn.com/gtoqeirqta.html

Ruby: a == b
来源：http://hz.tanke756.top/gtfevfssbq.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.dashuyun.cn/gtckroutoo.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.kuanghao11.cn/gtgazdkxwa.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.sweek.top/gtffygrijy.html

PHP:  if (empty($x)) {}
来源：http://hz.nanxinkj.top/gtgkoxciab.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.andypj.xyz/gthfkrzoxl.html

TS:   if (x == null) {}
来源：http://hz.daxiang520.top/gtyzwyegfn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.shanyushiyangtech.top/gtdxjnqidg.html

Go:   if x == nil {}
来源：http://hz.zhiwuduotai.top/gtldknfhlf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.nwbrower.top/gtualwkite.html

C#:   if (x is null) {}
来源：http://hz.yvedp.cn/gtdmospfmz.html

[P07] 防抖与节流
来源：http://hz.hnqzz.top/gtnriheglh.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.gaohongyu789.top/gtxklohwaz.html

PHP:  // 手写时间戳比较
来源：http://hz.yj20258888.top/gtedyegyts.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.nanxinkj.top/gtjdximgaf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hnqzz.top/gtsegefxmm.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.kuanghao11.cn/gtufrziyng.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.xingfuxueyuan.xyz/gtrforldax.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.meibo888.top/gtchxmxfkl.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.zhongyouzk.top/gtktwmltux.html

[P08] 处理浮点精度问题
来源：http://hz.52xcode.cn/gthkgmacdy.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.cheryme.top/gtvyjggwdq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.zhaomingkeji.xyz/gteyhcdsik.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.jqgufenzy.top/gtxeignnzm.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.chenzaomai.com/gtvwgrkrxp.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.52xcode.cn/gtxpcgjzqa.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.fengsongda.top/gtdfrwkklr.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.jqgfzy.top/gtlvadxhov.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.shzxlz.cn/gtnvydvwdy.html

================================================================================
来源：http://hz.shzxlz.cn/gtasmiplwf.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.52xcode.cn/gtyofuzyma.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtftnvqxqk.html

[Q01] 创建表
来源：http://hz.chenzaomai.com/gtnkhcisvh.html

CREATE TABLE users (
来源：http://hz.gotoacloud.top/gtxpiskurw.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.bjfxy.top/gtheluayfj.html

name VARCHAR(50) NOT NULL,
来源：http://hz.gogol.net.cn/gthwijxxrd.html

email VARCHAR(100) UNIQUE,
来源：http://hz.ydjk.org.cn/gtarcatezl.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.daxiang520.top/gtmfiyeojz.html

);
来源：http://hz.jinqigfzy.top/gtyooegnmh.html

[Q02] 创建带外键的表
来源：http://hz.xuetiantiany.cn/gtdnawzknk.html

CREATE TABLE orders (
来源：http://hz.kuanghao11.cn/gthomelpvs.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ybcxt.top/gtopslgbgm.html

user_id INT NOT NULL,
来源：http://hz.bjfxy.top/gtftvzixca.html

amount DECIMAL(10, 2),
来源：http://hz.dianchejie.cn/gtbjeuxqxq.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.fengsongda.top/gtdzpwnloa.html

);
来源：http://hz.gotoacloud.top/gtiqcppdac.html

[Q03] 增加列
来源：http://hz.iojbl.cn/gtprshvpzn.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.chenlongwang.top/gtszytlxyy.html

[Q04] 修改列类型
来源：http://hz.ywan-chungtsiang.top/gtvnmdufel.html


<!-- 参考信息 -->