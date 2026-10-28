代发 wailian999

TS:   process.platform;  process.version
来源：http://hz.nanxuanxn.top/gtrejkbcji.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.feifeiyinyue.top/gtrjeydyss.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jiagoushi.top/gtwjguhxha.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.mhx1999.top/gtbtnnalmu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.jyoumei.cn/gtcanejvaw.html

================================================================================
来源：http://hz.xylfe.cn/gtxatncnfl.html

N. 数据结构与算法
来源：http://hz.gogol.net.cn/gtmnganpzq.html

================================================================================
来源：http://hz.hfpthk.cn/gtchczwefp.html

[N01] 二分查找（有序数组）
来源：http://hz.ywan-chungtsiang.top/gtayowvqwj.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.xylfe.cn/gtsjyiplll.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.haohaochexian.top/gtgkgwsbqq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.316326.xyz/gtvdgxcatd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.aizwys.cn/gtiapapubi.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.dianchejie.cn/gtgqcorrui.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.ivvv.top/gtgqntestr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.ydjk.org.cn/gtdopybtje.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.zhengqikj.top/gtswypfhdg.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.pycfn.com/gtbinnqjjs.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xingfuxueyuan.xyz/gtqjfkdjft.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.aibaodan.cn/gtcxkrwojy.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yanxiufei.cn/gtruomkiqn.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hnxiangtu.top/gtzgouoqor.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.kuanghao11.cn/gtzuwugbiy.html

Go:   slices.Sort(arr)
来源：http://hz.xinyue.icu/gtqqgdprpy.html

Ruby: arr.sort
来源：http://hz.nanxuanxn.top/gtakevqepv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.yueranfly.top/gtyvxahynt.html

[N03] 快速排序（分治示例）
来源：http://hz.daxiang520.top/gtgbxprokc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.guowangkeji.top/gtmxjqixri.html

PHP:  // 递归实现，或用 usort
来源：http://hz.xinyue.icu/gtpttivzee.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.mhx1999.top/gtldgofqkp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jqgufenzy.top/gtqrqcowel.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.shzxlz.cn/gtdszsuvcr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.shanyushiyangkeji.top/gtasfxjmcd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.pengpengdd.cyou/gtbjsbjpbr.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.snrcjt.cn/gtngkkonbh.html

[N04] 斐波那契数列
来源：http://hz.guannengcc.top/gttjrrziam.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yj20258888.top/gtufotwpkl.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.shanyushiyangtech.top/gtxfwwuqtn.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.meibo888.top/gtouugpvfd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ywan-chungtsiang.top/gtybqogrcm.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.shanyushiyangtech.top/gtijbuhkas.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.iojbl.cn/gthdwvgvob.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.nanxinkj.top/gtamzgemng.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.cucudq.cn/gtnyrgzhjs.html

[N05] 最大公约数
来源：http://hz.gaohongyu789.top/gtixvbqmkp.html

Py:   math.gcd(a, b)
来源：http://hz.jiagoushi.top/gtkpgsekjp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.pengpengdd.cyou/gtqemdxoxz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhiwuduotai.top/gthmgomzes.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.cdnleiting.top/gtplugnhmr.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.sysykeji.top/gtgyetnoky.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.jianghu66.top/gtuhkofgld.html

Ruby: a.gcd(b)
来源：http://hz.sxryk.cn/gtgtessoxj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.cheryme.top/gtkkrflmcq.html

[N06] 判断回文字符串
来源：http://hz.tian-w.cn/gtbatzphcn.html

Py:   s == s[::-1]
来源：http://hz.feifeiyinyue.top/gtdmeakkci.html

PHP:  $s === strrev($s);
来源：http://hz.yvedp.cn/gtnznrjmvi.html

JS:   s === [...s].reverse().join("")
来源：http://hz.jiagoushi.top/gtejotqukn.html

TS:   s === [...s].reverse().join("")
来源：http://hz.52xcode.cn/gtetttqlqc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.meibo888.top/gtdnowstnc.html

Go:   // 双指针从两端比较
来源：http://hz.wangdashe.top/gtyoasqdcl.html

Ruby: s == s.reverse
来源：http://hz.pycfn.com/gtjuownhls.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.zhaomingkeji.xyz/gtdnomanfw.html

[N07] 两数之和（返回下标）
来源：http://hz.dianchejie.cn/gtiratjwrk.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.c1oappe.top/gtfionlipg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.hnxiangtu.top/gthokdbloi.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.dashuyun.cn/gtehwzbkbh.html

