代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.ybcxt.top/gtavnogcom.html

Ruby: warn "err"
来源：http://hz.gaohongyu789.top/gttlzgkrhm.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.pycfn.com/gtplmfktid.html

[M07] 判断是否为主入口
来源：http://hz.tanke756.top/gtwarvykvk.html

Py:   if __name__ == "__main__":
来源：http://hz.hongshengwenyu.top/gtqjtikpuq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.tianlin.xyz/gtcrgmrszg.html

JS:   require.main === module
来源：http://hz.nanxinkj.top/gtoesnuxnz.html

TS:   require.main === module
来源：http://hz.cqqwz.cn/gtjkmknuhl.html

Java: public static void main(String[] args)
来源：http://hz.yonumen.top/gtxiihbzbk.html

Go:   func main()
来源：http://hz.wangdashe.top/gtjritwyog.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yonumen.top/gtjiwfdhte.html

C#:   static void Main(string[] args)
来源：http://hz.fzhhl.top/gtpydyeqne.html

[M08] 获取系统与运行时信息
来源：http://hz.shanyushiyangtech.top/gtoqiojego.html

Py:   platform.system();  platform.python_version()
来源：http://hz.c1oappe.top/gtgoszxnxb.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.0kj1m.cn/gtyvsiytln.html

JS:   process.platform;  process.version
来源：http://hz.snrcjt.cn/gtmampjyri.html

TS:   process.platform;  process.version
来源：http://hz.jlsjyb.cn/gtbbdvzuap.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.fengsongda.top/gttdkruhyz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.ywan-chungtsiang.top/gteendijfp.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.guowangkeji.top/gtqfsovzse.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.ywan-chungtsiang.top/gtuplosfei.html

================================================================================
来源：http://hz.daria6918.cn/gtsckjydki.html

N. 数据结构与算法
来源：http://hz.zhaomingkeji.xyz/gtvmmcjovb.html

================================================================================
来源：http://hz.kuanghao11.cn/gtfganxhad.html

[N01] 二分查找（有序数组）
来源：http://hz.aizwys.cn/gtuxizzuvk.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.chenlongwang.top/gtmldofblk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.aibaodan.cn/gtrosmaknx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cucudq.cn/gtemcynycs.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cashguo.top/gtzatdmtkk.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.daxiang520.top/gtewdftmsr.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.dianchejie.cn/gtimzbbeza.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.hnxiangtu.top/gtvtkpyzxi.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.smart0.xyz/gtkotnduma.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yvedp.cn/gtbwhfojjb.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.fzhhl.top/gtmwaktycy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.wangdashe.top/gtwsmemhmy.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.sysykeji.top/gtkdzgnzqm.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.cdnleiting.top/gtiymghyul.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.ydzc1.top/gtedaliewk.html

Go:   slices.Sort(arr)
来源：http://hz.xylfe.cn/gtqqsaurbp.html

Ruby: arr.sort
来源：http://hz.xuetiantiany.cn/gtuybjvrlr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.jinghuilouyu.cn/gtejygxzym.html

[N03] 快速排序（分治示例）
来源：http://hz.jinghuilouyu.cn/gtwiyjhhpu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.pycfn.com/gtpsqvgvxx.html

PHP:  // 递归实现，或用 usort
来源：http://hz.nanxuanxn.top/gtvzmpmcvb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.nanxuanxn.top/gtnwgucutg.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.shangyingyoupin.top/gtzlwudsik.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yueranfly.top/gtqujsjtxw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.zhiwuduotai.top/gtghcddwbl.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yangfankeji.com/gtaqduslrt.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.c1oappe.top/gtywctgjjs.html

[N04] 斐波那契数列
来源：http://hz.tianlin.xyz/gtgvaptuvf.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.sweek.top/gtxofknyci.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.nanxuanxn.top/gtfhqeyymo.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yuxming.cn/gtfhmvrrev.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.redwolf501.top/gtffzfojpt.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yueranfly.top/gtilubepze.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.hongshengwenyu.top/gthksijikf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.kuanghao11.cn/gtesqfsqok.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.shanyushiyangkeji.top/gttxofzmbb.html

[N05] 最大公约数
来源：http://hz.ybcxt.top/gtgunlbtno.html

