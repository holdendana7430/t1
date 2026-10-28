代发 wailian999

Java: public static void main(String[] args)
来源：http://hz.dashuyun.cn/gtgljebkgp.html

Go:   func main()
来源：http://hz.yj202588.top/gtcopdizoe.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.bjfxy.top/gthgmsnstg.html

C#:   static void Main(string[] args)
来源：http://hz.ybcxt.top/gtuivhjxdp.html

[M08] 获取系统与运行时信息
来源：http://hz.wangdashe.top/gthesruzpb.html

Py:   platform.system();  platform.python_version()
来源：http://hz.xingfuxueyuan.xyz/gtqbjdzzva.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.jinghuilouyu.cn/gtotbuvhbn.html

JS:   process.platform;  process.version
来源：http://hz.gogol.net.cn/gtldadosvv.html

TS:   process.platform;  process.version
来源：http://hz.shanyushiyangtech.top/gtgyumhcnb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.xinyue.icu/gtnhjgvpes.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.quarkkingdee.top/gtarygltxw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.hongshengwenyu.top/gtazcbkkdu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.gaohongyu789.top/gtvkafobih.html

================================================================================
来源：http://hz.shzxlz.cn/gtxqsrsfpj.html

N. 数据结构与算法
来源：http://hz.fengsongda.top/gtwbauojuc.html

================================================================================
来源：http://hz.daria6918.cn/gtoiyatabv.html

[N01] 二分查找（有序数组）
来源：http://hz.gaohongyu789.top/gtsqrkfwgf.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.fzhhl.top/gtloyrlhem.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.xziqi.cn/gtqziksrud.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.shuidangran.top/gtxsfbeuyt.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.nwbrower.top/gtoqqbkkjn.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.bjfxy.top/gthwqrhals.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.zhixingplan.top/gtjacajrln.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.dianchejie.cn/gttphjmrdt.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.ydjk.org.cn/gtnajvwhbb.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.zhixingplan.top/gtohrbnzxt.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.gzhubu.top/gtwkljbytr.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.cheryme.top/gthrqmwekw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.aizwys.cn/gtytpzbqca.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.aibaodan.cn/gtnyefkcwe.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.jlsjyb.cn/gtoaasprht.html

Go:   slices.Sort(arr)
来源：http://hz.havefunace.top/gtfwliwswy.html

Ruby: arr.sort
来源：http://hz.c1oappe.top/gtokutiwwj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.9152youxi.cn/gtlqydnthe.html

[N03] 快速排序（分治示例）
来源：http://hz.ydzc1.top/gttdfogqvu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.daxiang520.top/gtyfziptdw.html

PHP:  // 递归实现，或用 usort
来源：http://hz.mhx1999.top/gtmpyplamn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.chenjidiqi.icu/gtlsjryuea.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.aizwys.cn/gtnsvnskqv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.tian-w.cn/gtyuqiisnu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.hammf.cn/gtaeifwqtb.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.chenzaomai.com/gtwqiohprd.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zhaomingkeji.xyz/gtzemoxrbf.html

[N04] 斐波那契数列
来源：http://hz.cdnleiting.top/gtuvoqxtnv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.gogol.net.cn/gtyhtoegpz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.pycfn.com/gtwgjcfair.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hnqzz.top/gthktoitwk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xingfuxueyuan.xyz/gtpfsfmegv.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yangfankeji.com/gtbcthsqmq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jinyuanbaomall.cn/gthxbiieee.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.zhongyouzk.top/gtvjdilpez.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.jiagoushi.top/gtavayuamh.html

[N05] 最大公约数
来源：http://hz.cashguo.top/gtbgyfropg.html

Py:   math.gcd(a, b)
来源：http://hz.smart0.xyz/gtnhonnvpb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.0kj1m.cn/gtgkgdjdsx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.shangyingyoupin.top/gtkohwcelq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ivvv.top/gtkweodume.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.jqgufenzy.top/gtfradglyz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.ehwqpu.com/gtanarsyov.html

Ruby: a.gcd(b)
来源：http://hz.zhaomingkeji.xyz/gtevyuxfyc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.zhongyouzk.top/gtwyfpechd.html

[N06] 判断回文字符串
来源：http://hz.tian-w.cn/gtogzmajuy.html

Py:   s == s[::-1]
来源：http://hz.mhx1999.top/gtfqusqina.html

