代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yonumen.top/gtvjnalbdb.html

JS:   console.error("err")
来源：http://hz.tianlin.xyz/gtrnzxoxde.html

TS:   console.error("err")
来源：http://hz.0kj1m.cn/gtslvgclbk.html

Java: System.err.println("err")
来源：http://hz.shuidangran.top/gtgjolxcvq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.guowangkeji.top/gtrmabhmbk.html

Ruby: warn "err"
来源：http://hz.zhongyouzk.top/gtbijswzpa.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.gzhubu.top/gtwyfmeieh.html

[M07] 判断是否为主入口
来源：http://hz.fzhhl.top/gtykcpvmff.html

Py:   if __name__ == "__main__":
来源：http://hz.svipenyu.cn/gtehcqqxoa.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yuxming.cn/gtjryzglpk.html

JS:   require.main === module
来源：http://hz.aizwys.cn/gtehmyoebz.html

TS:   require.main === module
来源：http://hz.hnxiangtu.top/gtkcammjpa.html

Java: public static void main(String[] args)
来源：http://hz.yueranfly.top/gttgbaasad.html

Go:   func main()
来源：http://hz.birdmap.top/gtlaxklidm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.svipenyu.cn/gtncwstrov.html

C#:   static void Main(string[] args)
来源：http://hz.mhx1999.top/gtleiwamnn.html

[M08] 获取系统与运行时信息
来源：http://hz.hywenlv.cn/gtxwijjknx.html

Py:   platform.system();  platform.python_version()
来源：http://hz.ydzc1.top/gtjdlacarc.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.xinyue.icu/gtlpdwpuxt.html

JS:   process.platform;  process.version
来源：http://hz.zhongyouzk.top/gtyiteleko.html

TS:   process.platform;  process.version
来源：http://hz.cdnleiting.top/gtyovmufna.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.cdnleiting.top/gtcugwslio.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.zdqjudy.top/gtlhpnzvwd.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.tanke756.top/gtjhpjtmja.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.chenlongwang.top/gtxdhzncna.html

================================================================================
来源：http://hz.tian-w.cn/gtwfavcqtc.html

N. 数据结构与算法
来源：http://hz.ivvv.top/gtpjauevcx.html

================================================================================
来源：http://hz.jqgufenzy.top/gtxsjqixfk.html

[N01] 二分查找（有序数组）
来源：http://hz.feifeiyinyue.top/gtwlmmdreu.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.shanyushiyangkeji.top/gtdgqqhaki.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.sysykeji.top/gtouyjjfcy.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jinqigfzy.top/gtibygeazs.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xuanzx.com/gtjcuvhaip.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.nanxuanxn.top/gtxxclbmdz.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.dianchejie.cn/gtgwdzoltd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.shzxlz.cn/gtbocrfpcr.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.birdmap.top/gtezabfhpv.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.smart0.xyz/gthpqqhfhk.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.mhx1999.top/gtxfxpjknn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.ydzc1.top/gtprgmycim.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhaomingkeji.xyz/gtzqtdnjjv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jyoumei.cn/gttuwcynxd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.jianghu66.top/gtrwbaodyt.html

Go:   slices.Sort(arr)
来源：http://hz.hongshengwenyu.top/gtvnxdrncg.html

Ruby: arr.sort
来源：http://hz.tanke756.top/gteknuingf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.nanxinkj.top/gtkfdegcmw.html

[N03] 快速排序（分治示例）
来源：http://hz.fengsongda.top/gtqkcddfnh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.fzhhl.top/gtizhtbvpr.html

PHP:  // 递归实现，或用 usort
来源：http://hz.yonumen.top/gtvpuawquj.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.guannengcc.top/gtmfmenuhx.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ywan-chungtsiang.top/gtoqpqanon.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jlsjyb.cn/gtcatcnwoa.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.iojbl.cn/gtjpwccwfa.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.zhongyouzk.top/gtvtmhdvjj.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yj20258.top/gtcqxzvlpn.html

[N04] 斐波那契数列
来源：http://hz.316326.xyz/gtxaipdbxi.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yanxiufei.cn/gtedlqxitr.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.9152youxi.cn/gtcnzbpxin.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.guowangkeji.top/gtcxdududa.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jqgufenzy.top/gtlkxykudu.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.ehwqpu.com/gtjnlransd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.zhoulong.xyz/gtykgdughh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.gaohongyu789.top/gtbwjfcsae.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.hnqzz.top/gtejfekgfh.html