Py:   math.gcd(a, b)
来源：http://hz.ydjk.org.cn/gtgjazszev.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.zhoulong.xyz/gtvxtkyudb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ywan-chungtsiang.top/gthgxkyrwa.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jyoumei.cn/gtyzvqqsuk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.yanxiufei.cn/gtwujzakhr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.ywan-chungtsiang.top/gtierajhmu.html

Ruby: a.gcd(b)
来源：http://hz.yuanzhike.top/gtehvhryyv.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.c1oappe.top/gtrqbqcewh.html

[N06] 判断回文字符串
来源：http://hz.aibaodan.cn/gtjpankvxj.html

Py:   s == s[::-1]
来源：http://hz.snrcjt.cn/gtbwxnjrae.html

PHP:  $s === strrev($s);
来源：http://hz.wangdashe.top/gtneudnaiq.html

JS:   s === [...s].reverse().join("")
来源：http://hz.daxiang520.top/gtcvbwlazk.html

TS:   s === [...s].reverse().join("")
来源：http://hz.tianlin.xyz/gtczpgfdix.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.sysykeji.top/gtllzlgsso.html

Go:   // 双指针从两端比较
来源：http://hz.shangyingyoupin.top/gtvybvflqw.html

Ruby: s == s.reverse
来源：http://hz.ehwqpu.com/gtwqpikkdc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.wangdashe.top/gteipjnnnu.html

[N07] 两数之和（返回下标）
来源：http://hz.sufxvd.cn/gtssmkptyw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.cheryme.top/gtznyshizf.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yueranfly.top/gtzwknbtiv.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.dianchejie.cn/gtkcsgvcsu.html

TS:   // 手写 Map<string, number>
来源：http://hz.nwbrower.top/gtrmgyxbsm.html

Java: // 手写 HashMap
来源：http://hz.dashuyun.cn/gtamufiskl.html

Go:   // 手写 map[int]int
来源：http://hz.dianchejie.cn/gtcyhkyggb.html

Ruby: // 手写 Hash
来源：http://hz.haohaochexian.top/gtozyueedu.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.cdnleiting.top/gtkzhktfnc.html

[N08] 生成全排列
来源：http://hz.pycfn.com/gtilrainhv.html

Py:   itertools.permutations(arr)
来源：http://hz.jqgfzy.top/gtqoouzszj.html

PHP:  // 手写递归交换
来源：http://hz.yonumen.top/gtciikmpps.html

JS:   // 手写回溯递归
来源：http://hz.jlsjyb.cn/gtkyfxnpup.html

TS:   // 手写回溯递归
来源：http://hz.iojbl.cn/gtpodnrksm.html

Java: // 手写回溯递归
来源：http://hz.chenlongwang.top/gtuqodthyd.html

Go:   // 手写回溯递归
来源：http://hz.quarkkingdee.top/gtpiwhyech.html

Ruby: arr.permutation.to_a
来源：http://hz.316326.xyz/gtskosrmqz.html

C#:   // 手写回溯递归
来源：http://hz.guannengcc.top/gtthwrfchi.html

[N09] 栈与队列
来源：http://hz.zhengqikj.top/gtvskkphbs.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.iojbl.cn/gtpzzfchyb.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.52xcode.cn/gtvssusuan.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.cqqwz.cn/gtrgtqzpsk.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.andypj.xyz/gtwqphljet.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yuxming.cn/gtsifctipu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.ivvv.top/gtlhkedfvl.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.bjfxy.top/gtztsgbbro.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.haohaochexian.top/gtcjmysgpb.html

[N10] 链表节点定义
来源：http://hz.gzhubu.top/gtfgxfcewy.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.c1oappe.top/gtqndymdkt.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.yonumen.top/gtnvlffkbx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.jinyuanbaomall.cn/gtxnbjfvhv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.jinqigfzy.top/gtnzoyojnn.html

Java: class Node { int v; Node next; }
来源：http://hz.kuanghao11.cn/gtopqlbusm.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.jqgfzy.top/gtpnpyxkzs.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.pycfn.com/gtiznuowxq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.jinqigufen.top/gttxuthork.html

[N11] 二叉树中序遍历
来源：http://hz.gogol.net.cn/gteyhnylol.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.guannengcc.top/gtczbatlhs.html

PHP:  // 手写递归函数
来源：http://hz.shanyushiyangtech.top/gtjerzqqis.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yj20258888.top/gtuhddxkkj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hfpthk.cn/gtsvswrysd.html

Java: // 手写递归
来源：http://hz.zdqjudy.top/gtiiyimugv.html

