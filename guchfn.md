代发 wailian999

Py:   if __name__ == "__main__":
来源：http://hz.tianlin.xyz/gtxjzqtekn.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.feifeiyinyue.top/gtqxdyegzv.html

JS:   require.main === module
来源：http://hz.ybcxt.top/gtorqweocy.html

TS:   require.main === module
来源：http://hz.xziqi.cn/gtrcdazgzx.html

Java: public static void main(String[] args)
来源：http://hz.ybcxt.top/gteillndam.html

Go:   func main()
来源：http://hz.guowangkeji.top/gttswpmzov.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.xinyue.icu/gtjfvsknpf.html

C#:   static void Main(string[] args)
来源：http://hz.zhijiandao.cn/gtbqtutpco.html

[M08] 获取系统与运行时信息
来源：http://hz.tian-w.cn/gtxilagqvt.html

Py:   platform.system();  platform.python_version()
来源：http://hz.hywenlv.cn/gtkidpluqs.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.jyoumei.cn/gtgdkgvjjb.html

JS:   process.platform;  process.version
来源：http://hz.sysykeji.top/gtjmijenjb.html

TS:   process.platform;  process.version
来源：http://hz.gzhubu.top/gthgbaxuzv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.yj20258888.top/gtbuxvhobt.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.ybcxt.top/gtombmfmtp.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.zhengqikj.top/gtlennfwiz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.shanyushiyangtech.top/gtzolmesae.html

================================================================================
来源：http://hz.daria6918.cn/gttohddblv.html

N. 数据结构与算法
来源：http://hz.iojbl.cn/gthnjlmnno.html

================================================================================
来源：http://hz.0kj1m.cn/gtstieguah.html

[N01] 二分查找（有序数组）
来源：http://hz.jqgufenzy.top/gtianvxapm.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.xziqi.cn/gtcqehswyd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.ppjwa.cn/gtwllrlssa.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.shzxlz.cn/gtytsgpdqs.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.vqdsnc.cn/gttvzkyima.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.wangdashe.top/gtjibtpqes.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.xinyue.icu/gthedfjeuc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.sxryk.cn/gtrttukhpi.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.gzhubu.top/gtwepgkcrp.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.bjfxy.top/gtoyspxpsu.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hfpthk.cn/gtwcfhzjjn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.316326.xyz/gtahaqelbk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.vqdsnc.cn/gtneihsppn.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.pycfn.com/gtpjqirxcj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.jinqigufen.top/gtiwepwpjq.html

Go:   slices.Sort(arr)
来源：http://hz.sufxvd.cn/gtehzzldhk.html

Ruby: arr.sort
来源：http://hz.zhengqikj.top/gtxeabwvqv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.ppjwa.cn/gthczmslfd.html

[N03] 快速排序（分治示例）
来源：http://hz.c1oappe.top/gtptgdvwdi.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.cheryme.top/gtaekzxqns.html

PHP:  // 递归实现，或用 usort
来源：http://hz.wangshuangyany.cn/gtgzsaybfu.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.kuanghao11.cn/gtuncrxpkp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xuanzx.com/gtleohkjxw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.c1oappe.top/gtkkudrgbf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.kuanghao11.cn/gtrttovurf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yangfankeji.com/gttqhesaes.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yvedp.cn/gtagcrrtwq.html

[N04] 斐波那契数列
来源：http://hz.redwolf501.top/gtqcuhnmnz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jinghuilouyu.cn/gtijowwovj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.cdnleiting.top/gtbozuzqio.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yuxming.cn/gtadzledun.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jqgfzy.top/gtnhlebkso.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.hnxiangtu.top/gtbhigseso.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.9152youxi.cn/gtyxuajlby.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.tian-w.cn/gtbyixhpma.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.guowangkeji.top/gtszybnhpm.html

[N05] 最大公约数
来源：http://hz.gzhubu.top/gttsxulvnc.html

Py:   math.gcd(a, b)
来源：http://hz.xingfuxueyuan.xyz/gtpzypicyx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.snrcjt.cn/gtnvpoybql.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hammf.cn/gtmskzbhel.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ywan-chungtsiang.top/gtxxlgopwg.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.jinqigufen.top/gtsitukphe.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.yanxiufei.cn/gtqvhzagal.html

Ruby: a.gcd(b)
来源：http://hz.tian-w.cn/gtzcjjhgqc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.316326.xyz/gttdsqylsf.html

