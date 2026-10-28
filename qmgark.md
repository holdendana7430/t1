代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.nwbrower.top/gtfmownyoy.html

JS:   console.error("err")
来源：http://hz.xziqi.cn/gtfdygsytf.html

TS:   console.error("err")
来源：http://hz.jqgfzy.top/gtbdmtqtxy.html

Java: System.err.println("err")
来源：http://hz.yuxming.cn/gtqzjmtsop.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jqgfzy.top/gtzetvworw.html

Ruby: warn "err"
来源：http://hz.redwolf501.top/gtkwhvqytw.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yj20258.top/gtxqgmhwaz.html

[M07] 判断是否为主入口
来源：http://hz.zhoulong.xyz/gtljeblsil.html

Py:   if __name__ == "__main__":
来源：http://hz.zhengqikj.top/gtcacspcnx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.jinyuanbaomall.cn/gtxqnfatph.html

JS:   require.main === module
来源：http://hz.tanke756.top/gtajvzihul.html

TS:   require.main === module
来源：http://hz.hysaishi.cn/gttuiahjar.html

Java: public static void main(String[] args)
来源：http://hz.bjfxy.top/gtmpifoenw.html

Go:   func main()
来源：http://hz.hongshengwenyu.top/gtlwgnayif.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.kuanghao11.cn/gtrylivnmf.html

C#:   static void Main(string[] args)
来源：http://hz.ehwqpu.com/gttuosepdr.html

[M08] 获取系统与运行时信息
来源：http://hz.vqdsnc.cn/gtjgvgxtya.html

Py:   platform.system();  platform.python_version()
来源：http://hz.fzhhl.top/gteeapocpr.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yj20258888.top/gtbugmjwun.html

JS:   process.platform;  process.version
来源：http://hz.ybcxt.top/gtssdstpdg.html

TS:   process.platform;  process.version
来源：http://hz.shangyingyoupin.top/gtjathamkh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.zhaomingkeji.xyz/gtjdohgywo.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jlsjyb.cn/gtnwaanvki.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.xuetiantiany.cn/gtttuwwalg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.shanyushiyangkeji.top/gtaxbxzjns.html

================================================================================
来源：http://hz.xziqi.cn/gtkndeqnvm.html

N. 数据结构与算法
来源：http://hz.jyoumei.cn/gtbltjydts.html

================================================================================
来源：http://hz.yanxiufei.cn/gtiltacaqe.html

[N01] 二分查找（有序数组）
来源：http://hz.jqgfzy.top/gtvvjgcenq.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.jlsjyb.cn/gtegypcbwq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jqgufenzy.top/gtipatgmoa.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.c1oappe.top/gtrdaiyyva.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cucudq.cn/gtomzpkgpv.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.andypj.xyz/gthauhieje.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.yanxiufei.cn/gtpiyuhlob.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.kuanghao11.cn/gthykuoiaf.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.yj202588.top/gtutlevdqe.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.tanke756.top/gtkkrogyqw.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shanyushiyangkeji.top/gtgrlzusnx.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.316326.xyz/gthazrzwuq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.daxiang520.top/gtwycaprpe.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.316326.xyz/gtiistplzo.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.ydjk.org.cn/gttbllnqyf.html

Go:   slices.Sort(arr)
来源：http://hz.shanyushiyangtech.top/gthyeyehlx.html

Ruby: arr.sort
来源：http://hz.iojbl.cn/gtuaamncvl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.yangfankeji.com/gthisyblfl.html

[N03] 快速排序（分治示例）
来源：http://hz.sweek.top/gtvkidsktq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yuanzhike.top/gtshrftcjl.html

PHP:  // 递归实现，或用 usort
来源：http://hz.smart0.xyz/gtygfqvbam.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhaomingkeji.xyz/gtxkgtsfoi.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xziqi.cn/gtgurdlcpb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jlsjyb.cn/gtdqmlvmnx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.gzhubu.top/gtmtvsorvs.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.xuanzx.com/gtynzftmyq.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.cheryme.top/gtscoxlwpm.html

[N04] 斐波那契数列
来源：http://hz.chenzaomai.com/gtiqqgxjyq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.aizwys.cn/gtmgiwkrzt.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.yj20258.top/gtxjbtivrj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.smart0.xyz/gtqudvygik.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ppjwa.cn/gtuawhunqv.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.xinyue.icu/gtjhpzamkg.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jianghu66.top/gtwgxkaria.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.shangyingyoupin.top/gttpbyegre.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.kuanghao11.cn/gtqhmnwvym.html

