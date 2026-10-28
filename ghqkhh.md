代发 wailian999

Py:   if __name__ == "__main__":
来源：http://hz.xylfe.cn/gtifxajauy.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.feifeiyinyue.top/gtmppwedzx.html

JS:   require.main === module
来源：http://hz.yvedp.cn/gtrbnvafxa.html

TS:   require.main === module
来源：http://hz.dianchejie.cn/gtrsqijpok.html

Java: public static void main(String[] args)
来源：http://hz.wangdashe.top/gtbnnsudul.html

Go:   func main()
来源：http://hz.dashuyun.cn/gtgkhhhudg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.guannengcc.top/gtoskrgyjy.html

C#:   static void Main(string[] args)
来源：http://hz.pengpengdd.cyou/gtufpwdsac.html

[M08] 获取系统与运行时信息
来源：http://hz.jqgufenzy.top/gtxjvysqrc.html

Py:   platform.system();  platform.python_version()
来源：http://hz.shuidangran.top/gtrxhozttl.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yj20258888.top/gtzbjixngv.html

JS:   process.platform;  process.version
来源：http://hz.jiagoushi.top/gtioewmeun.html

TS:   process.platform;  process.version
来源：http://hz.haohaochexian.top/gtmwpkyijq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.zhoulong.xyz/gtskciqxrg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.c1oappe.top/gtpydlfaan.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.chenlongwang.top/gtbzialpko.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.tian-w.cn/gtlxjheiwp.html

================================================================================
来源：http://hz.vqdsnc.cn/gtwxrejedm.html

N. 数据结构与算法
来源：http://hz.tanke756.top/gtoyilcnmq.html

================================================================================
来源：http://hz.zhoulong.xyz/gtboynszcj.html

[N01] 二分查找（有序数组）
来源：http://hz.pengpengdd.cyou/gtoeynifme.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.9152youxi.cn/gtzxzyalcv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.cucudq.cn/gtqrphbecz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.wangshuangyany.cn/gtygawsnzf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.sxryk.cn/gtoenyfwvp.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.zdqjudy.top/gtitfrugyb.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.quarkkingdee.top/gtnebckvpm.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.mhx1999.top/gtnnogueic.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.hfpthk.cn/gtrqzhxbjo.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.sysykeji.top/gtrcvmaffv.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.daxiang520.top/gtowjllglr.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.hammf.cn/gtmbwdntdw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.9152youxi.cn/gtheuvtdhw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.redwolf501.top/gtypmdgqwt.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.feifeiyinyue.top/gtyqnvqpbm.html

Go:   slices.Sort(arr)
来源：http://hz.chenjidiqi.icu/gtgcuarpnb.html

Ruby: arr.sort
来源：http://hz.0kj1m.cn/gtllvhmdmy.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.gzhubu.top/gtqlpcouje.html

[N03] 快速排序（分治示例）
来源：http://hz.jianghu66.top/gtrlwzcrfn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.gzhubu.top/gtumcypfqo.html

PHP:  // 递归实现，或用 usort
来源：http://hz.hnxiangtu.top/gtfovjdrgd.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hfpthk.cn/gtbvogayhi.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.sweek.top/gtctgyxevc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.gotoacloud.top/gtkpkvwirm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.zhongyouzk.top/gtkzkpxvfz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.jinyuanbaomall.cn/gtnruafkcu.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.redwolf501.top/gtvthasrbh.html

[N04] 斐波那契数列
来源：http://hz.vqdsnc.cn/gtttsztwxk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.c1oappe.top/gtvxygvugu.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.zhijiandao.cn/gtfizgfdsx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hysaishi.cn/gtbtwoecnd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.316326.xyz/gtfsklzxip.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.hammf.cn/gttyjotqrz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.ybcxt.top/gtcsvhndnm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.zhongyouzk.top/gtgqujnfly.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.cashguo.top/gtumbgnnme.html

[N05] 最大公约数
来源：http://hz.guannengcc.top/gtlawubhrl.html

Py:   math.gcd(a, b)
来源：http://hz.ehwqpu.com/gtoidtxrfb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.xingfuxueyuan.xyz/gtrdabrecb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jlsjyb.cn/gtgwahhpwt.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.dashuyun.cn/gtieukqiin.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.jiagoushi.top/gtoipstgbf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.yuxming.cn/gteipjpgnx.html

Ruby: a.gcd(b)
来源：http://hz.ybcxt.top/gtnxwjxarx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.hywenlv.cn/gtzvuhbbmu.html