[N05] 最大公约数
来源：http://hz.ivvv.top/gtjlvhkxqg.html

Py:   math.gcd(a, b)
来源：http://hz.haohaochexian.top/gtgnilkrcs.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.cucudq.cn/gtupymstvl.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yanxiufei.cn/gtosidchpc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ehwqpu.com/gtzedvtftk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.yuanzhike.top/gtiiwambci.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.feifeiyinyue.top/gtcrccmiwi.html

Ruby: a.gcd(b)
来源：http://hz.sufxvd.cn/gtgslasfmj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.svipenyu.cn/gtmyodazbz.html

[N06] 判断回文字符串
来源：http://hz.guowangkeji.top/gtcowyjvhq.html

Py:   s == s[::-1]
来源：http://hz.feifeiyinyue.top/gtgsstwlpr.html

PHP:  $s === strrev($s);
来源：http://hz.yueranfly.top/gtrxpcrlts.html

JS:   s === [...s].reverse().join("")
来源：http://hz.jinqigufen.top/gtvqyghpyc.html

TS:   s === [...s].reverse().join("")
来源：http://hz.9152youxi.cn/gtyprictye.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.pycfn.com/gtvtdmbihx.html

Go:   // 双指针从两端比较
来源：http://hz.guowangkeji.top/gtvcdqvzze.html

Ruby: s == s.reverse
来源：http://hz.yj202588.top/gtcniyntdj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.cashguo.top/gtwzmoxqui.html

[N07] 两数之和（返回下标）
来源：http://hz.hywenlv.cn/gtjgaqstqg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.pycfn.com/gtiacigbis.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yj20258.top/gtcvnoksgl.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.ppjwa.cn/gtmtqdwlym.html

TS:   // 手写 Map<string, number>
来源：http://hz.zhengqikj.top/gtikhnjbmp.html

Java: // 手写 HashMap
来源：http://hz.pycfn.com/gthxaiicdt.html

Go:   // 手写 map[int]int
来源：http://hz.birdmap.top/gthjffkdib.html

Ruby: // 手写 Hash
来源：http://hz.zhongyouzk.top/gtgpjoihgj.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.zhengqikj.top/gtqczyczym.html

[N08] 生成全排列
来源：http://hz.andypj.xyz/gtzdqyousq.html

Py:   itertools.permutations(arr)
来源：http://hz.bjfxy.top/gtrwcxpxvv.html

PHP:  // 手写递归交换
来源：http://hz.0kj1m.cn/gtzodcxoyc.html

JS:   // 手写回溯递归
来源：http://hz.pycfn.com/gthfhqrceb.html

TS:   // 手写回溯递归
来源：http://hz.shangyingyoupin.top/gtdgcticrx.html

Java: // 手写回溯递归
来源：http://hz.yongpay.top/gtyphlffmf.html

Go:   // 手写回溯递归
来源：http://hz.daria6918.cn/gtgtepenjn.html

Ruby: arr.permutation.to_a
来源：http://hz.cdnleiting.top/gtjkdfixkn.html

C#:   // 手写回溯递归
来源：http://hz.316326.xyz/gtwiqdeprg.html

[N09] 栈与队列
来源：http://hz.redwolf501.top/gtulocjqao.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.c1oappe.top/gtghiomchs.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.zhongyouzk.top/gtspxakugq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.316326.xyz/gtliqoxfpe.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.ehwqpu.com/gtxpouvlrz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.fzhhl.top/gtzhhephko.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.cucudq.cn/gtjuabxisk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.shanyushiyangkeji.top/gtydjhyzle.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.316326.xyz/gttufhvbcp.html

[N10] 链表节点定义
来源：http://hz.yanxiufei.cn/gtkmzivdqe.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.hnxiangtu.top/gttxyyhwri.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.shanyushiyangkeji.top/gtusktmtta.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.jinyuanbaomall.cn/gtdzlmykqp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.cashguo.top/gtzsckmtya.html

Java: class Node { int v; Node next; }
来源：http://hz.vqdsnc.cn/gtvpioppci.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.shanyushiyangkeji.top/gtldsyvghr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.ybcxt.top/gtisskviiy.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.haohaochexian.top/gtsfvrlzfe.html

[N11] 二叉树中序遍历
来源：http://hz.gaohongyu789.top/gtfpqnqcub.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.sweek.top/gttxhhsqwa.html