PHP:  $s === strrev($s);
来源：http://hz.ywan-chungtsiang.top/gtlxfckznn.html

JS:   s === [...s].reverse().join("")
来源：http://hz.tian-w.cn/gthlgytgex.html

TS:   s === [...s].reverse().join("")
来源：http://hz.vqdsnc.cn/gtadqaahgy.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.zhiwuduotai.top/gtrdkwsqfp.html

Go:   // 双指针从两端比较
来源：http://hz.sxryk.cn/gtcoctpnje.html

Ruby: s == s.reverse
来源：http://hz.xuanzx.com/gtunwvpxja.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.9152youxi.cn/gtborccqxx.html

[N07] 两数之和（返回下标）
来源：http://hz.yongpay.top/gtidmeavpd.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.zdqjudy.top/gtnabbcknh.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.smart0.xyz/gtywfmueil.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.bjfxy.top/gtcdqpdstz.html

TS:   // 手写 Map<string, number>
来源：http://hz.yanxiufei.cn/gtwpaacfzb.html

Java: // 手写 HashMap
来源：http://hz.0kj1m.cn/gtqakhftya.html

Go:   // 手写 map[int]int
来源：http://hz.dianchejie.cn/gtefgyvjry.html

Ruby: // 手写 Hash
来源：http://hz.yanxiufei.cn/gtasteksav.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.ehwqpu.com/gtalavjxpp.html

[N08] 生成全排列
来源：http://hz.sysykeji.top/gtfdyjknnf.html

Py:   itertools.permutations(arr)
来源：http://hz.zhoulong.xyz/gtoisqkgoc.html

PHP:  // 手写递归交换
来源：http://hz.xylfe.cn/gtduwpumvq.html

JS:   // 手写回溯递归
来源：http://hz.pycfn.com/gtuldpcizp.html

TS:   // 手写回溯递归
来源：http://hz.hfpthk.cn/gtodoskbpk.html

Java: // 手写回溯递归
来源：http://hz.316326.xyz/gtlxwvlhux.html

Go:   // 手写回溯递归
来源：http://hz.ywan-chungtsiang.top/gttgiutaso.html

Ruby: arr.permutation.to_a
来源：http://hz.tanke756.top/gtxrqbyqrt.html

C#:   // 手写回溯递归
来源：http://hz.mhx1999.top/gtqwaeiixu.html

[N09] 栈与队列
来源：http://hz.xinyue.icu/gtdjsmlozi.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.hongshengwenyu.top/gtjkyrvbxk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.hnqzz.top/gthybqjxpn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.tanke756.top/gtmxtucwnc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.dashuyun.cn/gtcwiqpetm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yj20258.top/gtlmwtgabs.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.zhijiandao.cn/gtfjlrihrw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yj20258.top/gtciahguqp.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.zhaomingkeji.xyz/gtuswboacs.html

[N10] 链表节点定义
来源：http://hz.zhoulong.xyz/gtcrikildv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.0kj1m.cn/gtsbgxmxxa.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.xuanzx.com/gtpigdluov.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.ivvv.top/gtvmphvzep.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.ydjk.org.cn/gtokovvzdu.html

Java: class Node { int v; Node next; }
来源：http://hz.zhixingplan.top/gtwzsbavvx.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.sweek.top/gtxlzolhzn.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.sufxvd.cn/gtuxgythkr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.zhongyouzk.top/gtinzjdfhs.html

[N11] 二叉树中序遍历
来源：http://hz.sxryk.cn/gtzhwquvtw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.9152youxi.cn/gtyhndttxf.html

PHP:  // 手写递归函数
来源：http://hz.gzhubu.top/gtxeprozvg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yj20258.top/gtjyululhs.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jlsjyb.cn/gtsdbayusr.html

Java: // 手写递归
来源：http://hz.ybcxt.top/gtvvulzcob.html

Go:   // 手写递归
来源：http://hz.shangyingyoupin.top/gtfbjncmkf.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.shanyushiyangtech.top/gtdbcjoskw.html

C#:   // 手写递归
来源：http://hz.xinyue.icu/gthzxxjnab.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.sweek.top/gtlfyoxghr.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.yuanzhike.top/gtqnfcgsbh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.zhoulong.xyz/gtatlujchx.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.svipenyu.cn/gtbegpdldu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xylfe.cn/gtfwyrqtkn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.chenlongwang.top/gtsyjpxkxg.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.shuidangran.top/gtcaglrimy.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.shuidangran.top/gthkfyjlgt.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.dianchejie.cn/gtuxgxczkz.html