[N05] 最大公约数
来源：http://hz.gzhubu.top/gtgsqxkwqz.html

Py:   math.gcd(a, b)
来源：http://hz.yongpay.top/gtzpqkuevt.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.ydjk.org.cn/gtxiajshth.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.cashguo.top/gtwhdinfdu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.daxiang520.top/gtqjpdpytt.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.c1oappe.top/gtbngaovxy.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.shangyingyoupin.top/gtcvpnmagd.html

Ruby: a.gcd(b)
来源：http://hz.ydzc1.top/gtvzlmuwdt.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.cqqwz.cn/gtlcppmrfz.html

[N06] 判断回文字符串
来源：http://hz.cqqwz.cn/gtzkccsmtv.html

Py:   s == s[::-1]
来源：http://hz.aibaodan.cn/gtjxzawaww.html

PHP:  $s === strrev($s);
来源：http://hz.jyoumei.cn/gterphqact.html

JS:   s === [...s].reverse().join("")
来源：http://hz.andypj.xyz/gtywtxmzkg.html

TS:   s === [...s].reverse().join("")
来源：http://hz.xinyue.icu/gtydnvmaku.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.andypj.xyz/gtgursoxqn.html

Go:   // 双指针从两端比较
来源：http://hz.zhiwuduotai.top/gtmjpzghlb.html

Ruby: s == s.reverse
来源：http://hz.bjfxy.top/gtuyvcutrq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.sxryk.cn/gtnsvqaxfz.html

[N07] 两数之和（返回下标）
来源：http://hz.snrcjt.cn/gtpbnzxzcj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.cdnleiting.top/gtjdwgpaxp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.zycfv.cn/gtxcdwhvia.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.ppjwa.cn/gtxlwrtjsl.html

TS:   // 手写 Map<string, number>
来源：http://hz.xuanzx.com/gthnzwhkva.html

Java: // 手写 HashMap
来源：http://hz.ywan-chungtsiang.top/gtnzxfoyqg.html

Go:   // 手写 map[int]int
来源：http://hz.ehwqpu.com/gtenvykcpj.html

Ruby: // 手写 Hash
来源：http://hz.yanxiufei.cn/gtcgzhsrcc.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.xuanzx.com/gtepxkefwi.html

[N08] 生成全排列
来源：http://hz.nanxuanxn.top/gtgwplllbm.html

Py:   itertools.permutations(arr)
来源：http://hz.bjfxy.top/gtligbpyfh.html

PHP:  // 手写递归交换
来源：http://hz.hysaishi.cn/gtnhtvklrq.html

JS:   // 手写回溯递归
来源：http://hz.hywenlv.cn/gtgypytbug.html

TS:   // 手写回溯递归
来源：http://hz.gotoacloud.top/gtthvdusbe.html

Java: // 手写回溯递归
来源：http://hz.hnxiangtu.top/gtkcxjdgru.html

Go:   // 手写回溯递归
来源：http://hz.ywan-chungtsiang.top/gtmzmsavlf.html

Ruby: arr.permutation.to_a
来源：http://hz.jinqigfzy.top/gtncxmmzqp.html

C#:   // 手写回溯递归
来源：http://hz.zhengqikj.top/gtkhudqsbs.html

[N09] 栈与队列
来源：http://hz.yj20258.top/gtyjwkdbgp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.shzxlz.cn/gtjpelyayc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.xingfuxueyuan.xyz/gtjzyhxeqm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.ivvv.top/gtfypskzjt.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.fengsongda.top/gtnryzrrfy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.c1oappe.top/gthfkhpanm.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.zhongyouzk.top/gtszcwqena.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.hammf.cn/gtosxhzbjo.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.zhaomingkeji.xyz/gtjisacnsx.html

[N10] 链表节点定义
来源：http://hz.ehwqpu.com/gtucvatcyn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.ehwqpu.com/gtsluenewp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jlsjyb.cn/gtkwodknpy.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.gogol.net.cn/gtvdszqszj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.yueranfly.top/gtwgiqczcr.html

Java: class Node { int v; Node next; }
来源：http://hz.snrcjt.cn/gtcxtcfcjf.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.pycfn.com/gtldgjkkox.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.daria6918.cn/gtyssehgan.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.0kj1m.cn/gtawoxqszq.html

[N11] 二叉树中序遍历
来源：http://hz.pycfn.com/gtktovoycv.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.feifeiyinyue.top/gtsuglybgk.html