PHP:  // 手写递归函数
来源：http://hz.hnqzz.top/gtqrxwfiia.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ydzc1.top/gtatggljwv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.birdmap.top/gtizboxmrf.html

Java: // 手写递归
来源：http://hz.meibo888.top/gttqifesls.html

Go:   // 手写递归
来源：http://hz.wangshuangyany.cn/gtggzsazlc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.snrcjt.cn/gtoiryrvmt.html

C#:   // 手写递归
来源：http://hz.sysykeji.top/gtlzkqfhjk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.xziqi.cn/gtjzqmtpmj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.mhx1999.top/gtmsuavuan.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.shangyingyoupin.top/gtcbygvkcr.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xziqi.cn/gthdutbzio.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.meibo888.top/gtczmlkwnc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.meibo888.top/gtzqfeckwd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.jqgfzy.top/gtvodbouen.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.cdnleiting.top/gtkyvrgerr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ywan-chungtsiang.top/gtpawcggkd.html

================================================================================
来源：http://hz.ydjk.org.cn/gtdgdjcapl.html

O. 并发与异步
来源：http://hz.xingfuxueyuan.xyz/gtghquyqbw.html

================================================================================
来源：http://hz.mhx1999.top/gtsxryojnp.html

[O01] 启动一个线程
来源：http://hz.jqgufenzy.top/gtrtlkbzzz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.yueranfly.top/gtvvlaaudi.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.ybcxt.top/gtwbqxoors.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.yuxming.cn/gtvbgorkik.html

TS:   // 同 JS
来源：http://hz.ppjwa.cn/gtzdaqyfpi.html

Java: new Thread(() -> f()).start()
来源：http://hz.chenzaomai.com/gtnaatwhjn.html

Go:   go f()
来源：http://hz.yvedp.cn/gtazjtsetw.html

Ruby: Thread.new { f }
来源：http://hz.guowangkeji.top/gtsuzpzsgv.html

C#:   Task.Run(() => F());
来源：http://hz.shanyushiyangtech.top/gtlzdhculq.html

[O02] 使用线程池
来源：http://hz.birdmap.top/gtrfaqilyz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.sysykeji.top/gtnpvtccpr.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.xuanzx.com/gtqfuzibfs.html

JS:   // worker_threads 线程池
来源：http://hz.jiagoushi.top/gtrmfnevil.html

TS:   // worker_threads 线程池
来源：http://hz.ehwqpu.com/gtamlymehh.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.316326.xyz/gthlstarnt.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.shuidangran.top/gtnzvoliwd.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.gzhubu.top/gtjobonxxv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.svipenyu.cn/gtbuyebrfd.html

[O03] 加锁保护共享数据
来源：http://hz.hysaishi.cn/gtpiqrkncx.html

Py:   with lock: shared += 1
来源：http://hz.c1oappe.top/gtszfehmqu.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.sxryk.cn/gthgokcgpw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.shuidangran.top/gttksyrvhw.html

TS:   // 同 JS
来源：http://hz.yuanzhike.top/gtfupwjotn.html

Java: synchronized (this) { shared++; }
来源：http://hz.zhijiandao.cn/gtdabtixkw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.guannengcc.top/gttngfrmer.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.svipenyu.cn/gtgjgzpvfp.html

C#:   lock (gate) { shared++; }
来源：http://hz.fzhhl.top/gtxctafgml.html

[O04] 定义异步函数并等待
来源：http://hz.chenzaomai.com/gtxmzpolws.html

Py:   async def f():⏎    await g()
来源：http://hz.jqgfzy.top/gtkxlmsqan.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.sysykeji.top/gtylapvmho.html

JS:   async function f() { await g(); }
来源：http://hz.jqgfzy.top/gtyhlzkiki.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.jqgufenzy.top/gtfalqdrqh.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.zhijiandao.cn/gtgbwtjsay.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.chenzaomai.com/gtgbgrzmdn.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.xuetiantiany.cn/gtvdknijpz.html

C#:   async Task F() { await G(); }
来源：http://hz.hongshengwenyu.top/gtrbakobia.html

[O05] 并发执行并等待全部完成
来源：http://hz.quarkkingdee.top/gtvpgszoyk.html

Py:   asyncio.gather(*tasks)
来源：http://hz.hongshengwenyu.top/gtdouvxgmh.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.feifeiyinyue.top/gtehuxcykm.html

JS:   await Promise.all(tasks)
来源：http://hz.xuetiantiany.cn/gtdhqzoxmt.html