[N06] 判断回文字符串
来源：http://hz.ybcxt.top/gtknamuayi.html

Py:   s == s[::-1]
来源：http://hz.birdmap.top/gtarpznsca.html

PHP:  $s === strrev($s);
来源：http://hz.shzxlz.cn/gtakvhrtmu.html

JS:   s === [...s].reverse().join("")
来源：http://hz.kuanghao11.cn/gtxohtoajm.html

TS:   s === [...s].reverse().join("")
来源：http://hz.mhx1999.top/gtwlkfbdvi.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.pycfn.com/gtxzuvaibu.html

Go:   // 双指针从两端比较
来源：http://hz.quarkkingdee.top/gtfgzmpuja.html

Ruby: s == s.reverse
来源：http://hz.jinqigfzy.top/gtkchrmoeo.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.shuidangran.top/gtdsaybtqy.html

[N07] 两数之和（返回下标）
来源：http://hz.shangyingyoupin.top/gtcdubpnaf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.redwolf501.top/gtmhupfitc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.jqgfzy.top/gtrlmeokzz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.xziqi.cn/gthaolybeq.html

TS:   // 手写 Map<string, number>
来源：http://hz.316326.xyz/gtpwtrbptx.html

Java: // 手写 HashMap
来源：http://hz.wangdashe.top/gtqjunxhxy.html

Go:   // 手写 map[int]int
来源：http://hz.iojbl.cn/gttzdlfepm.html

Ruby: // 手写 Hash
来源：http://hz.hammf.cn/gtbokbyrci.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.nanxinkj.top/gtjjxfhppn.html

[N08] 生成全排列
来源：http://hz.guannengcc.top/gtdrqxyazf.html

Py:   itertools.permutations(arr)
来源：http://hz.dianchejie.cn/gtrgphgcvx.html

PHP:  // 手写递归交换
来源：http://hz.jiagoushi.top/gtozimfoxn.html

JS:   // 手写回溯递归
来源：http://hz.xuetiantiany.cn/gteudyjjdj.html

TS:   // 手写回溯递归
来源：http://hz.tian-w.cn/gtswifeyuc.html

Java: // 手写回溯递归
来源：http://hz.guowangkeji.top/gtfotrbveu.html

Go:   // 手写回溯递归
来源：http://hz.pengpengdd.cyou/gtyfecpxsc.html

Ruby: arr.permutation.to_a
来源：http://hz.aibaodan.cn/gtxfumyvvv.html

C#:   // 手写回溯递归
来源：http://hz.hysaishi.cn/gtzxsppzyb.html

[N09] 栈与队列
来源：http://hz.316326.xyz/gtjrdjinxa.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.shzxlz.cn/gtgjgnkxbh.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.gzhubu.top/gtkrrxdtte.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.xuanzx.com/gtvordcgwm.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.0kj1m.cn/gtzkyavjhc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.jyoumei.cn/gtvezcgezq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.hywenlv.cn/gtolriycyp.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.wangshuangyany.cn/gtqmxjfdzn.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.zycfv.cn/gtiqgutisd.html

[N10] 链表节点定义
来源：http://hz.9152youxi.cn/gtaeqhbjra.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.daria6918.cn/gtzeaocvgr.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jianghu66.top/gtaohlheif.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.cashguo.top/gtwwrcrszj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.chenzaomai.com/gtfjzpjypm.html

Java: class Node { int v; Node next; }
来源：http://hz.nanxinkj.top/gtnefpvwxc.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.sweek.top/gtlvnkdeud.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.vqdsnc.cn/gtnqmgtwcf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.dashuyun.cn/gtcymcrjuv.html

[N11] 二叉树中序遍历
来源：http://hz.yj20258888.top/gtjkmouuyo.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.shanyushiyangkeji.top/gtgjvbiexd.html

PHP:  // 手写递归函数
来源：http://hz.sweek.top/gtlfxfyeik.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jqgufenzy.top/gtjlzhjzum.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.meibo888.top/gtvhgtlpun.html

Java: // 手写递归
来源：http://hz.zhixingplan.top/gthuwecucr.html

Go:   // 手写递归
来源：http://hz.nwbrower.top/gtlzxeptac.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.haohaochexian.top/gtwyzxbnsz.html

