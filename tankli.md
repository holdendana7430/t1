代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.shanyushiyangkeji.top/gtlwtbbghd.html

Ruby: warn "err"
来源：http://hz.hysaishi.cn/gtqsowgure.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.gaohongyu789.top/gtylcdhnsz.html

[M07] 判断是否为主入口
来源：http://hz.cheryme.top/gtrenocfzc.html

Py:   if __name__ == "__main__":
来源：http://hz.cucudq.cn/gtnemdizet.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yanxiufei.cn/gtfsbfnmjx.html

JS:   require.main === module
来源：http://hz.nanxuanxn.top/gtvetfeyhf.html

TS:   require.main === module
来源：http://hz.52xcode.cn/gthxgyaill.html

Java: public static void main(String[] args)
来源：http://hz.daria6918.cn/gtricvsrnt.html

Go:   func main()
来源：http://hz.guowangkeji.top/gtjxmcgkru.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.shangyingyoupin.top/gttofkhkfd.html

C#:   static void Main(string[] args)
来源：http://hz.fzhhl.top/gthkguvbvh.html

[M08] 获取系统与运行时信息
来源：http://hz.chenjidiqi.icu/gtvtvjfhjj.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yj20258888.top/gtwmqxcibk.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.shuidangran.top/gtijtsjelf.html

JS:   process.platform;  process.version
来源：http://hz.pycfn.com/gtolgfrpxb.html

TS:   process.platform;  process.version
来源：http://hz.yongpay.top/gteishcigp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.ppjwa.cn/gtrcxcbupp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.dashuyun.cn/gtndwjwqsw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.sufxvd.cn/gthgcpkxwn.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yongpay.top/gtohqktxrw.html

================================================================================
来源：http://hz.xinyue.icu/gtqzxylgpa.html

N. 数据结构与算法
来源：http://hz.xylfe.cn/gtdvvqvtcn.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtbcaahsbw.html

[N01] 二分查找（有序数组）
来源：http://hz.yangfankeji.com/gtyionlxbh.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.shuidangran.top/gtpcwoivbu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.hnqzz.top/gtvuecrddf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jianghu66.top/gtjxhnetzy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.0kj1m.cn/gtdirbaofh.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.cdnleiting.top/gtctjdjpru.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jinghuilouyu.cn/gtbgzphvvi.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.xuetiantiany.cn/gtsipgajog.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.birdmap.top/gtomzatdpd.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.hywenlv.cn/gtdvscuvqg.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.chenzaomai.com/gtqybfbzvc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.sufxvd.cn/gtlvzbgmbq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yj20258888.top/gtvbfsdsdf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yanxiufei.cn/gthqordkoe.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.cdnleiting.top/gthblepsin.html

Go:   slices.Sort(arr)
来源：http://hz.yonumen.top/gtwaucbxxw.html

Ruby: arr.sort
来源：http://hz.pengpengdd.cyou/gtuknfqzko.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.yongpay.top/gtdkxwfacu.html

[N03] 快速排序（分治示例）
来源：http://hz.dianchejie.cn/gtncvxpens.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.zhoulong.xyz/gtxhxogpjq.html

PHP:  // 递归实现，或用 usort
来源：http://hz.dashuyun.cn/gtodfqfqcs.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.wangshuangyany.cn/gtrsccjkhl.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.wangshuangyany.cn/gtmvpyfuzc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.cashguo.top/gtvafjvbyu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.316326.xyz/gtbhoyrlxo.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.cdnleiting.top/gteyipivhh.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.gogol.net.cn/gtnwowzlbn.html

[N04] 斐波那契数列
来源：http://hz.zhaomingkeji.xyz/gtrdyskgmg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yj20258.top/gtmquayksn.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.shanyushiyangtech.top/gtrowyceha.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shzxlz.cn/gtnyawfaku.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jinyuanbaomall.cn/gtesrnwvet.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.ppjwa.cn/gtoumfjcfs.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.9152youxi.cn/gtfmmxsuct.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.cucudq.cn/gtujutbofb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.guannengcc.top/gtdpocgmki.html

[N05] 最大公约数
来源：http://hz.zhijiandao.cn/gtwupdsbal.html

Py:   math.gcd(a, b)
来源：http://hz.yueranfly.top/gtnucshtbm.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.gaohongyu789.top/gtlmythnpt.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yangfankeji.com/gtdxdczudb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.cucudq.cn/gtftnelpnq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.jinghuilouyu.cn/gtfygluqio.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.cqqwz.cn/gtnifcukcm.html