================================================================================
来源：http://hz.sweek.top/gtlbhfmbpd.html

O. 并发与异步
来源：http://hz.yongpay.top/gtqkvvegdb.html

================================================================================
来源：http://hz.bjfxy.top/gtoskveura.html

[O01] 启动一个线程
来源：http://hz.52xcode.cn/gtuzmsrhrr.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.kuanghao11.cn/gtdzitrqnw.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.tian-w.cn/gtabnutkjz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.svipenyu.cn/gtmcrbygsp.html

TS:   // 同 JS
来源：http://hz.zycfv.cn/gtpzxcdlil.html

Java: new Thread(() -> f()).start()
来源：http://hz.hnqzz.top/gtkpidojyu.html

Go:   go f()
来源：http://hz.shanyushiyangkeji.top/gtrgvqqnzi.html

Ruby: Thread.new { f }
来源：http://hz.yj20258.top/gtabvskqya.html

C#:   Task.Run(() => F());
来源：http://hz.hnqzz.top/gtbxfosgas.html

[O02] 使用线程池
来源：http://hz.tian-w.cn/gtxxxgdiqb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.cheryme.top/gtjybvjvrn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.svipenyu.cn/gtpeumvlqu.html

JS:   // worker_threads 线程池
来源：http://hz.birdmap.top/gtinxxftsu.html

TS:   // worker_threads 线程池
来源：http://hz.cashguo.top/gtzcyrvkff.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.hysaishi.cn/gtxmtwkepi.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.chenlongwang.top/gtmhsovsuv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yj20258888.top/gtivjgtahv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.vqdsnc.cn/gtqzcrrxce.html

[O03] 加锁保护共享数据
来源：http://hz.tian-w.cn/gtknvieukz.html

Py:   with lock: shared += 1
来源：http://hz.ybcxt.top/gtviahitnz.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.yanxiufei.cn/gtmuapdqbv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.smart0.xyz/gtohxqemca.html

TS:   // 同 JS
来源：http://hz.316326.xyz/gtjwkribvs.html

Java: synchronized (this) { shared++; }
来源：http://hz.andypj.xyz/gtyszbrisk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.xinyue.icu/gtrrqavtsn.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jqgufenzy.top/gtevbaknfu.html

C#:   lock (gate) { shared++; }
来源：http://hz.yongpay.top/gtbwirdaso.html

[O04] 定义异步函数并等待
来源：http://hz.svipenyu.cn/gtdahshuih.html

Py:   async def f():⏎    await g()
来源：http://hz.svipenyu.cn/gtbxwzefvd.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jinqigufen.top/gtdidojvva.html

JS:   async function f() { await g(); }
来源：http://hz.svipenyu.cn/gtplfkqupg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.redwolf501.top/gtreeuufyh.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.cqqwz.cn/gttpwgoasm.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.wangdashe.top/gtqcgtqubr.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.xylfe.cn/gtgrctzhmq.html

C#:   async Task F() { await G(); }
来源：http://hz.gzhubu.top/gtjtdsydre.html

[O05] 并发执行并等待全部完成
来源：http://hz.haohaochexian.top/gttpxxptgg.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jlsjyb.cn/gtogqtbdqj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.chenlongwang.top/gtexkecwjq.html

JS:   await Promise.all(tasks)
来源：http://hz.tianlin.xyz/gtgmzgrjqv.html

TS:   await Promise.all(tasks)
来源：http://hz.ybcxt.top/gtaustsqxb.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.pycfn.com/gtsccolagx.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.wangdashe.top/gtdgyenmpd.html

Ruby: threads.map(&:join)
来源：http://hz.xuanzx.com/gtfzqqepdi.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.bjfxy.top/gtwhuoiwlj.html

[O06] 使用进程池
来源：http://hz.dashuyun.cn/gtlbkomcwu.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.nanxinkj.top/gtdiksucan.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.cashguo.top/gtewqwwuob.html

JS:   // child_process / cluster 模块
来源：http://hz.tianlin.xyz/gtrooygxgi.html

TS:   // child_process / cluster 模块
来源：http://hz.iojbl.cn/gtfrjxreuo.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.xylfe.cn/gtaozeuifv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.pengpengdd.cyou/gtudnjxigx.html