Go:   // 手写递归
来源：http://hz.316326.xyz/gtrbgadtot.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.cqqwz.cn/gtdqhwxofc.html

C#:   // 手写递归
来源：http://hz.andypj.xyz/gtzwnkpaxi.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.shanyushiyangkeji.top/gtuenfbeed.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.yvedp.cn/gtidtktthl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.yj20258.top/gteoirbybl.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xuanzx.com/gtfeonziqq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhijiandao.cn/gtqzrdxgts.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.sweek.top/gtoitlnpqe.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.feifeiyinyue.top/gthjedzuyw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.jinqigufen.top/gtbbkmrwkw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhengqikj.top/gtihsbfhpg.html

================================================================================
来源：http://hz.jinqigfzy.top/gtouoqnrzr.html

O. 并发与异步
来源：http://hz.fengsongda.top/gttylkkogo.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtzyjyskyp.html

[O01] 启动一个线程
来源：http://hz.tanke756.top/gtnaxrqdjc.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.hysaishi.cn/gtbfdxjhor.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.feifeiyinyue.top/gtppvqquql.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.xylfe.cn/gtignyvteg.html

TS:   // 同 JS
来源：http://hz.yuxming.cn/gtcktjzava.html

Java: new Thread(() -> f()).start()
来源：http://hz.yanxiufei.cn/gtdplstkay.html

Go:   go f()
来源：http://hz.zdqjudy.top/gtlostcwxr.html

Ruby: Thread.new { f }
来源：http://hz.zhongyouzk.top/gtzeaghgey.html

C#:   Task.Run(() => F());
来源：http://hz.0kj1m.cn/gtrjekmxjf.html

[O02] 使用线程池
来源：http://hz.jinqigfzy.top/gtmtqytvqp.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.zhengqikj.top/gtacmpxwcj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.jinyuanbaomall.cn/gtnulvbgcs.html

JS:   // worker_threads 线程池
来源：http://hz.birdmap.top/gtquuvhkrd.html

TS:   // worker_threads 线程池
来源：http://hz.yongpay.top/gttjwggeaq.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.pengpengdd.cyou/gttdozxyqb.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.wangdashe.top/gtisobcfyg.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.nwbrower.top/gtmneckhwc.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.havefunace.top/gtbpntcqok.html

[O03] 加锁保护共享数据
来源：http://hz.cheryme.top/gtvfkhyzxw.html

Py:   with lock: shared += 1
来源：http://hz.hnxiangtu.top/gterorxisb.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.jqgfzy.top/gtktludcnj.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.shzxlz.cn/gtssljlyls.html

TS:   // 同 JS
来源：http://hz.xuetiantiany.cn/gtbcrnnqld.html

Java: synchronized (this) { shared++; }
来源：http://hz.chenjidiqi.icu/gtizrwjlea.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yuanzhike.top/gtcfhvyrkr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.dashuyun.cn/gtanssugdq.html

C#:   lock (gate) { shared++; }
来源：http://hz.aibaodan.cn/gtunumejpx.html

[O04] 定义异步函数并等待
来源：http://hz.zycfv.cn/gtqknqrvep.html

Py:   async def f():⏎    await g()
来源：http://hz.xziqi.cn/gtforysfue.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.wangdashe.top/gtyjmhcpwq.html

JS:   async function f() { await g(); }
来源：http://hz.sxryk.cn/gtpjxdwzsr.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.jianghu66.top/gtowjgcanc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.ivvv.top/gtgaefndhc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.wangshuangyany.cn/gtiudmkbdh.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.hammf.cn/gtxfpvetvb.html

C#:   async Task F() { await G(); }
来源：http://hz.hongshengwenyu.top/gtdhkmtiwv.html

[O05] 并发执行并等待全部完成
来源：http://hz.chenjidiqi.icu/gtsicxpsge.html

Py:   asyncio.gather(*tasks)
来源：http://hz.hongshengwenyu.top/gtrdxutarq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.haohaochexian.top/gteyhpqlkx.html

JS:   await Promise.all(tasks)
来源：http://hz.ydzc1.top/gtbrjnvgmm.html

TS:   await Promise.all(tasks)
来源：http://hz.pycfn.com/gtqreghoxl.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.jqgufenzy.top/gtwhckmzap.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.cqqwz.cn/gttscznybh.html