C#:   // 手写递归
来源：http://hz.daria6918.cn/gtnazqegpx.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.jinyuanbaomall.cn/gtdxoqlncz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.c1oappe.top/gtvrmgalcn.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.316326.xyz/gtmphcdshz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.bjfxy.top/gtolvdqwdc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yj20258.top/gtlqgoxely.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yvedp.cn/gtrvvtwcbk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.mhx1999.top/gtfzyekryw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.yj20258888.top/gtbnncgicr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yj20258888.top/gttgdhlxrn.html

================================================================================
来源：http://hz.redwolf501.top/gtzfssiqqa.html

O. 并发与异步
来源：http://hz.xuetiantiany.cn/gtwkcieetv.html

================================================================================
来源：http://hz.yanxiufei.cn/gtzrkllqbs.html

[O01] 启动一个线程
来源：http://hz.andypj.xyz/gttpnawsjs.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.ydzc1.top/gtaqatzwda.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.chenlongwang.top/gtjllfarjq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.cdnleiting.top/gtntytgdly.html

TS:   // 同 JS
来源：http://hz.ydzc1.top/gtvtwgcimn.html

Java: new Thread(() -> f()).start()
来源：http://hz.chenjidiqi.icu/gtzfaoobrn.html

Go:   go f()
来源：http://hz.tanke756.top/gtzuoxzktl.html

Ruby: Thread.new { f }
来源：http://hz.hywenlv.cn/gtbzjxkexo.html

C#:   Task.Run(() => F());
来源：http://hz.hnxiangtu.top/gtrhkiixqk.html

[O02] 使用线程池
来源：http://hz.hnqzz.top/gtwobavkio.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.feifeiyinyue.top/gteuxzozdl.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.shzxlz.cn/gtfgxhhbrx.html

JS:   // worker_threads 线程池
来源：http://hz.mhx1999.top/gtydjncrmg.html

TS:   // worker_threads 线程池
来源：http://hz.xuetiantiany.cn/gtkfylcgsy.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.hysaishi.cn/gteukuajfu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.cheryme.top/gtptfmnsjc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.hfpthk.cn/gtbsnpvdsk.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.jiagoushi.top/gtrbcmljua.html

[O03] 加锁保护共享数据
来源：http://hz.snrcjt.cn/gtnjfnifky.html

Py:   with lock: shared += 1
来源：http://hz.sufxvd.cn/gtllfzmpzf.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.hammf.cn/gtktejpuut.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.hysaishi.cn/gteephbudu.html

TS:   // 同 JS
来源：http://hz.xuanzx.com/gtmkvghshv.html

Java: synchronized (this) { shared++; }
来源：http://hz.zhijiandao.cn/gtubquvldn.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.hammf.cn/gtfnzzftwz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.daxiang520.top/gtxkrpqadh.html

C#:   lock (gate) { shared++; }
来源：http://hz.birdmap.top/gtmagibmog.html

[O04] 定义异步函数并等待
来源：http://hz.yj202588.top/gtamlszwam.html

Py:   async def f():⏎    await g()
来源：http://hz.daria6918.cn/gtsfodkazf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.sxryk.cn/gtdfovnapa.html

JS:   async function f() { await g(); }
来源：http://hz.xziqi.cn/gtdqkbbgyp.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.svipenyu.cn/gtuyeothnv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.gaohongyu789.top/gtjltpczuq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.vqdsnc.cn/gtjpoxlvfh.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.ydzc1.top/gtdowgcald.html

C#:   async Task F() { await G(); }
来源：http://hz.tian-w.cn/gtivcdueju.html

[O05] 并发执行并等待全部完成
来源：http://hz.aibaodan.cn/gtodnghurr.html

Py:   asyncio.gather(*tasks)
来源：http://hz.c1oappe.top/gtogolwrbs.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.tanke756.top/gtfmfivzgv.html

JS:   await Promise.all(tasks)
来源：http://hz.snrcjt.cn/gtqmkicjdn.html

TS:   await Promise.all(tasks)
来源：http://hz.redwolf501.top/gtrkwlxaza.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.xuanzx.com/gtuxdyzrvs.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.hnqzz.top/gteofugpbz.html

Ruby: threads.map(&:join)
来源：http://hz.hywenlv.cn/gtmvedokzl.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.nanxinkj.top/gtigrwdgto.html

[O06] 使用进程池
来源：http://hz.snrcjt.cn/gtxjxsdooz.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.hongshengwenyu.top/gtyfgltlym.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.cheryme.top/gtobkfdmjo.html