[N06] 判断回文字符串
来源：http://hz.fengsongda.top/gtdnjokllg.html

Py:   s == s[::-1]
来源：http://hz.hywenlv.cn/gtvmpqapru.html

PHP:  $s === strrev($s);
来源：http://hz.fengsongda.top/gtzefpsxkp.html

JS:   s === [...s].reverse().join("")
来源：http://hz.gaohongyu789.top/gtkbfkenly.html

TS:   s === [...s].reverse().join("")
来源：http://hz.iojbl.cn/gtuqmuohyd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.gotoacloud.top/gtmivuehzf.html

Go:   // 双指针从两端比较
来源：http://hz.vqdsnc.cn/gtulynrjao.html

Ruby: s == s.reverse
来源：http://hz.guowangkeji.top/gtrecxgtxg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.aizwys.cn/gtjolsgfhj.html

[N07] 两数之和（返回下标）
来源：http://hz.aizwys.cn/gtnnkvodzj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.quarkkingdee.top/gtvfqdcvwg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.xylfe.cn/gtrunljimp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.jqgfzy.top/gtpnleobnm.html

TS:   // 手写 Map<string, number>
来源：http://hz.jinqigfzy.top/gtexawyval.html

Java: // 手写 HashMap
来源：http://hz.ivvv.top/gtqiwhuisx.html

Go:   // 手写 map[int]int
来源：http://hz.nanxinkj.top/gtizliawot.html

Ruby: // 手写 Hash
来源：http://hz.sysykeji.top/gtfqqiuxne.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.gzhubu.top/gtokujlmft.html

[N08] 生成全排列
来源：http://hz.cheryme.top/gttcnxbzqq.html

Py:   itertools.permutations(arr)
来源：http://hz.hfpthk.cn/gtuagzxvpg.html

PHP:  // 手写递归交换
来源：http://hz.guowangkeji.top/gtrnkgtdrj.html

JS:   // 手写回溯递归
来源：http://hz.nanxinkj.top/gtuifvdcac.html

TS:   // 手写回溯递归
来源：http://hz.hongshengwenyu.top/gtwzhouvzf.html

Java: // 手写回溯递归
来源：http://hz.jianghu66.top/gteydtaqlh.html

Go:   // 手写回溯递归
来源：http://hz.pengpengdd.cyou/gtljeixuyf.html

Ruby: arr.permutation.to_a
来源：http://hz.gzhubu.top/gtujmtvmdj.html

C#:   // 手写回溯递归
来源：http://hz.guannengcc.top/gtnisiukzr.html

[N09] 栈与队列
来源：http://hz.ydzc1.top/gtrunwzjzv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yuanzhike.top/gtvpyhtkky.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.xinyue.icu/gtibvcwrdn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yuanzhike.top/gtotgmmomv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.ydjk.org.cn/gtrlziyjnm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.jianghu66.top/gtvxjxpihh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.daxiang520.top/gtvwwysqjk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.zhaomingkeji.xyz/gtgnzvrawr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.hfpthk.cn/gtolcvvvuw.html

[N10] 链表节点定义
来源：http://hz.aibaodan.cn/gtglgyensw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.sufxvd.cn/gtzubaeesw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.hammf.cn/gtmvkgezgp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.tanke756.top/gtfbmvyhxg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.ydjk.org.cn/gtcntkqdli.html

Java: class Node { int v; Node next; }
来源：http://hz.bjfxy.top/gtjgqjcdmd.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.wangshuangyany.cn/gtyyxmlmdb.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.nanxuanxn.top/gthvyustex.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yj20258.top/gtnjqfxgbm.html

[N11] 二叉树中序遍历
来源：http://hz.yj202588.top/gtidxrhgbe.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.yj20258.top/gtnsybcicc.html

PHP:  // 手写递归函数
来源：http://hz.shanyushiyangkeji.top/gtqwegjktt.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.shuidangran.top/gtnhoiinhg.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ybcxt.top/gtvtgnkdke.html

Java: // 手写递归
来源：http://hz.yvedp.cn/gtsvieilcx.html

Go:   // 手写递归
来源：http://hz.hnxiangtu.top/gtvqdkpxto.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.cqqwz.cn/gtirpmffbr.html