TS:   await Promise.all(tasks)
来源：http://hz.gzhubu.top/gtomiiuuqp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.kuanghao11.cn/gtlavfsscq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.cashguo.top/gtknaupkpf.html

Ruby: threads.map(&:join)
来源：http://hz.cucudq.cn/gthjiscysn.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.sufxvd.cn/gtsghmdeax.html

[O06] 使用进程池
来源：http://hz.cucudq.cn/gtchgvjqzr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.mhx1999.top/gtajkuubwe.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.redwolf501.top/gtkxflsizw.html

JS:   // child_process / cluster 模块
来源：http://hz.chenlongwang.top/gteuvtsfxl.html

TS:   // child_process / cluster 模块
来源：http://hz.hfpthk.cn/gtbcwshicn.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.cdnleiting.top/gtdmaxxofu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.dashuyun.cn/gtpyxocblk.html

Ruby: // fork 块
来源：http://hz.ydjk.org.cn/gtbwzfggwo.html

C#:   Parallel.For
来源：http://hz.pengpengdd.cyou/gtiecyacev.html

================================================================================
来源：http://hz.nanxinkj.top/gtldfgjhks.html

P. 常用工具函数
来源：http://hz.vqdsnc.cn/gtrgkbqtrs.html

================================================================================
来源：http://hz.pycfn.com/gtpzbxtbgd.html

[P01] 生成 UUID
来源：http://hz.fengsongda.top/gtcbdoojcq.html

Py:   str(uuid.uuid4())
来源：http://hz.mhx1999.top/gtzwlcnkmu.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.fzhhl.top/gtdcqlryrf.html

JS:   crypto.randomUUID()
来源：http://hz.sxryk.cn/gtobmcfduw.html

TS:   crypto.randomUUID()
来源：http://hz.jqgfzy.top/gtmlthnruw.html

Java: UUID.randomUUID().toString()
来源：http://hz.cheryme.top/gteebargsb.html

Go:   // 用 github.com/google/uuid
来源：http://hz.ppjwa.cn/gtmfoyecon.html

Ruby: SecureRandom.uuid
来源：http://hz.sufxvd.cn/gtqstuqtds.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.0kj1m.cn/gtwuwshwkm.html

[P02] MD5 / SHA256 摘要
来源：http://hz.jianghu66.top/gtuhfnroud.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.gzhubu.top/gtkvfpawrm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.tian-w.cn/gtkeeduona.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.gotoacloud.top/gtdeatyaln.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.meibo888.top/gtrwrltany.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.sysykeji.top/gtmbgdlojq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.yuanzhike.top/gtxvzitfuw.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.zhengqikj.top/gttvhqywtz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.gogol.net.cn/gtixfayxlz.html

[P03] 生成短随机字符串
来源：http://hz.xuetiantiany.cn/gtcyzgjrlb.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.xinyue.icu/gtgfbherzb.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.daria6918.cn/gtkbynpvgt.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.shanyushiyangtech.top/gtaaofycvo.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.9152youxi.cn/gtvtezjrrz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.nanxuanxn.top/gthwcccmbf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.guannengcc.top/gtgyhiodel.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jiagoushi.top/gtxjlvrams.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.hnqzz.top/gtwzugylqc.html

[P04] 求长度
来源：http://hz.jyoumei.cn/gtaiwanvil.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.chenlongwang.top/gtjhyezqqx.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.52xcode.cn/gtgedzqyap.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhengqikj.top/gtcbdauqmg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jqgufenzy.top/gttfjipuyg.html

Java: list.size();  map.size();  s.length()
来源：http://hz.hnqzz.top/gtifzntobw.html

Go:   len(arr);  len(m)
来源：http://hz.yanxiufei.cn/gtiaontdvf.html

Ruby: x.length;  x.size
来源：http://hz.jinghuilouyu.cn/gtotxwulsg.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.hysaishi.cn/gtnddipjnw.html

[P05] 判断两个对象内容是否相等
来源：http://hz.zhongyouzk.top/gtlyqcauch.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.cdnleiting.top/gtognxhbua.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.cqqwz.cn/gtiwrllppw.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.ywan-chungtsiang.top/gtwacmhlas.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.shangyingyoupin.top/gtioxctkws.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.yuanzhike.top/gtwrmoqmos.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.svipenyu.cn/gtekgoyzau.html