PHP:  // 手写递归函数
来源：http://hz.yangfankeji.com/gtpxkyutpn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.xingfuxueyuan.xyz/gtwjctqxzz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhoulong.xyz/gthdkkflph.html

Java: // 手写递归
来源：http://hz.316326.xyz/gtopkftwmu.html

Go:   // 手写递归
来源：http://hz.jianghu66.top/gtelegzhna.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.316326.xyz/gtgteottbw.html

C#:   // 手写递归
来源：http://hz.yuanzhike.top/gtarwmkniv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.daria6918.cn/gtvmlwhyff.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.cqqwz.cn/gtcwikhllg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.gotoacloud.top/gtpihmacjs.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.9152youxi.cn/gtkquzhhez.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.316326.xyz/gtxdnycszf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yj20258888.top/gtytghiyei.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.mhx1999.top/gtucbyseaq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.daria6918.cn/gtqewdpqzu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.sweek.top/gtokimwbmw.html

================================================================================
来源：http://hz.daxiang520.top/gtsfucrqgn.html

O. 并发与异步
来源：http://hz.bjfxy.top/gtqehhblcc.html

================================================================================
来源：http://hz.cucudq.cn/gtctcuxhrq.html

[O01] 启动一个线程
来源：http://hz.nanxinkj.top/gtpkwxchlp.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.gogol.net.cn/gtiewzwxhd.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.zhengqikj.top/gtzzxtzezc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.hysaishi.cn/gtvdpvlgjf.html

TS:   // 同 JS
来源：http://hz.gogol.net.cn/gttzfwnfcc.html

Java: new Thread(() -> f()).start()
来源：http://hz.pengpengdd.cyou/gtxqdqawpl.html

Go:   go f()
来源：http://hz.52xcode.cn/gthnnubojq.html

Ruby: Thread.new { f }
来源：http://hz.52xcode.cn/gtghnstvdk.html

C#:   Task.Run(() => F());
来源：http://hz.cdnleiting.top/gtjacbdnqo.html

[O02] 使用线程池
来源：http://hz.zycfv.cn/gtfdlbxhgx.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.shanyushiyangtech.top/gtkpeoirye.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.zycfv.cn/gteguwcmkt.html

JS:   // worker_threads 线程池
来源：http://hz.aizwys.cn/gtwpwuughi.html

TS:   // worker_threads 线程池
来源：http://hz.feifeiyinyue.top/gtwgmmulsj.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.cdnleiting.top/gtuxvldpow.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.gzhubu.top/gtxckrjwnx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.pengpengdd.cyou/gtvpxlxcmn.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.sweek.top/gtfnawxuwz.html

[O03] 加锁保护共享数据
来源：http://hz.yuxming.cn/gthatvqjlw.html

Py:   with lock: shared += 1
来源：http://hz.gzhubu.top/gtoszabmyi.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.shanyushiyangkeji.top/gtpowmecpu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.cdnleiting.top/gtvqusptvs.html

TS:   // 同 JS
来源：http://hz.shanyushiyangkeji.top/gthqhfmspn.html

Java: synchronized (this) { shared++; }
来源：http://hz.yonumen.top/gtflssqeip.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.shzxlz.cn/gttheeilzr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.xziqi.cn/gtqnpirtsa.html

C#:   lock (gate) { shared++; }
来源：http://hz.zhixingplan.top/gtehcwrrvk.html

[O04] 定义异步函数并等待
来源：http://hz.hywenlv.cn/gtwaitddtf.html

Py:   async def f():⏎    await g()
来源：http://hz.nwbrower.top/gtdrilwlub.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jinqigufen.top/gtzvjhxjlg.html

JS:   async function f() { await g(); }
来源：http://hz.guowangkeji.top/gtasbufodt.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.jianghu66.top/gtsalmqsfm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.hnxiangtu.top/gtaeffhfcf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.yongpay.top/gttglpsprg.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.zhengqikj.top/gtbtevvqqu.html

C#:   async Task F() { await G(); }
来源：http://hz.wangdashe.top/gtjbtrxegv.html

[O05] 并发执行并等待全部完成
来源：http://hz.birdmap.top/gtxvpmvhml.html

Py:   asyncio.gather(*tasks)
来源：http://hz.cqqwz.cn/gthuktauxo.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.hnxiangtu.top/gtiskyyqkh.html

JS:   await Promise.all(tasks)
来源：http://hz.wangshuangyany.cn/gtjdahgxlc.html