Ruby: a.gcd(b)
来源：http://hz.jqgufenzy.top/gtdjwuzfvw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.wangdashe.top/gtitfvkuth.html

[N06] 判断回文字符串
来源：http://hz.jinqigufen.top/gtzpfvfbeg.html

Py:   s == s[::-1]
来源：http://hz.zhoulong.xyz/gtvopphxjv.html

PHP:  $s === strrev($s);
来源：http://hz.9152youxi.cn/gtbuyuscag.html

JS:   s === [...s].reverse().join("")
来源：http://hz.xuetiantiany.cn/gtgtrzqfie.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yuanzhike.top/gtvfnkolmk.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.ywan-chungtsiang.top/gtbxplxswf.html

Go:   // 双指针从两端比较
来源：http://hz.jinyuanbaomall.cn/gtunhidswv.html

Ruby: s == s.reverse
来源：http://hz.fzhhl.top/gtskdhqtyk.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.iojbl.cn/gtfvadqerh.html

[N07] 两数之和（返回下标）
来源：http://hz.nwbrower.top/gtkfvwjavu.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.dashuyun.cn/gtkhxzgolx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.hfpthk.cn/gthdpgkccc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.pengpengdd.cyou/gtaczithwa.html

TS:   // 手写 Map<string, number>
来源：http://hz.jianghu66.top/gtylbcbkqe.html

Java: // 手写 HashMap
来源：http://hz.cashguo.top/gtpoeunxtv.html

Go:   // 手写 map[int]int
来源：http://hz.yangfankeji.com/gtnckxvgnz.html

Ruby: // 手写 Hash
来源：http://hz.hywenlv.cn/gtvnuycono.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.aizwys.cn/gtuuxkupae.html

[N08] 生成全排列
来源：http://hz.hywenlv.cn/gttxgirloo.html

Py:   itertools.permutations(arr)
来源：http://hz.gzhubu.top/gtklrxbyio.html

PHP:  // 手写递归交换
来源：http://hz.xuetiantiany.cn/gturpkgsgn.html

JS:   // 手写回溯递归
来源：http://hz.xylfe.cn/gtzxqzujug.html

TS:   // 手写回溯递归
来源：http://hz.vqdsnc.cn/gtmiwhqdjb.html

Java: // 手写回溯递归
来源：http://hz.shzxlz.cn/gtqlwytyep.html

Go:   // 手写回溯递归
来源：http://hz.xuetiantiany.cn/gtfhrsapnu.html

Ruby: arr.permutation.to_a
来源：http://hz.feifeiyinyue.top/gtmelxfstc.html

C#:   // 手写回溯递归
来源：http://hz.feifeiyinyue.top/gtshfcidcb.html

[N09] 栈与队列
来源：http://hz.jianghu66.top/gtcubvbtkv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.jianghu66.top/gtzlwwkhjk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.c1oappe.top/gtdnxraogg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.sufxvd.cn/gtxikbproq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.hongshengwenyu.top/gtznttquzm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.jyoumei.cn/gtpfakfzcj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.smart0.xyz/gttkndolrd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.meibo888.top/gtagcskesu.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.iojbl.cn/gtqlufragq.html

[N10] 链表节点定义
来源：http://hz.andypj.xyz/gtljaibnlk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.fzhhl.top/gtllxyvuro.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.tianlin.xyz/gtoqauymxt.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.wangdashe.top/gttibacrct.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.yj20258.top/gtbzmhhwwo.html

Java: class Node { int v; Node next; }
来源：http://hz.yj202588.top/gtsrhvqosx.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.xingfuxueyuan.xyz/gtprowkahg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.haohaochexian.top/gtghqqzbwd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.c1oappe.top/gthgzaznkp.html

[N11] 二叉树中序遍历
来源：http://hz.guannengcc.top/gtzrrnxmiz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.wangshuangyany.cn/gtjheimxrq.html

PHP:  // 手写递归函数
来源：http://hz.shzxlz.cn/gtlhcwpcqd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.xuetiantiany.cn/gtraumnbox.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jinghuilouyu.cn/gtuzghlpst.html

Java: // 手写递归
来源：http://hz.jinqigfzy.top/gtokasftov.html

Go:   // 手写递归
来源：http://hz.yonumen.top/gtwmdfoaav.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.zhiwuduotai.top/gthqiwlrhu.html