JS:   // child_process / cluster 模块
来源：http://hz.chenjidiqi.icu/gtliicfzrb.html

TS:   // child_process / cluster 模块
来源：http://hz.gotoacloud.top/gtojealqrn.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jinghuilouyu.cn/gtbhgnnwpy.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.gzhubu.top/gtgvktnquo.html

Ruby: // fork 块
来源：http://hz.tian-w.cn/gtjaodtsfw.html

C#:   Parallel.For
来源：http://hz.havefunace.top/gtsqndvlum.html

================================================================================
来源：http://hz.nanxuanxn.top/gtbfudarsg.html

P. 常用工具函数
来源：http://hz.zhoulong.xyz/gtbsjfluig.html

================================================================================
来源：http://hz.yuanzhike.top/gtfjezbcok.html

[P01] 生成 UUID
来源：http://hz.zhaomingkeji.xyz/gttdgqmnmc.html

Py:   str(uuid.uuid4())
来源：http://hz.xylfe.cn/gttoetyybf.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.feifeiyinyue.top/gtbgbiidqf.html

JS:   crypto.randomUUID()
来源：http://hz.vqdsnc.cn/gtprwfjhtd.html

TS:   crypto.randomUUID()
来源：http://hz.yvedp.cn/gtrmjgdycf.html

Java: UUID.randomUUID().toString()
来源：http://hz.fzhhl.top/gtybqxkiqq.html

Go:   // 用 github.com/google/uuid
来源：http://hz.snrcjt.cn/gtrhgjxgzc.html

Ruby: SecureRandom.uuid
来源：http://hz.hongshengwenyu.top/gtbfjzchlv.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.shanyushiyangkeji.top/gtonmvavmy.html

[P02] MD5 / SHA256 摘要
来源：http://hz.xylfe.cn/gtlpjnuhts.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.pengpengdd.cyou/gtqwndbrzt.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.hnxiangtu.top/gtfsuemsbe.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yvedp.cn/gtffjjkdib.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.aibaodan.cn/gtqeyrejuw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.redwolf501.top/gtntysmtiq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.hywenlv.cn/gtttvbblsv.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.yonumen.top/gterykrijl.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.sufxvd.cn/gtljwczorc.html

[P03] 生成短随机字符串
来源：http://hz.bjfxy.top/gtektdfmwq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.shanyushiyangtech.top/gtdguvbsac.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.nanxinkj.top/gtnqsnlcoz.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jlsjyb.cn/gtzhwgqsjb.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.gotoacloud.top/gtghmrnleh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.redwolf501.top/gtafipehfs.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.mhx1999.top/gtgbgbsxuf.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.birdmap.top/gtbgbkykhe.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.zhijiandao.cn/gtiuyakniz.html

[P04] 求长度
来源：http://hz.hnqzz.top/gtgnrjksnv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.andypj.xyz/gtoinblsie.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.c1oappe.top/gtyjclnfrv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.daxiang520.top/gttkienpvv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hongshengwenyu.top/gtntzkyucu.html

Java: list.size();  map.size();  s.length()
来源：http://hz.zhixingplan.top/gtzgplofmf.html

Go:   len(arr);  len(m)
来源：http://hz.kuanghao11.cn/gtxraahbfe.html

Ruby: x.length;  x.size
来源：http://hz.yongpay.top/gtvelrurdl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.hongshengwenyu.top/gtoizpsrek.html

[P05] 判断两个对象内容是否相等
来源：http://hz.0kj1m.cn/gtgbxbthdo.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.pengpengdd.cyou/gtsownnyxt.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.cqqwz.cn/gtpioipois.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.ivvv.top/gthzqqvliq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zhongyouzk.top/gtghcdgujd.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.xinyue.icu/gtpoatevtu.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.redwolf501.top/gttxpgioou.html

Ruby: a == b
来源：http://hz.svipenyu.cn/gtrrutimhc.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.cdnleiting.top/gtlvpqkrzr.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.gaohongyu789.top/gtiiurgukv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.hongshengwenyu.top/gttzijbeqx.html

PHP:  if (empty($x)) {}
来源：http://hz.tianlin.xyz/gtvsuqjkla.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.xylfe.cn/gtodvexasz.html

TS:   if (x == null) {}
来源：http://hz.yuanzhike.top/gtqbmfbcre.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.sysykeji.top/gtgbqngetv.html

Go:   if x == nil {}
来源：http://hz.sweek.top/gtvtucsppg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.sxryk.cn/gtekivxckv.html

