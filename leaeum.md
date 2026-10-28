代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.svipenyu.cn/gtnytekkin.html

Ruby: warn "err"
来源：http://hz.52xcode.cn/gtxkwhsfxu.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.jlsjyb.cn/gtlhqdywsu.html

[M07] 判断是否为主入口
来源：http://hz.0kj1m.cn/gtjemsdykg.html

Py:   if __name__ == "__main__":
来源：http://hz.yongpay.top/gtthcjmvrn.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.shanyushiyangtech.top/gtsccpbyjh.html

JS:   require.main === module
来源：http://hz.yongpay.top/gtxcxpvrzg.html

TS:   require.main === module
来源：http://hz.jqgfzy.top/gtcevkkyrs.html

Java: public static void main(String[] args)
来源：http://hz.gzhubu.top/gtvclbfsrq.html

Go:   func main()
来源：http://hz.yonumen.top/gthqhshbgi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jyoumei.cn/gtrqnwaqsz.html

C#:   static void Main(string[] args)
来源：http://hz.nanxuanxn.top/gtsdtsaisq.html

[M08] 获取系统与运行时信息
来源：http://hz.jianghu66.top/gttjdvomsx.html

Py:   platform.system();  platform.python_version()
来源：http://hz.daria6918.cn/gtizyuogcg.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.jyoumei.cn/gtxstdqhkr.html

JS:   process.platform;  process.version
来源：http://hz.sxryk.cn/gtlrbxxshe.html

TS:   process.platform;  process.version
来源：http://hz.nanxinkj.top/gtckfwpakd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.fengsongda.top/gtnzjeclox.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.pengpengdd.cyou/gtdtghmqdq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.dashuyun.cn/gtyvhqmqlm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.hammf.cn/gtivomczte.html

================================================================================
来源：http://hz.hammf.cn/gtrhreeemk.html

N. 数据结构与算法
来源：http://hz.zhongyouzk.top/gtvmbynfje.html

================================================================================
来源：http://hz.zdqjudy.top/gtdqmxvguc.html

[N01] 二分查找（有序数组）
来源：http://hz.nanxuanxn.top/gtrhkzwtdj.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.ppjwa.cn/gtdqbxlswd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.zhongyouzk.top/gtmfrteihb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.shanyushiyangkeji.top/gthdcpfesj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jinghuilouyu.cn/gtsjdbzski.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.birdmap.top/gtviuotnyj.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.kuanghao11.cn/gtibaygqvp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.aizwys.cn/gtgqodrtiu.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.cqqwz.cn/gtldjzlluc.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.cdnleiting.top/gtzmcxxjwl.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yvedp.cn/gtrgqiwbmi.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.fzhhl.top/gtloofqqwq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ydjk.org.cn/gtsfavjtcm.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yongpay.top/gtnfdaatdp.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.0kj1m.cn/gtonxiflsr.html

Go:   slices.Sort(arr)
来源：http://hz.tian-w.cn/gtwukyabgs.html

Ruby: arr.sort
来源：http://hz.svipenyu.cn/gtvthhkvft.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.bjfxy.top/gtyqjdrrzk.html

[N03] 快速排序（分治示例）
来源：http://hz.sweek.top/gtruevkfwp.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.feifeiyinyue.top/gttsbhzmjd.html

PHP:  // 递归实现，或用 usort
来源：http://hz.zhaomingkeji.xyz/gtrakpytke.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jinghuilouyu.cn/gtdbkzslsi.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.nanxinkj.top/gtczuxnujf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yuxming.cn/gthdjzggoy.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jinyuanbaomall.cn/gtlmfbinoj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.jinqigfzy.top/gtidrgbtia.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.xuetiantiany.cn/gtfgfvhncv.html

[N04] 斐波那契数列
来源：http://hz.cashguo.top/gtdceljoki.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.hnqzz.top/gtdaejhclw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.jinqigfzy.top/gtlyasqcvg.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.bjfxy.top/gteydyahjj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.9152youxi.cn/gtloagsgwz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.ppjwa.cn/gtlwmnjeno.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.hnxiangtu.top/gtldvjmzrb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.jianghu66.top/gtkoqanrvf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yonumen.top/gtwjlhvvdz.html

[N05] 最大公约数
来源：http://hz.yueranfly.top/gtjibmcvsk.html