C#:   // 手写递归
来源：http://hz.jyoumei.cn/gtmvwggbry.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.feifeiyinyue.top/gtxhjqgykb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.xingfuxueyuan.xyz/gtmyogtbhl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.gaohongyu789.top/gtqrndszzt.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jinghuilouyu.cn/gtdkcuypoh.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ybcxt.top/gtblwlgsph.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yuanzhike.top/gtfdtrgcxv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.svipenyu.cn/gtbgqxtgov.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.chenjidiqi.icu/gtvpnpkuto.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.52xcode.cn/gtrwyoqazm.html

================================================================================
来源：http://hz.hammf.cn/gtwdkhmiuj.html

O. 并发与异步
来源：http://hz.svipenyu.cn/gtvpjfcsjw.html

================================================================================
来源：http://hz.sufxvd.cn/gtlvqahmqe.html

[O01] 启动一个线程
来源：http://hz.tian-w.cn/gtvtfojojb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.jinghuilouyu.cn/gtfbfzydbm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yueranfly.top/gtgachtatg.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.daxiang520.top/gtnjtzvtka.html

TS:   // 同 JS
来源：http://hz.haohaochexian.top/gttlqrqcdh.html

Java: new Thread(() -> f()).start()
来源：http://hz.ppjwa.cn/gtegioemon.html

Go:   go f()
来源：http://hz.ydzc1.top/gtvgazkldh.html

Ruby: Thread.new { f }
来源：http://hz.ydjk.org.cn/gtpdioglpq.html

C#:   Task.Run(() => F());
来源：http://hz.havefunace.top/gtbpzzbtbx.html

[O02] 使用线程池
来源：http://hz.dianchejie.cn/gtucbmkufn.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.smart0.xyz/gtikutuvhz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.ydzc1.top/gtxvvzzoiz.html

JS:   // worker_threads 线程池
来源：http://hz.jiagoushi.top/gtsdjcbmwx.html

TS:   // worker_threads 线程池
来源：http://hz.vqdsnc.cn/gttlvhvuzz.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.xinyue.icu/gtwejozykt.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.nanxuanxn.top/gtokhvvges.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.bjfxy.top/gtxbqxikaz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.meibo888.top/gtbdsoijti.html

[O03] 加锁保护共享数据
来源：http://hz.jianghu66.top/gtjvlxedhs.html

Py:   with lock: shared += 1
来源：http://hz.cashguo.top/gtudsjfowl.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.chenjidiqi.icu/gtleaztbcs.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.gzhubu.top/gtebbawfne.html

TS:   // 同 JS
来源：http://hz.daxiang520.top/gthkrgavhc.html

Java: synchronized (this) { shared++; }
来源：http://hz.jinqigfzy.top/gtqcqfbups.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.hnqzz.top/gtpsjzmowi.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.redwolf501.top/gtouyxdljw.html

C#:   lock (gate) { shared++; }
来源：http://hz.meibo888.top/gtsqrzpsom.html

[O04] 定义异步函数并等待
来源：http://hz.tianlin.xyz/gtoejgtmcx.html

Py:   async def f():⏎    await g()
来源：http://hz.xziqi.cn/gtoohzxbuz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jinqigufen.top/gtiubkkpea.html

JS:   async function f() { await g(); }
来源：http://hz.yangfankeji.com/gtcfaopjpu.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.andypj.xyz/gtlrigzueu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.zhoulong.xyz/gtaovopapb.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.zhengqikj.top/gtdkuskhxj.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.sufxvd.cn/gtxkxgzizt.html

C#:   async Task F() { await G(); }
来源：http://hz.andypj.xyz/gtentxurlb.html

[O05] 并发执行并等待全部完成
来源：http://hz.yj20258888.top/gtmxfgmgyd.html

Py:   asyncio.gather(*tasks)
来源：http://hz.shuidangran.top/gtvtbtswce.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.xylfe.cn/gtwsanfnkv.html

JS:   await Promise.all(tasks)
来源：http://hz.zhongyouzk.top/gtfrfbgizf.html

TS:   await Promise.all(tasks)
来源：http://hz.jyoumei.cn/gtmcanctwy.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.gogol.net.cn/gtcadviwzw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.cdnleiting.top/gtaxlzqryv.html

Ruby: threads.map(&:join)
来源：http://hz.cdnleiting.top/gtdgccxjsu.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.haohaochexian.top/gtsuyjmdic.html