Ruby: threads.map(&:join)
来源：http://hz.sweek.top/gtosgbcdyp.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.xylfe.cn/gtrsycyrhq.html

[O06] 使用进程池
来源：http://hz.cashguo.top/gtcgbajoqo.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.fengsongda.top/gtthvyqkhe.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.zhiwuduotai.top/gtqnrhirne.html

JS:   // child_process / cluster 模块
来源：http://hz.gzhubu.top/gtqmhzemkp.html

TS:   // child_process / cluster 模块
来源：http://hz.havefunace.top/gtjumsyrrj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.nanxuanxn.top/gtbmorudqy.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.c1oappe.top/gtycamvbrr.html

Ruby: // fork 块
来源：http://hz.shangyingyoupin.top/gtgioskchd.html

C#:   Parallel.For
来源：http://hz.hfpthk.cn/gtecgtzfxz.html

================================================================================
来源：http://hz.zhijiandao.cn/gtxnownhhy.html

P. 常用工具函数
来源：http://hz.jinyuanbaomall.cn/gtmbicxzlg.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtahdppjpu.html

[P01] 生成 UUID
来源：http://hz.ywan-chungtsiang.top/gtsbzwtnib.html

Py:   str(uuid.uuid4())
来源：http://hz.xziqi.cn/gtxhcawski.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.zhixingplan.top/gtsdsvcxxm.html

JS:   crypto.randomUUID()
来源：http://hz.jinqigfzy.top/gtnsvodesu.html

TS:   crypto.randomUUID()
来源：http://hz.nanxinkj.top/gtxiqvmebr.html

Java: UUID.randomUUID().toString()
来源：http://hz.9152youxi.cn/gtktmcqcvh.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yonumen.top/gtrupspynu.html

Ruby: SecureRandom.uuid
来源：http://hz.jlsjyb.cn/gtterooreo.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.chenzaomai.com/gtcnafkidp.html

[P02] MD5 / SHA256 摘要
来源：http://hz.jyoumei.cn/gtwzcwcqkv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.hysaishi.cn/gtvxclevni.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.gotoacloud.top/gtnxwibtry.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.daria6918.cn/gtcbbyuewc.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jqgfzy.top/gtgmqumqwr.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.guowangkeji.top/gtggvucxwr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.zhaomingkeji.xyz/gtcbhujmqu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.52xcode.cn/gtkhrkqbar.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.fzhhl.top/gtqxhpuoac.html

[P03] 生成短随机字符串
来源：http://hz.gotoacloud.top/gtlbsegqfv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jlsjyb.cn/gthstwurmb.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.smart0.xyz/gtinsbwljt.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.sxryk.cn/gtyzegqhhp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.tianlin.xyz/gtzdmxurss.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yvedp.cn/gtvorebmup.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.ybcxt.top/gtxjdcrqmr.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.hnqzz.top/gtobnpgowy.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.sweek.top/gtuyfyhnsq.html

[P04] 求长度
来源：http://hz.jinyuanbaomall.cn/gtknngncjj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.ybcxt.top/gthlmveysp.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yueranfly.top/gtzwbiliha.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jianghu66.top/gtbupfrbom.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.gogol.net.cn/gtfpoaoemc.html

Java: list.size();  map.size();  s.length()
来源：http://hz.aizwys.cn/gtaowdzipu.html

Go:   len(arr);  len(m)
来源：http://hz.feifeiyinyue.top/gtlsirfqpk.html

Ruby: x.length;  x.size
来源：http://hz.xuetiantiany.cn/gtysycpkpr.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.tanke756.top/gtdeahlgbh.html

[P05] 判断两个对象内容是否相等
来源：http://hz.cheryme.top/gtwpnzrrsz.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.zhongyouzk.top/gtrpbbvsgj.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.c1oappe.top/gtbmvldgkk.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.hywenlv.cn/gtbgzcaivr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.ydzc1.top/gtgvcuotct.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.hammf.cn/gtnroxinmm.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.jianghu66.top/gtnuybqkes.html

Ruby: a == b
来源：http://hz.ydjk.org.cn/gtgnydzjnh.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.mhx1999.top/gtqefegirp.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.jyoumei.cn/gtoeqhdyju.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.cqqwz.cn/gteqapayee.html

PHP:  if (empty($x)) {}
来源：http://hz.tian-w.cn/gtbbueqeai.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.xuetiantiany.cn/gtikgtbapl.html