C#:   if (x is null) {}
来源：http://hz.c1oappe.top/gtragsylfh.html

[P07] 防抖与节流
来源：http://hz.hywenlv.cn/gtzyqakuma.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.gotoacloud.top/gtaiwiwzkd.html

PHP:  // 手写时间戳比较
来源：http://hz.zhengqikj.top/gtpoyobcnj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.dashuyun.cn/gtebghafdi.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cashguo.top/gtwjquflmw.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.shangyingyoupin.top/gtatdfqhbt.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.cdnleiting.top/gtrxdbnyrp.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.chenzaomai.com/gtrjsstjnz.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.havefunace.top/gthjunwzpf.html

[P08] 处理浮点精度问题
来源：http://hz.xuetiantiany.cn/gtknbibrfc.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.mhx1999.top/gtvfzddort.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.haohaochexian.top/gtdrqjgosv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.jqgfzy.top/gtqqkbtmpr.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.redwolf501.top/gtjjiihlbf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.quarkkingdee.top/gtandokeaw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.cqqwz.cn/gtbumpdlel.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.xingfuxueyuan.xyz/gtdfrafymn.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.xziqi.cn/gtmnswxqxj.html

================================================================================
来源：http://hz.ydzc1.top/gtzswsxthg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.tanke756.top/gticeaifcd.html

================================================================================
来源：http://hz.dianchejie.cn/gtwrryajhp.html

[Q01] 创建表
来源：http://hz.shanyushiyangtech.top/gtbdjweuez.html

CREATE TABLE users (
来源：http://hz.iojbl.cn/gtflwkwzkg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.gogol.net.cn/gtnnqbgbji.html

name VARCHAR(50) NOT NULL,
来源：http://hz.jqgufenzy.top/gtpuuscgbu.html

email VARCHAR(100) UNIQUE,
来源：http://hz.haohaochexian.top/gtehbgplng.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.jqgfzy.top/gtaknwmart.html

);
来源：http://hz.cheryme.top/gtocfoqtfz.html

[Q02] 创建带外键的表
来源：http://hz.jianghu66.top/gtlcvaikmn.html

CREATE TABLE orders (
来源：http://hz.daria6918.cn/gtqukaoyle.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.sufxvd.cn/gtkhaxnfdr.html

user_id INT NOT NULL,
来源：http://hz.ydzc1.top/gtclqlhdvq.html

amount DECIMAL(10, 2),
来源：http://hz.chenjidiqi.icu/gtzmumsdnz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.sweek.top/gtlqomzyxc.html

);
来源：http://hz.yanxiufei.cn/gtffwwofxw.html

[Q03] 增加列
来源：http://hz.hnqzz.top/gtudogntfz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.fzhhl.top/gtbroffhcd.html

[Q04] 修改列类型
来源：http://hz.pengpengdd.cyou/gttrahmywi.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.zhijiandao.cn/gtlpstqpbx.html

[Q05] 重命名列
来源：http://hz.ydzc1.top/gtpojherwh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.daxiang520.top/gtjwpjhiwi.html

[Q06] 删除列
来源：http://hz.zycfv.cn/gtrddmfboc.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.yueranfly.top/gtegsuvciv.html

[Q07] 删除表
来源：http://hz.xuanzx.com/gtrhloezfb.html

DROP TABLE IF EXISTS orders;
来源：http://hz.birdmap.top/gtejpqdpel.html

[Q08] 创建普通索引
来源：http://hz.jqgufenzy.top/gtfhamrifb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.daxiang520.top/gtnhnvitpz.html

[Q09] 创建唯一索引
来源：http://hz.havefunace.top/gtbeclqmhn.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.hywenlv.cn/gtvdieursz.html

[Q10] 插入单行
来源：http://hz.meibo888.top/gtaejgmykj.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.hnxiangtu.top/gtmojlqgsr.html

[Q11] 一次插入多行
来源：http://hz.jiagoushi.top/gtakogikjz.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.meibo888.top/gtrplgwljv.html

[Q12] 插入后取自增 ID
来源：http://hz.jianghu66.top/gtvpbxgydu.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.nanxinkj.top/gtmppqjxsf.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yongpay.top/gtxuszvvfi.html

[Q13] 忽略重复插入
来源：http://hz.yuanzhike.top/gtdldhszhm.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jinqigfzy.top/gteznyvajr.html


<!-- 参考信息 -->