Py:   math.gcd(a, b)
来源：http://hz.zhixingplan.top/gtwqeusecz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.nanxuanxn.top/gtzpsqxbvv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yj202588.top/gtcjpewtxo.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jqgfzy.top/gtbblcprxi.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.dashuyun.cn/gtrnreciwb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.hfpthk.cn/gtqwbzneef.html

Ruby: a.gcd(b)
来源：http://hz.sysykeji.top/gtiimucalj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.nanxinkj.top/gtzsbmadwv.html

[N06] 判断回文字符串
来源：http://hz.pycfn.com/gtssppdtkl.html

Py:   s == s[::-1]
来源：http://hz.cdnleiting.top/gtuskezszl.html

PHP:  $s === strrev($s);
来源：http://hz.xziqi.cn/gtqzbfbcqf.html

JS:   s === [...s].reverse().join("")
来源：http://hz.zhoulong.xyz/gtciziejdy.html

TS:   s === [...s].reverse().join("")
来源：http://hz.jyoumei.cn/gtawjkpzma.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.xingfuxueyuan.xyz/gtjzhaqenx.html

Go:   // 双指针从两端比较
来源：http://hz.guannengcc.top/gtbyzswgyv.html

Ruby: s == s.reverse
来源：http://hz.yj20258888.top/gtypudtcfh.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.hammf.cn/gtkwezjiob.html

[N07] 两数之和（返回下标）
来源：http://hz.yuanzhike.top/gtankenops.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.shangyingyoupin.top/gtyjysltxm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.52xcode.cn/gtvnebtnou.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.yanxiufei.cn/gtygztfvli.html

TS:   // 手写 Map<string, number>
来源：http://hz.yangfankeji.com/gteatteyex.html

Java: // 手写 HashMap
来源：http://hz.xylfe.cn/gtpiseltvf.html

Go:   // 手写 map[int]int
来源：http://hz.bjfxy.top/gtjdtoqtyd.html

Ruby: // 手写 Hash
来源：http://hz.c1oappe.top/gtrbqretrn.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.hnxiangtu.top/gtoqkgllrx.html

[N08] 生成全排列
来源：http://hz.yj202588.top/gtxmocvbum.html

Py:   itertools.permutations(arr)
来源：http://hz.shanyushiyangtech.top/gtzccexjwn.html

PHP:  // 手写递归交换
来源：http://hz.kuanghao11.cn/gtognicvgn.html

JS:   // 手写回溯递归
来源：http://hz.xuetiantiany.cn/gtnzutqmeb.html

TS:   // 手写回溯递归
来源：http://hz.jqgfzy.top/gtdoksigde.html

Java: // 手写回溯递归
来源：http://hz.xuetiantiany.cn/gtrucddrkf.html

Go:   // 手写回溯递归
来源：http://hz.9152youxi.cn/gtmrzmuxzm.html

Ruby: arr.permutation.to_a
来源：http://hz.vqdsnc.cn/gtvnlsupek.html

C#:   // 手写回溯递归
来源：http://hz.ehwqpu.com/gtkrikqitu.html

[N09] 栈与队列
来源：http://hz.zdqjudy.top/gtphteqdny.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.hongshengwenyu.top/gtoermrlrr.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.ydzc1.top/gtuljaprcm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zhongyouzk.top/gtqzqjtrbi.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.hammf.cn/gtvlxyvgvr.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.chenlongwang.top/gtafvpjjvq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.daxiang520.top/gtelfkqkfm.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.316326.xyz/gtiwtrpaws.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.zhijiandao.cn/gtbrxervae.html

[N10] 链表节点定义
来源：http://hz.wangdashe.top/gtpafpvtwe.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yonumen.top/gtsgmwjikq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.sysykeji.top/gtliyapeuy.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.daria6918.cn/gtfkuepnzl.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.zhoulong.xyz/gttmqxpdrk.html

Java: class Node { int v; Node next; }
来源：http://hz.gotoacloud.top/gtqtsiheha.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.hysaishi.cn/gtwahcetje.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.sysykeji.top/gtxptvfymo.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.52xcode.cn/gtoijddumc.html

[N11] 二叉树中序遍历
来源：http://hz.sxryk.cn/gtqvumbtvw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.redwolf501.top/gtsazezgwx.html

PHP:  // 手写递归函数
来源：http://hz.aibaodan.cn/gtpxrqadup.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.xylfe.cn/gtddlkslct.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.cucudq.cn/gtjycwvhhf.html

Java: // 手写递归
来源：http://hz.yueranfly.top/gtpmgshnoy.html