TS:   // 手写 Map<string, number>
来源：http://hz.pengpengdd.cyou/gtarenbhmw.html

Java: // 手写 HashMap
来源：http://hz.hnqzz.top/gtkprdunkr.html

Go:   // 手写 map[int]int
来源：http://hz.hfpthk.cn/gtedkqbbwm.html

Ruby: // 手写 Hash
来源：http://hz.jiagoushi.top/gtpnwlgojb.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.gzhubu.top/gttqeaqpin.html

[N08] 生成全排列
来源：http://hz.cashguo.top/gtkagajpwb.html

Py:   itertools.permutations(arr)
来源：http://hz.ydzc1.top/gtqdewfzrj.html

PHP:  // 手写递归交换
来源：http://hz.svipenyu.cn/gtqchzgxvp.html

JS:   // 手写回溯递归
来源：http://hz.52xcode.cn/gtbanldhdg.html

TS:   // 手写回溯递归
来源：http://hz.zhixingplan.top/gttsptrleq.html

Java: // 手写回溯递归
来源：http://hz.hammf.cn/gtyptchcph.html

Go:   // 手写回溯递归
来源：http://hz.shuidangran.top/gtlgmqqrnn.html

Ruby: arr.permutation.to_a
来源：http://hz.hnqzz.top/gtdtohjtuz.html

C#:   // 手写回溯递归
来源：http://hz.ydzc1.top/gtjlwllfje.html

[N09] 栈与队列
来源：http://hz.zhongyouzk.top/gtverkkctv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.shanyushiyangtech.top/gtqneenhcu.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.mhx1999.top/gtflviilyb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.jyoumei.cn/gtilpqdewg.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.chenzaomai.com/gtofpggsqx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yvedp.cn/gtybkwfuvs.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.zhixingplan.top/gtsdykcfbh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.cdnleiting.top/gtvkhgylgc.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.cashguo.top/gtsfedosro.html

[N10] 链表节点定义
来源：http://hz.jiagoushi.top/gtbwvjjhju.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.9152youxi.cn/gthpwvehhx.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jinqigfzy.top/gtqphnaxfr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.jyoumei.cn/gttblkjgyh.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.jqgfzy.top/gtggvodzee.html

Java: class Node { int v; Node next; }
来源：http://hz.c1oappe.top/gtlrzflwvs.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.havefunace.top/gtifrsnfij.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.zhongyouzk.top/gtpkfsnwlz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.zhixingplan.top/gtteimeyfw.html

[N11] 二叉树中序遍历
来源：http://hz.guowangkeji.top/gtsatbqbct.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.gotoacloud.top/gtzlpvkkwz.html

PHP:  // 手写递归函数
来源：http://hz.svipenyu.cn/gtrphtudnc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.mhx1999.top/gtciuzbkyg.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ivvv.top/gtpoantnyi.html

Java: // 手写递归
来源：http://hz.ehwqpu.com/gtpnqbekfi.html

Go:   // 手写递归
来源：http://hz.ehwqpu.com/gtsgovkqoy.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.bjfxy.top/gtcxirizqi.html

C#:   // 手写递归
来源：http://hz.tianlin.xyz/gtgjhwlqxt.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.pycfn.com/gtrdownbcc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.cdnleiting.top/gtzdbmyhdc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.hammf.cn/gtjahnkfyq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yvedp.cn/gtihylyfoa.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.kuanghao11.cn/gtxrcsznhy.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.cqqwz.cn/gtskarynir.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.hnxiangtu.top/gtffqvpjxh.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.jinqigfzy.top/gtrnbcyijm.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.wangdashe.top/gtgqxmbode.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtuvktiueu.html

O. 并发与异步
来源：http://hz.316326.xyz/gtrxwvhjle.html

================================================================================
来源：http://hz.cashguo.top/gtqaqmnplk.html

[O01] 启动一个线程
来源：http://hz.c1oappe.top/gthmrfzqwf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.chenlongwang.top/gtdxlwzlos.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.quarkkingdee.top/gtgoeuefuv.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.zhixingplan.top/gtnktvyczi.html

TS:   // 同 JS
来源：http://hz.sufxvd.cn/gtkokvmojg.html

Java: new Thread(() -> f()).start()
来源：http://hz.zhongyouzk.top/gtskfbcxch.html