Ruby: // fork 块
来源：http://hz.svipenyu.cn/gtrwoseheg.html

C#:   Parallel.For
来源：http://hz.hnqzz.top/gtzeswwran.html

================================================================================
来源：http://hz.jiagoushi.top/gtlljjvrjl.html

P. 常用工具函数
来源：http://hz.ydjk.org.cn/gtkxhdvkoe.html

================================================================================
来源：http://hz.guannengcc.top/gtigrewncr.html

[P01] 生成 UUID
来源：http://hz.yonumen.top/gtvjyjjeqf.html

Py:   str(uuid.uuid4())
来源：http://hz.hnxiangtu.top/gtjwbsxagb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.hongshengwenyu.top/gtpspnujbn.html

JS:   crypto.randomUUID()
来源：http://hz.jiagoushi.top/gtcwjbneub.html

TS:   crypto.randomUUID()
来源：http://hz.redwolf501.top/gtnfzurcej.html

Java: UUID.randomUUID().toString()
来源：http://hz.jinqigufen.top/gtnenkqglc.html

Go:   // 用 github.com/google/uuid
来源：http://hz.316326.xyz/gtsidsydre.html

Ruby: SecureRandom.uuid
来源：http://hz.daxiang520.top/gtiqeddtry.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.nanxuanxn.top/gthvkjuggu.html

[P02] MD5 / SHA256 摘要
来源：http://hz.birdmap.top/gtmqupudam.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.vqdsnc.cn/gtvxmwibzz.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.jinqigufen.top/gtlohadsgb.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.wangdashe.top/gtqxenzkwc.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.0kj1m.cn/gtcncpumyk.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.zhiwuduotai.top/gtohlrblki.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.vqdsnc.cn/gthucfuird.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.hfpthk.cn/gtcraxqqjb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.xuanzx.com/gtexyipkch.html

[P03] 生成短随机字符串
来源：http://hz.zdqjudy.top/gtxxvpgthk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.ydzc1.top/gtquontrxp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.tianlin.xyz/gtzdimqmwx.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.feifeiyinyue.top/gtgxumpdwe.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.andypj.xyz/gtrrygzurv.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yvedp.cn/gtfiisdfld.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.hywenlv.cn/gtzeztpcok.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jqgufenzy.top/gtcmzjewwl.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.shzxlz.cn/gtjnxijqsy.html

[P04] 求长度
来源：http://hz.zycfv.cn/gtiqmrpnjt.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.ydjk.org.cn/gtmtrqbzno.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ywan-chungtsiang.top/gtyybselnc.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.quarkkingdee.top/gtzoeunukc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhengqikj.top/gtslhjytgd.html

Java: list.size();  map.size();  s.length()
来源：http://hz.hfpthk.cn/gtgkvuzflg.html

Go:   len(arr);  len(m)
来源：http://hz.ybcxt.top/gtkmszeiyi.html

Ruby: x.length;  x.size
来源：http://hz.yj20258888.top/gtfcnczepn.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.quarkkingdee.top/gtdvlxhgva.html

[P05] 判断两个对象内容是否相等
来源：http://hz.havefunace.top/gtwwhckkyy.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.snrcjt.cn/gtsjqytnzi.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.xingfuxueyuan.xyz/gtxjnwmugk.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.aibaodan.cn/gtmuambrjl.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.cashguo.top/gtibeoupby.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.zhiwuduotai.top/gtgwvynqch.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.cheryme.top/gtmqlczhxi.html

Ruby: a == b
来源：http://hz.yuxming.cn/gtdkpsckvk.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.tianlin.xyz/gtyssfnvkp.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.hongshengwenyu.top/gtuukizfxl.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.xuanzx.com/gttlcrjlwt.html

PHP:  if (empty($x)) {}
来源：http://hz.xuanzx.com/gtorgxyich.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.ivvv.top/gtfylglhtu.html

TS:   if (x == null) {}
来源：http://hz.aibaodan.cn/gtapkzljhu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.jianghu66.top/gtyawrrluy.html

Go:   if x == nil {}
来源：http://hz.shanyushiyangkeji.top/gtnkfbqqna.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.yonumen.top/gtxqxsedrm.html

C#:   if (x is null) {}
来源：http://hz.chenjidiqi.icu/gtiiugphol.html

[P07] 防抖与节流
来源：http://hz.zhengqikj.top/gtmkqjpvgl.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yj20258.top/gtffodeowi.html