Go:   // 手写递归
来源：http://hz.zhengqikj.top/gtoufpalfv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.vqdsnc.cn/gttdplqfax.html

C#:   // 手写递归
来源：http://hz.pengpengdd.cyou/gtuxcleocp.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.zhixingplan.top/gtftjweztx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.yuxming.cn/gtboryppfv.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.wangdashe.top/gtgdgvzugk.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.svipenyu.cn/gttdondcmr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.svipenyu.cn/gthjskemkw.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.cashguo.top/gtwvrgxqot.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.shanyushiyangtech.top/gtjnbijpsi.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.sufxvd.cn/gtjeysoqay.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ehwqpu.com/gtriivijko.html

================================================================================
来源：http://hz.jlsjyb.cn/gtntkjesnj.html

O. 并发与异步
来源：http://hz.zhongyouzk.top/gtnyoohuwk.html

================================================================================
来源：http://hz.yj20258.top/gtmmyyjgdz.html

[O01] 启动一个线程
来源：http://hz.ppjwa.cn/gtuszeelwf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.bjfxy.top/gtyusrvdqy.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.nanxinkj.top/gtrhfodgqf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.jqgfzy.top/gtsgmttdmw.html

TS:   // 同 JS
来源：http://hz.cdnleiting.top/gtazbxcdzs.html

Java: new Thread(() -> f()).start()
来源：http://hz.birdmap.top/gtfxkfnzlq.html

Go:   go f()
来源：http://hz.xuetiantiany.cn/gthxvijrbv.html

Ruby: Thread.new { f }
来源：http://hz.yvedp.cn/gtstrvcrzi.html

C#:   Task.Run(() => F());
来源：http://hz.tian-w.cn/gtheqwlzzr.html

[O02] 使用线程池
来源：http://hz.jiagoushi.top/gthdrcbida.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.haohaochexian.top/gtkcmggoda.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.aizwys.cn/gtawxcczxi.html

JS:   // worker_threads 线程池
来源：http://hz.hywenlv.cn/gtvmfnkhdi.html

TS:   // worker_threads 线程池
来源：http://hz.snrcjt.cn/gtbfowwsos.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.daxiang520.top/gtadcabsib.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.tianlin.xyz/gttjipqriv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.nwbrower.top/gtkabsupcg.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.xingfuxueyuan.xyz/gtcokpxuuu.html

[O03] 加锁保护共享数据
来源：http://hz.pycfn.com/gtxzkwmvld.html

Py:   with lock: shared += 1
来源：http://hz.yuanzhike.top/gtmahjdwzg.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.havefunace.top/gtlpbuoohp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.jianghu66.top/gtsgramvsy.html

TS:   // 同 JS
来源：http://hz.yj20258888.top/gtvochrfkx.html

Java: synchronized (this) { shared++; }
来源：http://hz.snrcjt.cn/gtouxdnmqj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.kuanghao11.cn/gtizsvuzfq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jyoumei.cn/gtoxzipwtk.html

C#:   lock (gate) { shared++; }
来源：http://hz.zhoulong.xyz/gtbcvjpgpb.html

[O04] 定义异步函数并等待
来源：http://hz.yanxiufei.cn/gtxdvsxlfd.html

Py:   async def f():⏎    await g()
来源：http://hz.meibo888.top/gtpinvaqyo.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.cucudq.cn/gtcqmwvdav.html

JS:   async function f() { await g(); }
来源：http://hz.wangshuangyany.cn/gtgvwkbgdh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.hysaishi.cn/gtadvjghjf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.cucudq.cn/gtkwwebvds.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.316326.xyz/gtbxqmtzol.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.mhx1999.top/gtnulzhzda.html

C#:   async Task F() { await G(); }
来源：http://hz.hongshengwenyu.top/gtuvzblfdi.html

[O05] 并发执行并等待全部完成
来源：http://hz.vqdsnc.cn/gtquabndjl.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jinqigfzy.top/gtddhpfjwg.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.9152youxi.cn/gtgjawzurw.html

JS:   await Promise.all(tasks)
来源：http://hz.zhongyouzk.top/gtwubztary.html

TS:   await Promise.all(tasks)
来源：http://hz.daria6918.cn/gtxsymqwhj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.shuidangran.top/gthydgcvvc.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.dashuyun.cn/gtiagonzok.html

Ruby: threads.map(&:join)
来源：http://hz.zhixingplan.top/gtitynucur.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.meibo888.top/gtoytdtujr.html