[O06] 使用进程池
来源：http://hz.tianlin.xyz/gtposmvzhf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.tianlin.xyz/gtletzffyv.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.xuetiantiany.cn/gtbkpgmiek.html

JS:   // child_process / cluster 模块
来源：http://hz.gotoacloud.top/gtqacyicby.html

TS:   // child_process / cluster 模块
来源：http://hz.9152youxi.cn/gtcfkruhne.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.svipenyu.cn/gtmqzfauar.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.gzhubu.top/gteuivlryb.html

Ruby: // fork 块
来源：http://hz.jqgufenzy.top/gtmokyvxwh.html

C#:   Parallel.For
来源：http://hz.daria6918.cn/gtabuzlkmy.html

================================================================================
来源：http://hz.daria6918.cn/gtznwtprzu.html

P. 常用工具函数
来源：http://hz.zhaomingkeji.xyz/gtjsiuuojn.html

================================================================================
来源：http://hz.iojbl.cn/gtbvlmqkvj.html

[P01] 生成 UUID
来源：http://hz.mhx1999.top/gtnijlfywk.html

Py:   str(uuid.uuid4())
来源：http://hz.nanxinkj.top/gtcsyzewhl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.sysykeji.top/gtsdeqyjkp.html

JS:   crypto.randomUUID()
来源：http://hz.cashguo.top/gtbdtkyftn.html

TS:   crypto.randomUUID()
来源：http://hz.zhaomingkeji.xyz/gtqqlcinee.html

Java: UUID.randomUUID().toString()
来源：http://hz.ydjk.org.cn/gtghepzbdk.html

Go:   // 用 github.com/google/uuid
来源：http://hz.aizwys.cn/gtafsvxfal.html

Ruby: SecureRandom.uuid
来源：http://hz.snrcjt.cn/gtrpeqguiv.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.chenjidiqi.icu/gtebbzlzcq.html

[P02] MD5 / SHA256 摘要
来源：http://hz.shangyingyoupin.top/gtjeyzhhjh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.zhongyouzk.top/gtghdsujlq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.tian-w.cn/gtaawkgrsx.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.svipenyu.cn/gtnfqjrlqx.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.meibo888.top/gtexlhubql.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.aibaodan.cn/gtkqnhltpu.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.shuidangran.top/gtjdhlbjwo.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.tanke756.top/gtnoigcazv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.nwbrower.top/gtewgoflzk.html

[P03] 生成短随机字符串
来源：http://hz.yonumen.top/gtfekgkwvq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.fengsongda.top/gtdzwffose.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.cdnleiting.top/gtptebmzqw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhijiandao.cn/gtguslywsi.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.fengsongda.top/gtrgmpsztn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.xziqi.cn/gtlpiibrop.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.zhengqikj.top/gthkpunclj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.gotoacloud.top/gtgahumrtl.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jqgfzy.top/gthmvfamhx.html

[P04] 求长度
来源：http://hz.ybcxt.top/gtcqagbgva.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.kuanghao11.cn/gtkxhdlmta.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.aibaodan.cn/gtvhejukie.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jinyuanbaomall.cn/gtkisksgtt.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yanxiufei.cn/gterlixcnl.html

Java: list.size();  map.size();  s.length()
来源：http://hz.dianchejie.cn/gtpekceyih.html

Go:   len(arr);  len(m)
来源：http://hz.xylfe.cn/gtxusdhhfx.html

Ruby: x.length;  x.size
来源：http://hz.fzhhl.top/gtcqxyehnd.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.guannengcc.top/gtjyjckzjq.html

[P05] 判断两个对象内容是否相等
来源：http://hz.dianchejie.cn/gtluihhshb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.sweek.top/gtxpibebkv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.haohaochexian.top/gtdviyuziy.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.pycfn.com/gttciiegkq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yvedp.cn/gthtavfpgs.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jyoumei.cn/gtjtsqsphy.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.pycfn.com/gtlibxuhxs.html

Ruby: a == b
来源：http://hz.sufxvd.cn/gtufhxlzoi.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.shzxlz.cn/gttfcwqlyr.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.daxiang520.top/gtaugqnenu.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.ydzc1.top/gtkgkzzcrh.html

PHP:  if (empty($x)) {}
来源：http://hz.jinqigufen.top/gttwnsbyjc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.zhoulong.xyz/gtitysixme.html