PHP:  // 手写时间戳比较
来源：http://hz.shanyushiyangkeji.top/gtsvwgcccy.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cashguo.top/gtwltckenc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.andypj.xyz/gtxlyxijhv.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.wangshuangyany.cn/gtuuigozll.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.jqgfzy.top/gtfhhxflfl.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yongpay.top/gtccibhuah.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.ydjk.org.cn/gtjtavsiob.html

[P08] 处理浮点精度问题
来源：http://hz.ivvv.top/gtheysqpvz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.aibaodan.cn/gtjghomznd.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.ydzc1.top/gtgqjxrfgu.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.guowangkeji.top/gtqbeqrrkl.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.havefunace.top/gtxgcnqdhl.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.pycfn.com/gtuushjlfl.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.yuxming.cn/gtjmyonqrn.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.yangfankeji.com/gtqpfxtgsy.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.wangdashe.top/gtjcyhpala.html

================================================================================
来源：http://hz.yj202588.top/gthhvhitvm.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.quarkkingdee.top/gtfxtjiajk.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtstlxgtjv.html

[Q01] 创建表
来源：http://hz.ywan-chungtsiang.top/gtlrsougmk.html

CREATE TABLE users (
来源：http://hz.c1oappe.top/gtuplwczuj.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.andypj.xyz/gtgrhsupdf.html

name VARCHAR(50) NOT NULL,
来源：http://hz.sufxvd.cn/gtmgyghfpj.html

email VARCHAR(100) UNIQUE,
来源：http://hz.tianlin.xyz/gtsuwspsnu.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.zhiwuduotai.top/gtzppsxoeo.html

);
来源：http://hz.cheryme.top/gtcfffmaxw.html

[Q02] 创建带外键的表
来源：http://hz.yuanzhike.top/gtxfvrudnw.html

CREATE TABLE orders (
来源：http://hz.hongshengwenyu.top/gtpbhrigpo.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yj202588.top/gtqytvgghw.html

user_id INT NOT NULL,
来源：http://hz.chenlongwang.top/gtagcxfouo.html

amount DECIMAL(10, 2),
来源：http://hz.zhongyouzk.top/gtxbjtktjl.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.shangyingyoupin.top/gtuceycnes.html

);
来源：http://hz.c1oappe.top/gtqgiiarym.html

[Q03] 增加列
来源：http://hz.zycfv.cn/gtdkwphmcl.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.cqqwz.cn/gtzempmlci.html

[Q04] 修改列类型
来源：http://hz.xziqi.cn/gtlbhsrmqv.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.chenjidiqi.icu/gtpdtexxux.html

[Q05] 重命名列
来源：http://hz.hfpthk.cn/gtgvqtoufk.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.hywenlv.cn/gtkfdocjwx.html

[Q06] 删除列
来源：http://hz.pycfn.com/gtoqoaacom.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.9152youxi.cn/gtvwqodmwz.html

[Q07] 删除表
来源：http://hz.yj20258.top/gtaglomfyt.html

DROP TABLE IF EXISTS orders;
来源：http://hz.kuanghao11.cn/gtswaihibz.html

[Q08] 创建普通索引
来源：http://hz.zdqjudy.top/gtrmyhqqlu.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.smart0.xyz/gtpujuptjs.html

[Q09] 创建唯一索引
来源：http://hz.jinghuilouyu.cn/gtourvmpjg.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.jqgfzy.top/gtabrcxvvm.html

[Q10] 插入单行
来源：http://hz.ehwqpu.com/gtnzeifesr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jiagoushi.top/gtwlierops.html

[Q11] 一次插入多行
来源：http://hz.bjfxy.top/gtowxkpaau.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.xinyue.icu/gtdvkoptes.html

[Q12] 插入后取自增 ID
来源：http://hz.yueranfly.top/gtoqjoxxyu.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.daxiang520.top/gtfwgcnmqy.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.zhijiandao.cn/gtvwyyaicq.html

[Q13] 忽略重复插入
来源：http://hz.xylfe.cn/gtxapftimw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.smart0.xyz/gtkeazgggc.html

[Q14] 存在则更新（upsert）
来源：http://hz.c1oappe.top/gtlsoazwxw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.xylfe.cn/gterycuvuu.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.meibo888.top/gtmfgdflmv.html

[Q15] 查询全部
来源：http://hz.yonumen.top/gtikuobark.html


<!-- 参考信息 -->