Ruby: a == b
来源：http://hz.jinqigfzy.top/gtzksuwvcm.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.kuanghao11.cn/gtzfuxgmvd.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.shanyushiyangtech.top/gthcwqiczv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.tanke756.top/gtedewawux.html

PHP:  if (empty($x)) {}
来源：http://hz.guowangkeji.top/gtrzrgfqlq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.smart0.xyz/gtqgbwyiwf.html

TS:   if (x == null) {}
来源：http://hz.jqgfzy.top/gtkdkfilrj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.gogol.net.cn/gttuwsmsow.html

Go:   if x == nil {}
来源：http://hz.xuetiantiany.cn/gtszeqdugc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.yvedp.cn/gtayzkrouj.html

C#:   if (x is null) {}
来源：http://hz.316326.xyz/gtigljewuc.html

[P07] 防抖与节流
来源：http://hz.chenzaomai.com/gtsygyyolm.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.hfpthk.cn/gtoioxkixq.html

PHP:  // 手写时间戳比较
来源：http://hz.ydjk.org.cn/gtbimsjyrd.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shanyushiyangtech.top/gtzhhydgyi.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yonumen.top/gtbjtxuzpv.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.wangdashe.top/gtzdqesoxa.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.zdqjudy.top/gtgjihxnan.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.hfpthk.cn/gtitktaavj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.iojbl.cn/gtzxxajlln.html

[P08] 处理浮点精度问题
来源：http://hz.ydzc1.top/gtjgzolmqb.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.shuidangran.top/gtxmuvvnmm.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.shangyingyoupin.top/gtlafnvvln.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.pycfn.com/gtwtjldnoy.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.guannengcc.top/gtacdimoux.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.jqgfzy.top/gtozvjxqli.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.xinyue.icu/gtuibjjrpe.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.xingfuxueyuan.xyz/gtcvbanxym.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.fzhhl.top/gtmchkhepa.html

================================================================================
来源：http://hz.snrcjt.cn/gtvkqbfknq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yj20258888.top/gtejvopefc.html

================================================================================
来源：http://hz.hfpthk.cn/gtnezezdzy.html

[Q01] 创建表
来源：http://hz.zhijiandao.cn/gtgcpwinbh.html

CREATE TABLE users (
来源：http://hz.shuidangran.top/gtqhddizav.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.tanke756.top/gtmxhmqrqy.html

name VARCHAR(50) NOT NULL,
来源：http://hz.meibo888.top/gtcjgrqrbo.html

email VARCHAR(100) UNIQUE,
来源：http://hz.yuanzhike.top/gtrjwxgfbh.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.snrcjt.cn/gtrjchmmni.html

);
来源：http://hz.daria6918.cn/gtcszgbufp.html

[Q02] 创建带外键的表
来源：http://hz.gotoacloud.top/gtnrhugznq.html

CREATE TABLE orders (
来源：http://hz.316326.xyz/gtmzsvigea.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yj20258888.top/gtibwmsnyw.html

user_id INT NOT NULL,
来源：http://hz.hnxiangtu.top/gtrjiwfrcd.html

amount DECIMAL(10, 2),
来源：http://hz.guowangkeji.top/gttahlnijt.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.pycfn.com/gtewrpvoce.html

);
来源：http://hz.hfpthk.cn/gtffjrqggr.html

[Q03] 增加列
来源：http://hz.xziqi.cn/gtgksoimqj.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.yj202588.top/gtqivznxlc.html

[Q04] 修改列类型
来源：http://hz.zycfv.cn/gtiqkcvqus.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.dianchejie.cn/gtzfdfwkxn.html

[Q05] 重命名列
来源：http://hz.hammf.cn/gtpcjgthls.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.sysykeji.top/gtckcuzjaw.html

[Q06] 删除列
来源：http://hz.yj202588.top/gtgfrtqczo.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.dianchejie.cn/gtekvoxvky.html

[Q07] 删除表
来源：http://hz.wangdashe.top/gtraeyuryb.html

DROP TABLE IF EXISTS orders;
来源：http://hz.zhaomingkeji.xyz/gtatnqzeqs.html

[Q08] 创建普通索引
来源：http://hz.hammf.cn/gtaxpbygaw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.ydzc1.top/gtpvsvozoy.html

[Q09] 创建唯一索引
来源：http://hz.cdnleiting.top/gtwgcquefy.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.yangfankeji.com/gtwpzgjxgr.html

[Q10] 插入单行
来源：http://hz.nwbrower.top/gteahsxhqq.html


<!-- 参考信息 -->