C#:   // 手写递归
来源：http://hz.xuanzx.com/gtvpdkxbmm.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.chenjidiqi.icu/gtcvpbuavu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.jqgufenzy.top/gtrginskrk.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.dashuyun.cn/gtvkykozoq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhiwuduotai.top/gtbxxwykvt.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhiwuduotai.top/gtzsnnvnmt.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.andypj.xyz/gtzoryyiwo.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.guannengcc.top/gtgimefswn.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.smart0.xyz/gtyoersmki.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.chenjidiqi.icu/gtktestvyl.html

================================================================================
来源：http://hz.dashuyun.cn/gtiheccqyc.html

O. 并发与异步
来源：http://hz.snrcjt.cn/gtbgnoaznt.html

================================================================================
来源：http://hz.smart0.xyz/gtlunzgrdo.html

[O01] 启动一个线程
来源：http://hz.fengsongda.top/gtgtuwprck.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.sweek.top/gtsfhnistr.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.xuanzx.com/gtqzglfjmn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.zycfv.cn/gtvlibouuo.html

TS:   // 同 JS
来源：http://hz.andypj.xyz/gtypykwzho.html

Java: new Thread(() -> f()).start()
来源：http://hz.jiagoushi.top/gtedonbxmg.html

Go:   go f()
来源：http://hz.dashuyun.cn/gtkkpiuhpv.html

Ruby: Thread.new { f }
来源：http://hz.ivvv.top/gtysafxplc.html

C#:   Task.Run(() => F());
来源：http://hz.quarkkingdee.top/gtgbsvnxdk.html

[O02] 使用线程池
来源：http://hz.wangdashe.top/gtztuwyvjx.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yuanzhike.top/gtjyxxhncv.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.shzxlz.cn/gtppnknrav.html

JS:   // worker_threads 线程池
来源：http://hz.0kj1m.cn/gtwgcacbui.html

TS:   // worker_threads 线程池
来源：http://hz.jiagoushi.top/gtukgwwzfm.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.feifeiyinyue.top/gtqievckxk.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.xziqi.cn/gtabdtpzqq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.shzxlz.cn/gtwtxsgvhe.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.316326.xyz/gtzqzjfzqt.html

[O03] 加锁保护共享数据
来源：http://hz.ppjwa.cn/gtxlwgjcur.html

Py:   with lock: shared += 1
来源：http://hz.sufxvd.cn/gtaznvewgu.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.jlsjyb.cn/gtnqzxawxe.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.cdnleiting.top/gtdxjyueiu.html

TS:   // 同 JS
来源：http://hz.snrcjt.cn/gtqzvwxfoq.html

Java: synchronized (this) { shared++; }
来源：http://hz.ywan-chungtsiang.top/gtvwaqxfvf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.zhongyouzk.top/gtlllpxjfx.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.havefunace.top/gtelfievun.html

C#:   lock (gate) { shared++; }
来源：http://hz.ehwqpu.com/gtttysvzhh.html

[O04] 定义异步函数并等待
来源：http://hz.cashguo.top/gtycasenjk.html

Py:   async def f():⏎    await g()
来源：http://hz.aibaodan.cn/gtsehyzcdc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.cheryme.top/gtvssrdgua.html

JS:   async function f() { await g(); }
来源：http://hz.yueranfly.top/gtcqdttayr.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.haohaochexian.top/gtpbbvbqxj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.gotoacloud.top/gtdtqoclgj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.iojbl.cn/gtnvgtuzgt.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.ivvv.top/gttdmbibol.html

C#:   async Task F() { await G(); }
来源：http://hz.zhixingplan.top/gtlwbqnwqj.html

[O05] 并发执行并等待全部完成
来源：http://hz.sweek.top/gtbsevhsvu.html

Py:   asyncio.gather(*tasks)
来源：http://hz.snrcjt.cn/gtfqyxogfe.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.yonumen.top/gtnkhkbfly.html

JS:   await Promise.all(tasks)
来源：http://hz.nanxuanxn.top/gtyenckhsc.html

TS:   await Promise.all(tasks)
来源：http://hz.meibo888.top/gtnddrsdqr.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.hnxiangtu.top/gturyexnno.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.tianlin.xyz/gtvcsztoei.html

Ruby: threads.map(&:join)
来源：http://hz.zdqjudy.top/gtwneavyma.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.hywenlv.cn/gtdmhbotxv.html

[O06] 使用进程池
来源：http://hz.shanyushiyangtech.top/gtugfxpbbi.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.hongshengwenyu.top/gtfnihhtcg.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.yueranfly.top/gtlquarmvr.html