TS:   if (x == null) {}
来源：http://hz.cucudq.cn/gtogaouirh.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.gotoacloud.top/gtbjzacrko.html

Go:   if x == nil {}
来源：http://hz.feifeiyinyue.top/gtfkeptjhi.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.zhijiandao.cn/gtlqkgvbjr.html

C#:   if (x is null) {}
来源：http://hz.wangshuangyany.cn/gtupdmgmgy.html

[P07] 防抖与节流
来源：http://hz.zhongyouzk.top/gtjkmdsdhi.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.dashuyun.cn/gtyamkihog.html

PHP:  // 手写时间戳比较
来源：http://hz.xziqi.cn/gticpxlexu.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jinyuanbaomall.cn/gtpwgyolde.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.quarkkingdee.top/gthumkzrnt.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.kuanghao11.cn/gtoyjlyppr.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.havefunace.top/gtuytmtqrk.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.ybcxt.top/gtiusirkmu.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.chenlongwang.top/gtjrkfqckd.html

[P08] 处理浮点精度问题
来源：http://hz.jinqigufen.top/gtkovnhlhw.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.birdmap.top/gtzkfgttdc.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.ivvv.top/gtdaqtdbcf.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.nanxuanxn.top/gtxzqwbhod.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.iojbl.cn/gtekkjjjsw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.pengpengdd.cyou/gtkafgsmda.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.cheryme.top/gtacyfpdst.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.guowangkeji.top/gtzoqkqyuu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.c1oappe.top/gtnweyuzmo.html

================================================================================
来源：http://hz.shzxlz.cn/gtqahrecik.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.redwolf501.top/gtlktzlewk.html

================================================================================
来源：http://hz.birdmap.top/gtbsbrqjng.html

[Q01] 创建表
来源：http://hz.jqgfzy.top/gtgzevcqez.html

CREATE TABLE users (
来源：http://hz.cashguo.top/gttxinzdaa.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ybcxt.top/gtwavoofqs.html

name VARCHAR(50) NOT NULL,
来源：http://hz.zhongyouzk.top/gtiazrzrgx.html

email VARCHAR(100) UNIQUE,
来源：http://hz.gotoacloud.top/gtpdpklzhc.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.chenjidiqi.icu/gtzevixegc.html

);
来源：http://hz.ywan-chungtsiang.top/gtujskjilg.html

[Q02] 创建带外键的表
来源：http://hz.yongpay.top/gtpgxutddi.html

CREATE TABLE orders (
来源：http://hz.sweek.top/gthsbnngwl.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.snrcjt.cn/gtudlkwipa.html

user_id INT NOT NULL,
来源：http://hz.yuxming.cn/gtyxzpmhzl.html

amount DECIMAL(10, 2),
来源：http://hz.316326.xyz/gtixneqgbw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.snrcjt.cn/gtnvuyefib.html

);
来源：http://hz.nwbrower.top/gthzoeumqs.html

[Q03] 增加列
来源：http://hz.sweek.top/gtihflrkeo.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.svipenyu.cn/gtilqtyrwl.html

[Q04] 修改列类型
来源：http://hz.andypj.xyz/gtpwncblqa.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.cheryme.top/gtuwnlzapa.html

[Q05] 重命名列
来源：http://hz.wangshuangyany.cn/gtpuonnwym.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.c1oappe.top/gtrtahbpoh.html

[Q06] 删除列
来源：http://hz.tanke756.top/gtsabzwuht.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.dashuyun.cn/gtcjejmssm.html

[Q07] 删除表
来源：http://hz.zycfv.cn/gtkhrpgegp.html

DROP TABLE IF EXISTS orders;
来源：http://hz.snrcjt.cn/gtzvldaesv.html

[Q08] 创建普通索引
来源：http://hz.jqgfzy.top/gtshgxcdaq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.cheryme.top/gtnemyhhhd.html

[Q09] 创建唯一索引
来源：http://hz.aibaodan.cn/gtisrtbjof.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.pengpengdd.cyou/gtfarcimct.html

[Q10] 插入单行
来源：http://hz.sxryk.cn/gtyecyonxv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.xingfuxueyuan.xyz/gtjyxxybxr.html

[Q11] 一次插入多行
来源：http://hz.pengpengdd.cyou/gtkrxnjxtg.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.redwolf501.top/gtixafjoru.html

[Q12] 插入后取自增 ID
来源：http://hz.aibaodan.cn/gtxiwmazxd.html


<!-- 参考信息 -->