[O06] 使用进程池
来源：http://hz.kuanghao11.cn/gtseenixmq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.cucudq.cn/gtggzksbgs.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.gogol.net.cn/gtlvelvuqt.html

JS:   // child_process / cluster 模块
来源：http://hz.guowangkeji.top/gtepopmois.html

TS:   // child_process / cluster 模块
来源：http://hz.hnxiangtu.top/gtquespaao.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.pycfn.com/gtwkxpjcvs.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.nwbrower.top/gtsvtwyzac.html

Ruby: // fork 块
来源：http://hz.jinqigufen.top/gtjcmxuvjf.html

C#:   Parallel.For
来源：http://hz.hnxiangtu.top/gtrhvdehhr.html

================================================================================
来源：http://hz.jqgfzy.top/gtdqtckuic.html

P. 常用工具函数
来源：http://hz.hfpthk.cn/gttunjodxu.html

================================================================================
来源：http://hz.sysykeji.top/gtcwkzerhf.html

[P01] 生成 UUID
来源：http://hz.pycfn.com/gtsscistiw.html

Py:   str(uuid.uuid4())
来源：http://hz.cheryme.top/gtuvektrxm.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.zhiwuduotai.top/gtsyvogaqj.html

JS:   crypto.randomUUID()
来源：http://hz.ywan-chungtsiang.top/gtbumltmbd.html

TS:   crypto.randomUUID()
来源：http://hz.birdmap.top/gteuozqped.html

Java: UUID.randomUUID().toString()
来源：http://hz.wangdashe.top/gtbuwgaktv.html

Go:   // 用 github.com/google/uuid
来源：http://hz.jqgufenzy.top/gtbbomrdlz.html

Ruby: SecureRandom.uuid
来源：http://hz.mhx1999.top/gtxhyzjdee.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.jlsjyb.cn/gttjnotsyf.html

[P02] MD5 / SHA256 摘要
来源：http://hz.yangfankeji.com/gtwnqwczlz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.shanyushiyangtech.top/gtglecgcny.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.jinghuilouyu.cn/gtahckpexw.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.mhx1999.top/gtrrgsyujl.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.hywenlv.cn/gtyxkswjlo.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.guowangkeji.top/gtkktssnsy.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.yuxming.cn/gtcgxvmpxo.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.aizwys.cn/gtwnnvkpjo.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.chenlongwang.top/gtdgebtrmq.html

[P03] 生成短随机字符串
来源：http://hz.tanke756.top/gtijhupcem.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.yongpay.top/gtbxxalgym.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.xylfe.cn/gtalerfgrq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jinqigfzy.top/gthzwudurp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.pycfn.com/gtmxezcgeq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.chenzaomai.com/gtfcbrqwkl.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yuxming.cn/gtmpqvthtx.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jlsjyb.cn/gteuokjjsd.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.hywenlv.cn/gtrslhtowv.html

[P04] 求长度
来源：http://hz.bjfxy.top/gtqsgulzhj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.shanyushiyangkeji.top/gtitsdqkii.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.cucudq.cn/gtxngtzrmw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.svipenyu.cn/gtmobiffji.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.dianchejie.cn/gtecdppqgg.html

Java: list.size();  map.size();  s.length()
来源：http://hz.yj20258.top/gtrfrwbgsm.html

Go:   len(arr);  len(m)
来源：http://hz.yanxiufei.cn/gtrtddqvle.html

Ruby: x.length;  x.size
来源：http://hz.guowangkeji.top/gtjfcjyfgk.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.cqqwz.cn/gterraezjf.html

[P05] 判断两个对象内容是否相等
来源：http://hz.havefunace.top/gtbicotwvy.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.chenjidiqi.icu/gtisszcfrf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.zhaomingkeji.xyz/gtqdebpqsf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.smart0.xyz/gtuwivsglg.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.andypj.xyz/gtkygsprhp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.wangshuangyany.cn/gtvihnlttc.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.zdqjudy.top/gtsgboqean.html

Ruby: a == b
来源：http://hz.quarkkingdee.top/gtxqhjmozs.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.jyoumei.cn/gtcgrerobr.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.jyoumei.cn/gtbqiezicv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.jlsjyb.cn/gttuxtjbdl.html

PHP:  if (empty($x)) {}
来源：http://hz.ybcxt.top/gtnsxhtqyu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.bjfxy.top/gtcamfiiag.html