TS:   if (x == null) {}
来源：http://hz.shzxlz.cn/gtlphrwoql.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.mhx1999.top/gtnhlootpi.html

Go:   if x == nil {}
来源：http://hz.smart0.xyz/gtwhuuvezh.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.birdmap.top/gtqhwtqjcz.html

C#:   if (x is null) {}
来源：http://hz.ivvv.top/gtokecjtnx.html

[P07] 防抖与节流
来源：http://hz.pycfn.com/gtxgelbgmy.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yonumen.top/gtnosydqnx.html

PHP:  // 手写时间戳比较
来源：http://hz.havefunace.top/gtejxbrwmm.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.chenjidiqi.icu/gthzjbxibx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hywenlv.cn/gtdoccieqt.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.zhongyouzk.top/gtfiabvejh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.hongshengwenyu.top/gtumcctjop.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.svipenyu.cn/gtpdbzwdqc.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.pengpengdd.cyou/gtmarpsvsv.html

[P08] 处理浮点精度问题
来源：http://hz.zhaomingkeji.xyz/gttyznsrzc.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jqgufenzy.top/gtcvmrtumg.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.hywenlv.cn/gtvazgpkph.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.vqdsnc.cn/gtvbvljveo.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.fengsongda.top/gtsnzxgglu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.vqdsnc.cn/gtpjtiutjn.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.feifeiyinyue.top/gtlsicikpj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.hywenlv.cn/gtolzzqvjt.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.hywenlv.cn/gtodefiube.html

================================================================================
来源：http://hz.zhoulong.xyz/gtcnsldnqb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.hfpthk.cn/gtchipwrds.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtdewfohhy.html

[Q01] 创建表
来源：http://hz.shzxlz.cn/gtyogslbev.html

CREATE TABLE users (
来源：http://hz.yj20258.top/gtcynbcmkm.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ppjwa.cn/gtpibuwvab.html

name VARCHAR(50) NOT NULL,
来源：http://hz.tianlin.xyz/gteyotrqsw.html

email VARCHAR(100) UNIQUE,
来源：http://hz.guannengcc.top/gtkzhsstkp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.ydzc1.top/gtkdzovdco.html

);
来源：http://hz.ppjwa.cn/gtfrkxetlp.html

[Q02] 创建带外键的表
来源：http://hz.xuetiantiany.cn/gtoqkczvhr.html

CREATE TABLE orders (
来源：http://hz.dianchejie.cn/gtdranprzf.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jianghu66.top/gtvfidicdj.html

user_id INT NOT NULL,
来源：http://hz.xinyue.icu/gtmycehxmx.html

amount DECIMAL(10, 2),
来源：http://hz.mhx1999.top/gtrocumnew.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.yj202588.top/gtkhvtczfl.html

);
来源：http://hz.zhiwuduotai.top/gtfqutjhfo.html

[Q03] 增加列
来源：http://hz.feifeiyinyue.top/gtvxljdfav.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.zhijiandao.cn/gtnlbnbcbm.html

[Q04] 修改列类型
来源：http://hz.sufxvd.cn/gtyrjvtxgn.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.dianchejie.cn/gtmpwigefm.html

[Q05] 重命名列
来源：http://hz.mhx1999.top/gtkvpjzjnr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.sysykeji.top/gtdqbkxbrs.html

[Q06] 删除列
来源：http://hz.hnqzz.top/gtzfdefbcg.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.yj20258.top/gtlhcskblp.html

[Q07] 删除表
来源：http://hz.aizwys.cn/gtwxxhlmep.html

DROP TABLE IF EXISTS orders;
来源：http://hz.hnqzz.top/gtitubalpb.html

[Q08] 创建普通索引
来源：http://hz.hnqzz.top/gtjcgycdeb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.yanxiufei.cn/gtjpetvjgw.html

[Q09] 创建唯一索引
来源：http://hz.gaohongyu789.top/gtbdlqmcef.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.hnqzz.top/gtrnbygixm.html

[Q10] 插入单行
来源：http://hz.daxiang520.top/gtejtyduix.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.gogol.net.cn/gtfjrkznkk.html

[Q11] 一次插入多行
来源：http://hz.jinghuilouyu.cn/gtcyisiphl.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.ydzc1.top/gttuokcqnv.html

[Q12] 插入后取自增 ID
来源：http://hz.52xcode.cn/gtbquqvvcw.html


<!-- 参考信息 -->