TS:   await Promise.all(tasks)
来源：http://hz.feifeiyinyue.top/gtswhwdtaz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.chenjidiqi.icu/gtqsgqbqsr.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yj202588.top/gtdiyihgry.html

Ruby: threads.map(&:join)
来源：http://hz.kuanghao11.cn/gtdcmzvuav.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.daxiang520.top/gtaozifefw.html

[O06] 使用进程池
来源：http://hz.shanyushiyangkeji.top/gtqqeoxvrs.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.yj20258.top/gtwvzsbovx.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.ydjk.org.cn/gtbkxlqnhs.html

JS:   // child_process / cluster 模块
来源：http://hz.gaohongyu789.top/gtugkvbkyc.html

TS:   // child_process / cluster 模块
来源：http://hz.zhengqikj.top/gtgpbdqazn.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.zhengqikj.top/gtupgjeytq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.fzhhl.top/gtrbfrblta.html

Ruby: // fork 块
来源：http://hz.yj20258888.top/gtypkczane.html

C#:   Parallel.For
来源：http://hz.hfpthk.cn/gtnapfzjeb.html

================================================================================
来源：http://hz.daria6918.cn/gtqhsdetbn.html

P. 常用工具函数
来源：http://hz.0kj1m.cn/gtyehfhyyl.html

================================================================================
来源：http://hz.svipenyu.cn/gtttblxiib.html

[P01] 生成 UUID
来源：http://hz.svipenyu.cn/gtyewbdjqe.html

Py:   str(uuid.uuid4())
来源：http://hz.jqgufenzy.top/gtwqxhmxqa.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.zhengqikj.top/gtyqoxnrwz.html

JS:   crypto.randomUUID()
来源：http://hz.tianlin.xyz/gtqjxtdjsa.html

TS:   crypto.randomUUID()
来源：http://hz.jiagoushi.top/gtwafrhgwe.html

Java: UUID.randomUUID().toString()
来源：http://hz.havefunace.top/gtlspxjzlv.html

Go:   // 用 github.com/google/uuid
来源：http://hz.c1oappe.top/gtamctgfjs.html

Ruby: SecureRandom.uuid
来源：http://hz.wangdashe.top/gtqzywcucf.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.quarkkingdee.top/gtkmkzotew.html

[P02] MD5 / SHA256 摘要
来源：http://hz.svipenyu.cn/gtujhxlgtu.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.cdnleiting.top/gtavgrivte.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.aizwys.cn/gtuljxvkvr.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.jlsjyb.cn/gtvpvnbspo.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.dianchejie.cn/gtlurcfqpe.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.sweek.top/gtgcbjpitl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.zhaomingkeji.xyz/gtefkxqdcd.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.quarkkingdee.top/gtbjlzgsha.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.9152youxi.cn/gtdrjkbgem.html

[P03] 生成短随机字符串
来源：http://hz.gogol.net.cn/gtmzxomfwg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jinqigfzy.top/gtovepfypa.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.jyoumei.cn/gtulenrneh.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ybcxt.top/gtfsidlpjs.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ydzc1.top/gtuosdohsx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.zhongyouzk.top/gtoiouimtf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.bjfxy.top/gtnraiskmn.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.xuetiantiany.cn/gtxgglgwvp.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.shanyushiyangkeji.top/gtemialqti.html

[P04] 求长度
来源：http://hz.gogol.net.cn/gtjxmoicug.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.birdmap.top/gtcnlxmylb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.52xcode.cn/gtkhegurzd.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hnqzz.top/gtxplzkuin.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.cheryme.top/gtfrgrdolg.html

Java: list.size();  map.size();  s.length()
来源：http://hz.feifeiyinyue.top/gttppyfzhp.html

Go:   len(arr);  len(m)
来源：http://hz.yj20258.top/gtfkhbgifo.html

Ruby: x.length;  x.size
来源：http://hz.jinghuilouyu.cn/gtyrtnrpoo.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.jinqigfzy.top/gtsbnrgboq.html

[P05] 判断两个对象内容是否相等
来源：http://hz.jianghu66.top/gtnscaschh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.yueranfly.top/gtdewddrhe.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.yj202588.top/gtgckkisjh.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.ppjwa.cn/gtyvcgpaqw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.gotoacloud.top/gtwzjqsdkp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.zhongyouzk.top/gtabxlhylc.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.shzxlz.cn/gtkhlzkovd.html