Go:   go f()
来源：http://hz.guannengcc.top/gtbtkafjpr.html

Ruby: Thread.new { f }
来源：http://hz.ybcxt.top/gtswdwcuau.html

C#:   Task.Run(() => F());
来源：http://hz.ydjk.org.cn/gtxnlltgsg.html

[O02] 使用线程池
来源：http://hz.yuxming.cn/gtcheqnkmy.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.zhongyouzk.top/gtnascpkkm.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.havefunace.top/gtkasexbny.html

JS:   // worker_threads 线程池
来源：http://hz.cdnleiting.top/gtcfjvuxmh.html

TS:   // worker_threads 线程池
来源：http://hz.pycfn.com/gtomswgbuu.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.quarkkingdee.top/gtzrouhzjk.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.iojbl.cn/gtqskptpwu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.svipenyu.cn/gthhclbgah.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.9152youxi.cn/gtixyfjfug.html

[O03] 加锁保护共享数据
来源：http://hz.andypj.xyz/gtseozikfx.html

Py:   with lock: shared += 1
来源：http://hz.zhaomingkeji.xyz/gtgzuzxsyy.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.xingfuxueyuan.xyz/gtwjhmajtv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.jinyuanbaomall.cn/gtforhlpvp.html

TS:   // 同 JS
来源：http://hz.fengsongda.top/gteoznhnga.html

Java: synchronized (this) { shared++; }
来源：http://hz.cqqwz.cn/gtvktnkzso.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.ywan-chungtsiang.top/gtzmusfxjg.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.dashuyun.cn/gttmsdjzyl.html

C#:   lock (gate) { shared++; }
来源：http://hz.xylfe.cn/gtstnovjra.html

[O04] 定义异步函数并等待
来源：http://hz.yuxming.cn/gtnobthkjl.html

Py:   async def f():⏎    await g()
来源：http://hz.hammf.cn/gtukxjtfhq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.yvedp.cn/gtsgsalqza.html

JS:   async function f() { await g(); }
来源：http://hz.zhaomingkeji.xyz/gtmaxtbotw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.jianghu66.top/gtknhirtgu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.bjfxy.top/gtjclpwbpw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.gogol.net.cn/gttrvwvyyz.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.tianlin.xyz/gtiqnfepaz.html

C#:   async Task F() { await G(); }
来源：http://hz.ehwqpu.com/gtmqsuloja.html

[O05] 并发执行并等待全部完成
来源：http://hz.hysaishi.cn/gtzwhtedxn.html

Py:   asyncio.gather(*tasks)
来源：http://hz.chenlongwang.top/gtyngeoolc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.fzhhl.top/gtxofwjped.html

JS:   await Promise.all(tasks)
来源：http://hz.gogol.net.cn/gtqvxevvej.html

TS:   await Promise.all(tasks)
来源：http://hz.xziqi.cn/gtbuzlcdty.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.shanyushiyangkeji.top/gttuhvmrfb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.316326.xyz/gtmhipqscw.html

Ruby: threads.map(&:join)
来源：http://hz.gotoacloud.top/gtnvznjnmf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.jqgufenzy.top/gtybkrhjvw.html

[O06] 使用进程池
来源：http://hz.tian-w.cn/gthqomdrtb.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.jiagoushi.top/gtkhbeyuol.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.pycfn.com/gtrvivjiks.html

JS:   // child_process / cluster 模块
来源：http://hz.guowangkeji.top/gtkafbvfol.html

TS:   // child_process / cluster 模块
来源：http://hz.aibaodan.cn/gtdjzvcdsa.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.sufxvd.cn/gtagcufyfe.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.ehwqpu.com/gtwwhourgt.html

Ruby: // fork 块
来源：http://hz.cashguo.top/gtvkaucrnq.html

C#:   Parallel.For
来源：http://hz.xziqi.cn/gtwyximqws.html

================================================================================
来源：http://hz.zhoulong.xyz/gtahzomchi.html

P. 常用工具函数
来源：http://hz.zhaomingkeji.xyz/gtqbrraweo.html

================================================================================
来源：http://hz.smart0.xyz/gtdjsqnsfm.html

[P01] 生成 UUID
来源：http://hz.chenzaomai.com/gtqpmbenfm.html

Py:   str(uuid.uuid4())
来源：http://hz.yuxming.cn/gtnzbwtqmi.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.kuanghao11.cn/gtopqebova.html