JS:   // child_process / cluster 模块
来源：http://hz.yuanzhike.top/gtweehohmj.html

TS:   // child_process / cluster 模块
来源：http://hz.yuanzhike.top/gtcowmzwla.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yongpay.top/gtgmtxrdbg.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.jinghuilouyu.cn/gtjvrrabwb.html

Ruby: // fork 块
来源：http://hz.52xcode.cn/gtfzjypeip.html

C#:   Parallel.For
来源：http://hz.yj20258888.top/gtmrinfpxh.html

================================================================================
来源：http://hz.tanke756.top/gtxbhzbmkk.html

P. 常用工具函数
来源：http://hz.aizwys.cn/gtuswgrrrc.html

================================================================================
来源：http://hz.quarkkingdee.top/gtsguanmov.html

[P01] 生成 UUID
来源：http://hz.gzhubu.top/gtdmtrysva.html

Py:   str(uuid.uuid4())
来源：http://hz.hfpthk.cn/gtmbmzkeii.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.fzhhl.top/gtsybbrkdb.html

JS:   crypto.randomUUID()
来源：http://hz.zhixingplan.top/gtdzsflmms.html

TS:   crypto.randomUUID()
来源：http://hz.zhiwuduotai.top/gtqnqtjcxh.html

Java: UUID.randomUUID().toString()
来源：http://hz.havefunace.top/gtndbufpxk.html

Go:   // 用 github.com/google/uuid
来源：http://hz.hongshengwenyu.top/gtzgiwoqea.html

Ruby: SecureRandom.uuid
来源：http://hz.yonumen.top/gtvmqzeptt.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.yangfankeji.com/gtfsmtumri.html

[P02] MD5 / SHA256 摘要
来源：http://hz.svipenyu.cn/gtbsxwfymg.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.sufxvd.cn/gtbgdkphwi.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.yuanzhike.top/gtbmtpsmhp.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.haohaochexian.top/gtruwvivhl.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jinqigfzy.top/gtmyyevnur.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.sweek.top/gtqpecgivs.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.52xcode.cn/gtdoxijigu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.zhengqikj.top/gtlppdxjff.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.zhijiandao.cn/gtmjmlrlpp.html

[P03] 生成短随机字符串
来源：http://hz.pengpengdd.cyou/gtbevrview.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.havefunace.top/gtqxtjiowl.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.9152youxi.cn/gtinbevjml.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yvedp.cn/gthyfpslwv.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xuetiantiany.cn/gtikrxvntf.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.aizwys.cn/gtersycwqx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.pengpengdd.cyou/gtfsmntnmc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jinqigfzy.top/gtvxkkfvzn.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.cashguo.top/gtwwrysmse.html

[P04] 求长度
来源：http://hz.xuetiantiany.cn/gtlcgirjzz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.andypj.xyz/gtknvdaquk.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.gaohongyu789.top/gtoizqybcz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jyoumei.cn/gtvpekisux.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hnxiangtu.top/gtmesrcipm.html

Java: list.size();  map.size();  s.length()
来源：http://hz.birdmap.top/gtbtzykyjg.html

Go:   len(arr);  len(m)
来源：http://hz.316326.xyz/gtzvoyopwf.html

Ruby: x.length;  x.size
来源：http://hz.bjfxy.top/gtftlchrau.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.c1oappe.top/gtynpsuyst.html

[P05] 判断两个对象内容是否相等
来源：http://hz.nanxuanxn.top/gtpnebpyxq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.hongshengwenyu.top/gtkeajnzcl.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.jinghuilouyu.cn/gtvpufnxeq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.xziqi.cn/gtbciqgolj.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.hysaishi.cn/gtwryuwqjh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.zhaomingkeji.xyz/gttjqmuwrq.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.ydzc1.top/gtpjknccpl.html

Ruby: a == b
来源：http://hz.xuanzx.com/gtqnwqhylb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.vqdsnc.cn/gttwfsthqn.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.gaohongyu789.top/gtimdbvycl.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.yonumen.top/gtyhkckogb.html

PHP:  if (empty($x)) {}
来源：http://hz.haohaochexian.top/gtbzrgcthg.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.yanxiufei.cn/gtomnvhpjl.html

TS:   if (x == null) {}
来源：http://hz.kuanghao11.cn/gtepkchwgj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.xuanzx.com/gtobcqhhgk.html

Go:   if x == nil {}
来源：http://hz.hfpthk.cn/gtuxldypnk.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jqgfzy.top/gtoqnsbmiv.html