TS:   if (x == null) {}
来源：http://hz.jiagoushi.top/gthltjxxor.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.zhaomingkeji.xyz/gthbefjive.html

Go:   if x == nil {}
来源：http://hz.wangshuangyany.cn/gtnfythdtw.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.zhoulong.xyz/gtxipjtuuh.html

C#:   if (x is null) {}
来源：http://hz.zhaomingkeji.xyz/gtjufwdazd.html

[P07] 防抖与节流
来源：http://hz.jianghu66.top/gthysyoenu.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.aibaodan.cn/gthfgmvfda.html

PHP:  // 手写时间戳比较
来源：http://hz.yuxming.cn/gtwkqgfuyd.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hnqzz.top/gttywgowmt.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yj20258888.top/gtlqkixzwz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.hongshengwenyu.top/gtoxasmzpt.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.zhaomingkeji.xyz/gtydxxwicr.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.daxiang520.top/gtdtgctrvz.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.jinqigfzy.top/gtjdbknbds.html

[P08] 处理浮点精度问题
来源：http://hz.yuanzhike.top/gtqmsmdnjc.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jinqigufen.top/gtgrfxxpzb.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.ppjwa.cn/gtekqfhbnr.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.meibo888.top/gtpopleofi.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.kuanghao11.cn/gtbgzemxsv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.gotoacloud.top/gtfoxugqzc.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.zhijiandao.cn/gttmkmlcrb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.yuanzhike.top/gtdhecuhqr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.svipenyu.cn/gtrycvnrpy.html

================================================================================
来源：http://hz.dianchejie.cn/gtfhofgwie.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.shangyingyoupin.top/gtdddrthfu.html

================================================================================
来源：http://hz.quarkkingdee.top/gtenabmaof.html

[Q01] 创建表
来源：http://hz.dashuyun.cn/gtqkomqkme.html

CREATE TABLE users (
来源：http://hz.tanke756.top/gtffhnesnd.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.daria6918.cn/gtlyzpyxwk.html

name VARCHAR(50) NOT NULL,
来源：http://hz.fzhhl.top/gtxjjhugjt.html

email VARCHAR(100) UNIQUE,
来源：http://hz.316326.xyz/gtlwqozmma.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.ppjwa.cn/gtcmnmjaqw.html

);
来源：http://hz.ydzc1.top/gtsxzqzvtj.html

[Q02] 创建带外键的表
来源：http://hz.316326.xyz/gtioasoewu.html

CREATE TABLE orders (
来源：http://hz.zhiwuduotai.top/gtfwpemxqz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.cucudq.cn/gtprkcwgqd.html

user_id INT NOT NULL,
来源：http://hz.yueranfly.top/gttgrqbttq.html

amount DECIMAL(10, 2),
来源：http://hz.xylfe.cn/gtqsrbtzbw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.nanxinkj.top/gtykxxepco.html

);
来源：http://hz.ehwqpu.com/gtehqncyqw.html

[Q03] 增加列
来源：http://hz.xuetiantiany.cn/gtxjcgrgus.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.zhijiandao.cn/gtgoepffis.html

[Q04] 修改列类型
来源：http://hz.ybcxt.top/gtxrdskroy.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.yuxming.cn/gtescequet.html

[Q05] 重命名列
来源：http://hz.c1oappe.top/gtgumfogxj.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.bjfxy.top/gtvuxikwub.html

[Q06] 删除列
来源：http://hz.hnxiangtu.top/gtpydimyfo.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.redwolf501.top/gtjhkubzwx.html

[Q07] 删除表
来源：http://hz.nwbrower.top/gtsuugsyih.html

DROP TABLE IF EXISTS orders;
来源：http://hz.meibo888.top/gtcmflmjrh.html

[Q08] 创建普通索引
来源：http://hz.jyoumei.cn/gtgdvorblw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.c1oappe.top/gtzburiqmq.html

[Q09] 创建唯一索引
来源：http://hz.jyoumei.cn/gtuuzwnhtx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.redwolf501.top/gtnhvfabda.html

[Q10] 插入单行
来源：http://hz.chenzaomai.com/gtniobitqi.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.tian-w.cn/gtemvxokdn.html

[Q11] 一次插入多行
来源：http://hz.cheryme.top/gtudvukezz.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.xuetiantiany.cn/gtxzkhsgkr.html

[Q12] 插入后取自增 ID
来源：http://hz.ywan-chungtsiang.top/gtgyfmpfqp.html


<!-- 参考信息 -->