Ruby: a == b
来源：http://hz.0kj1m.cn/gtewarmhzt.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.redwolf501.top/gtkihrdieh.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.jyoumei.cn/gtwcyakqez.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.snrcjt.cn/gtjflcnirr.html

PHP:  if (empty($x)) {}
来源：http://hz.wangdashe.top/gtxhjkbait.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.feifeiyinyue.top/gtxpavldis.html

TS:   if (x == null) {}
来源：http://hz.feifeiyinyue.top/gtfivutsfw.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.ivvv.top/gtwifnbvgl.html

Go:   if x == nil {}
来源：http://hz.jianghu66.top/gtvxbkogkr.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.bjfxy.top/gtcubffnzd.html

C#:   if (x is null) {}
来源：http://hz.52xcode.cn/gtfcpnovnv.html

[P07] 防抖与节流
来源：http://hz.iojbl.cn/gtirnjdbie.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.nanxinkj.top/gtbqvkjccf.html

PHP:  // 手写时间戳比较
来源：http://hz.yangfankeji.com/gtgarecfey.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.fzhhl.top/gtmxqcgrho.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.316326.xyz/gtetwfdrce.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.daxiang520.top/gtoppdwzfu.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.shanyushiyangkeji.top/gtwmjifzav.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.hnqzz.top/gtwlfbgcbm.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.nanxinkj.top/gtloapanqr.html

[P08] 处理浮点精度问题
来源：http://hz.sweek.top/gtyctyiloj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.mhx1999.top/gtjmykvrpw.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.xziqi.cn/gtbcwxzczz.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.bjfxy.top/gtetfmmjyp.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.yuxming.cn/gtaelpiqph.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.hfpthk.cn/gtsctqppor.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.yj20258.top/gtvkvhyddw.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.xingfuxueyuan.xyz/gtmckwvbih.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.chenzaomai.com/gtebtsyhjv.html

================================================================================
来源：http://hz.jinqigufen.top/gtaomxnpfy.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.chenjidiqi.icu/gtvamarhag.html

================================================================================
来源：http://hz.zycfv.cn/gtudvqrgaa.html

[Q01] 创建表
来源：http://hz.mhx1999.top/gtkclgxjba.html

CREATE TABLE users (
来源：http://hz.bjfxy.top/gtejtfaeix.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.cqqwz.cn/gtcpmiziei.html

name VARCHAR(50) NOT NULL,
来源：http://hz.c1oappe.top/gtnuyodxcy.html

email VARCHAR(100) UNIQUE,
来源：http://hz.gaohongyu789.top/gttgcqijhd.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.zhixingplan.top/gtsheqgnxx.html

);
来源：http://hz.yueranfly.top/gtsmsluafw.html

[Q02] 创建带外键的表
来源：http://hz.yj20258.top/gtbpljponh.html

CREATE TABLE orders (
来源：http://hz.ppjwa.cn/gtvvbjilss.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.cheryme.top/gttxyvgupc.html

user_id INT NOT NULL,
来源：http://hz.hywenlv.cn/gtiryrbvde.html

amount DECIMAL(10, 2),
来源：http://hz.aibaodan.cn/gtiwkfppte.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.tianlin.xyz/gtgczljhsm.html

);
来源：http://hz.svipenyu.cn/gtmiihnkdv.html

[Q03] 增加列
来源：http://hz.hongshengwenyu.top/gtvxffbqud.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.chenzaomai.com/gtrnglztvq.html

[Q04] 修改列类型
来源：http://hz.yvedp.cn/gtubaemfuc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.316326.xyz/gthbkdsznn.html

[Q05] 重命名列
来源：http://hz.gotoacloud.top/gtqzthehnn.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.jqgfzy.top/gtdnoigbmz.html

[Q06] 删除列
来源：http://hz.zhijiandao.cn/gtohirwgfv.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.daxiang520.top/gtdhdekghw.html

[Q07] 删除表
来源：http://hz.jlsjyb.cn/gtqxhotmys.html

DROP TABLE IF EXISTS orders;
来源：http://hz.0kj1m.cn/gtxxaptoyk.html

[Q08] 创建普通索引
来源：http://hz.xuanzx.com/gtkllxfcty.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.xuanzx.com/gtmtdnyzlb.html

[Q09] 创建唯一索引
来源：http://hz.chenjidiqi.icu/gtsgndmuks.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.daria6918.cn/gtfmalcgml.html

[Q10] 插入单行
来源：http://hz.xylfe.cn/gtykflmteh.html


<!-- 参考信息 -->