JS:   crypto.randomUUID()
来源：http://hz.shzxlz.cn/gtlamncjhy.html

TS:   crypto.randomUUID()
来源：http://hz.yvedp.cn/gtamtipqos.html

Java: UUID.randomUUID().toString()
来源：http://hz.gzhubu.top/gthzespiug.html

Go:   // 用 github.com/google/uuid
来源：http://hz.svipenyu.cn/gtljxklqyc.html

Ruby: SecureRandom.uuid
来源：http://hz.nwbrower.top/gtxvuhktgs.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.cheryme.top/gtyumivdzw.html

[P02] MD5 / SHA256 摘要
来源：http://hz.zhijiandao.cn/gtzdqzcuvb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.hfpthk.cn/gtcnsrjiyk.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.hongshengwenyu.top/gtrxxpmhkh.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.ydjk.org.cn/gtspwfkrqf.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.zhijiandao.cn/gtgwyscvjy.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.mhx1999.top/gtavuxadmu.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.yonumen.top/gtcyzvaezy.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.hfpthk.cn/gtyhtqnjeg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yuxming.cn/gthazpfrnt.html

[P03] 生成短随机字符串
来源：http://hz.cashguo.top/gtddcafajf.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.yvedp.cn/gtgsegsleg.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.shanyushiyangkeji.top/gtqekrcgcp.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.tanke756.top/gtlwkybboo.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.feifeiyinyue.top/gtfrlcibfd.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jlsjyb.cn/gtxkchfdkj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.jqgufenzy.top/gtapnckxru.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.yangfankeji.com/gtzoobizuo.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.pengpengdd.cyou/gtipdbzney.html

[P04] 求长度
来源：http://hz.jinyuanbaomall.cn/gtkhnlwfxs.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.tanke756.top/gtnhzarzbi.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.wangdashe.top/gtkembuolx.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.daria6918.cn/gtteflkfgq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.chenlongwang.top/gtltqrzthf.html

Java: list.size();  map.size();  s.length()
来源：http://hz.yvedp.cn/gtcmmlwwcl.html

Go:   len(arr);  len(m)
来源：http://hz.sxryk.cn/gtfwzamifx.html

Ruby: x.length;  x.size
来源：http://hz.zhiwuduotai.top/gtzzgerkzf.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.aibaodan.cn/gtltstgtvj.html

[P05] 判断两个对象内容是否相等
来源：http://hz.tianlin.xyz/gtrhzcntas.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.yanxiufei.cn/gtnxpoubmq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.gaohongyu789.top/gtjbeatjpz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.pycfn.com/gtvmimjyka.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.sufxvd.cn/gtdjroqiyz.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jlsjyb.cn/gtmypgvlzf.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yuanzhike.top/gtfekdbyag.html

Ruby: a == b
来源：http://hz.xuetiantiany.cn/gthozzbqaz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.yonumen.top/gtmguittke.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.yanxiufei.cn/gtqlgdwsxm.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.yueranfly.top/gttgiehuwv.html

PHP:  if (empty($x)) {}
来源：http://hz.yuxming.cn/gthycvpoxa.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.shangyingyoupin.top/gtmjefgrwr.html

TS:   if (x == null) {}
来源：http://hz.mhx1999.top/gtepduroak.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.shanyushiyangkeji.top/gtsdnaavhf.html

Go:   if x == nil {}
来源：http://hz.havefunace.top/gtaiketsos.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.cdnleiting.top/gtsyobxuyy.html

C#:   if (x is null) {}
来源：http://hz.hnxiangtu.top/gthxxfjqqt.html

[P07] 防抖与节流
来源：http://hz.nwbrower.top/gtrvxrohtr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.hammf.cn/gtiyecsgjw.html

PHP:  // 手写时间戳比较
来源：http://hz.yueranfly.top/gtokrcbghz.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jinqigufen.top/gtvhsrfmbp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.smart0.xyz/gtlxjlnykr.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.yuxming.cn/gttbadhium.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.yangfankeji.com/gtgqzxnmow.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yonumen.top/gtgldiimuy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.zdqjudy.top/gtehtidwxt.html

[P08] 处理浮点精度问题
来源：http://hz.yuanzhike.top/gtcwxersfk.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.nanxuanxn.top/gtrxyoeeee.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.jinyuanbaomall.cn/gtjnuvbyfc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.tanke756.top/gtoglenohy.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.hnqzz.top/gtynsqtmlk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.shangyingyoupin.top/gtdiuailox.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.iojbl.cn/gttawlowgo.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.zycfv.cn/gtrjenetpb.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.hfpthk.cn/gtbkvagonq.html