C#:   if (x is null) {}
来源：http://hz.daria6918.cn/gtjbeylwdp.html

[P07] 防抖与节流
来源：http://hz.yvedp.cn/gtvjhsidao.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.gaohongyu789.top/gtdasxvgax.html

PHP:  // 手写时间戳比较
来源：http://hz.redwolf501.top/gtbrisicjt.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hnxiangtu.top/gtgixklzmx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jinyuanbaomall.cn/gtotglegpy.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.zhongyouzk.top/gtnvnlsnyc.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.ybcxt.top/gtbfvazino.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.nanxuanxn.top/gtdlcvagkh.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.nwbrower.top/gtptuydlkt.html

[P08] 处理浮点精度问题
来源：http://hz.iojbl.cn/gtktoppsgk.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.haohaochexian.top/gtghdbpzwu.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.chenzaomai.com/gtdiossatw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.c1oappe.top/gtnsxxgneb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.xuetiantiany.cn/gthsnclwjb.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.zhixingplan.top/gtgbguqoyl.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.chenzaomai.com/gtqspdonxj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.nwbrower.top/gtemkopeiq.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.yj20258888.top/gtolfjgbaz.html

================================================================================
来源：http://hz.pycfn.com/gtjatykiyd.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.vqdsnc.cn/gtoabfhpkb.html

================================================================================
来源：http://hz.iojbl.cn/gtmnletbdz.html

[Q01] 创建表
来源：http://hz.chenjidiqi.icu/gtfxzpwgza.html

CREATE TABLE users (
来源：http://hz.hfpthk.cn/gtymcjjauf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hongshengwenyu.top/gtsoutbeau.html

name VARCHAR(50) NOT NULL,
来源：http://hz.bjfxy.top/gtzrbluivp.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jlsjyb.cn/gtqclzwyve.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.zhoulong.xyz/gttfnqnvqm.html

);
来源：http://hz.wangshuangyany.cn/gtgsiahxwx.html

[Q02] 创建带外键的表
来源：http://hz.zhengqikj.top/gtrgwmeziz.html

CREATE TABLE orders (
来源：http://hz.gogol.net.cn/gtiimkyobe.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.sweek.top/gtepykorhu.html

user_id INT NOT NULL,
来源：http://hz.quarkkingdee.top/gtognbpyip.html

amount DECIMAL(10, 2),
来源：http://hz.xinyue.icu/gtizpkvmbq.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.guannengcc.top/gtdxdnfman.html

);
来源：http://hz.zhijiandao.cn/gtxsjzvckm.html

[Q03] 增加列
来源：http://hz.nanxuanxn.top/gtjgjglpjx.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.feifeiyinyue.top/gtbfuyazbo.html

[Q04] 修改列类型
来源：http://hz.hywenlv.cn/gtckpkwmrx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.hfpthk.cn/gtpomcgrod.html

[Q05] 重命名列
来源：http://hz.jyoumei.cn/gtswjjqgsf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.jinyuanbaomall.cn/gtadgjeaub.html

[Q06] 删除列
来源：http://hz.kuanghao11.cn/gtmydqhtjf.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.sysykeji.top/gteqwwvhhi.html

[Q07] 删除表
来源：http://hz.cheryme.top/gtwlmurrbf.html

DROP TABLE IF EXISTS orders;
来源：http://hz.yuanzhike.top/gttsintaay.html

[Q08] 创建普通索引
来源：http://hz.havefunace.top/gtqjhtbxru.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jinghuilouyu.cn/gtoqqncsac.html

[Q09] 创建唯一索引
来源：http://hz.birdmap.top/gtlbazhudd.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.chenjidiqi.icu/gtqfsuqerw.html

[Q10] 插入单行
来源：http://hz.zdqjudy.top/gtrnssaluz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jqgufenzy.top/gtcvbdvmhi.html

[Q11] 一次插入多行
来源：http://hz.chenzaomai.com/gtswbynlez.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.guannengcc.top/gttkasrfas.html

[Q12] 插入后取自增 ID
来源：http://hz.zhongyouzk.top/gtgzdmabpy.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.jqgufenzy.top/gtqmcpppum.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yueranfly.top/gtqnhmvxbj.html

[Q13] 忽略重复插入
来源：http://hz.xuanzx.com/gtgphjhyea.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.shuidangran.top/gttmcluvya.html


<!-- 参考信息 -->