================================================================================
来源：http://hz.gaohongyu789.top/gtlmdnhhnh.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.jianghu66.top/gtqoyrpqvq.html

================================================================================
来源：http://hz.guowangkeji.top/gtesjqyxiu.html

[Q01] 创建表
来源：http://hz.cqqwz.cn/gtngaskwgm.html

CREATE TABLE users (
来源：http://hz.hongshengwenyu.top/gtgsevjvmf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yongpay.top/gtarwovjem.html

name VARCHAR(50) NOT NULL,
来源：http://hz.jinqigufen.top/gtegxhijdq.html

email VARCHAR(100) UNIQUE,
来源：http://hz.fzhhl.top/gtjeefbuvw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.jqgufenzy.top/gtkfkcbhpg.html

);
来源：http://hz.jqgufenzy.top/gtbxdogyjp.html

[Q02] 创建带外键的表
来源：http://hz.haohaochexian.top/gtpkxuweae.html

CREATE TABLE orders (
来源：http://hz.tian-w.cn/gtmgvtxadh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.gaohongyu789.top/gtlivbfpqn.html

user_id INT NOT NULL,
来源：http://hz.xuetiantiany.cn/gtdmxotsoa.html

amount DECIMAL(10, 2),
来源：http://hz.cdnleiting.top/gtxosfinmm.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.zhongyouzk.top/gttqobvriz.html

);
来源：http://hz.jyoumei.cn/gtprxglvql.html

[Q03] 增加列
来源：http://hz.zycfv.cn/gtdeluonvl.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.yj20258.top/gtyjiuchxq.html

[Q04] 修改列类型
来源：http://hz.jlsjyb.cn/gtxanydgfm.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.kuanghao11.cn/gtdgcsapyu.html

[Q05] 重命名列
来源：http://hz.yonumen.top/gtgjqzxjfj.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.yueranfly.top/gtoqxloeli.html

[Q06] 删除列
来源：http://hz.zhongyouzk.top/gtpjfquply.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.pengpengdd.cyou/gtxnrkvlip.html

[Q07] 删除表
来源：http://hz.dashuyun.cn/gtnlhxwyct.html

DROP TABLE IF EXISTS orders;
来源：http://hz.zhoulong.xyz/gtzxqurwmf.html

[Q08] 创建普通索引
来源：http://hz.gaohongyu789.top/gtbevciujp.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jinqigfzy.top/gttaenzado.html

[Q09] 创建唯一索引
来源：http://hz.xziqi.cn/gtbjyiwokf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.hammf.cn/gtjfqufzah.html

[Q10] 插入单行
来源：http://hz.tian-w.cn/gtppxccdgv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.shanyushiyangtech.top/gttcolggxl.html

[Q11] 一次插入多行
来源：http://hz.guannengcc.top/gtorzfljag.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.chenlongwang.top/gtgovyfrty.html

[Q12] 插入后取自增 ID
来源：http://hz.hfpthk.cn/gtgxkwodjs.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.gotoacloud.top/gtoevfbrkx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.hnqzz.top/gtreeadzrq.html

[Q13] 忽略重复插入
来源：http://hz.zycfv.cn/gtxtmuequa.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.nwbrower.top/gtuwitsbgd.html

[Q14] 存在则更新（upsert）
来源：http://hz.hammf.cn/gtosnfxdmm.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.fzhhl.top/gtjinnjmhh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.zycfv.cn/gtdvdccmfk.html

[Q15] 查询全部
来源：http://hz.zycfv.cn/gtmekghjwu.html

SELECT * FROM users;
来源：http://hz.zhixingplan.top/gtlygtctgb.html

[Q16] 查询指定列
来源：http://hz.yvedp.cn/gtwhsnbyzs.html

SELECT id, name FROM users;
来源：http://hz.fengsongda.top/gtsgibrvol.html

[Q17] 条件查询
来源：http://hz.tianlin.xyz/gtflgurlol.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.zdqjudy.top/gtirypuopt.html

[Q18] 模糊匹配
来源：http://hz.sweek.top/gtgbqpxfkc.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.c1oappe.top/gtduvwsrfo.html

[Q19] 范围查询
来源：http://hz.jinghuilouyu.cn/gtmwgnfzvs.html


<!-- 参考信息 -->