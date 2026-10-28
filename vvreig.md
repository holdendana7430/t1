代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.fzhhl.top/gtifqmzdlr.html

Ruby: warn "err"
来源：http://hz.zhiwuduotai.top/gtgqwvdxhx.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.xylfe.cn/gtsbamqnmw.html

[M07] 判断是否为主入口
来源：http://hz.tanke756.top/gthwbbuxrf.html

Py:   if __name__ == "__main__":
来源：http://hz.nwbrower.top/gtnafumfbc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zhijiandao.cn/gtkwqoxmkv.html

JS:   require.main === module
来源：http://hz.yanxiufei.cn/gtzelywany.html

TS:   require.main === module
来源：http://hz.316326.xyz/gtvnqqeopb.html

Java: public static void main(String[] args)
来源：http://hz.jinghuilouyu.cn/gtkxdswogz.html

Go:   func main()
来源：http://hz.zhijiandao.cn/gtxglhudyj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.gaohongyu789.top/gtikpqqpgs.html

C#:   static void Main(string[] args)
来源：http://hz.yuxming.cn/gtjgwcbgqr.html

[M08] 获取系统与运行时信息
来源：http://hz.xylfe.cn/gtdkkaqesl.html

Py:   platform.system();  platform.python_version()
来源：http://hz.zdqjudy.top/gtoioilvab.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.andypj.xyz/gtncubgwfs.html

JS:   process.platform;  process.version
来源：http://hz.hywenlv.cn/gtcdftgnxl.html

TS:   process.platform;  process.version
来源：http://hz.bjfxy.top/gtgvvwtqzh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.sysykeji.top/gtatkazkuc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yuxming.cn/gtstvioxrp.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.dashuyun.cn/gttymrsyae.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.chenjidiqi.icu/gtlniycdmh.html

================================================================================
来源：http://hz.hammf.cn/gtffbznerx.html

N. 数据结构与算法
来源：http://hz.tianlin.xyz/gtcdsbgplh.html

================================================================================
来源：http://hz.kuanghao11.cn/gtpjlomijb.html

[N01] 二分查找（有序数组）
来源：http://hz.cdnleiting.top/gtcvhjdlal.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.cdnleiting.top/gtyoghbsoq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.aibaodan.cn/gtbqoycfvz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.kuanghao11.cn/gthsqhsksg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.shzxlz.cn/gtytvvxihr.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.ybcxt.top/gtsddygwqx.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.9152youxi.cn/gtpmodliqe.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.hfpthk.cn/gtzotmfkii.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.vqdsnc.cn/gtgbpqdwzl.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jyoumei.cn/gtrvtiioll.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cqqwz.cn/gtgivxkftn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.cdnleiting.top/gtpknmwihv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hnxiangtu.top/gtsckapsjz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.svipenyu.cn/gtmckdbguh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.svipenyu.cn/gtnwfziesb.html

Go:   slices.Sort(arr)
来源：http://hz.jiagoushi.top/gtmkdnhwev.html

Ruby: arr.sort
来源：http://hz.ybcxt.top/gtemzbflid.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.jlsjyb.cn/gtlrkfexxf.html

[N03] 快速排序（分治示例）
来源：http://hz.zhengqikj.top/gtakynsulz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.hnxiangtu.top/gtdfevytlz.html

PHP:  // 递归实现，或用 usort
来源：http://hz.guowangkeji.top/gtuxyfzevb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhijiandao.cn/gtynbvvfar.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jinqigufen.top/gtjqhepupr.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jiagoushi.top/gtwpmamryl.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yangfankeji.com/gtzqaittig.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.sweek.top/gtjvkmhcha.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.tianlin.xyz/gtjxxrvwgz.html

[N04] 斐波那契数列
来源：http://hz.jiagoushi.top/gtbihbccml.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yj20258.top/gtwbetafrk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.iojbl.cn/gtoaghrztc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.sufxvd.cn/gtimubpgge.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.iojbl.cn/gtwdjykkrt.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.xuanzx.com/gtmkdzfjaj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.tanke756.top/gtrhjqwkwb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.shzxlz.cn/gtullpsyof.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.tianlin.xyz/gtqdefldky.html

[N05] 最大公约数
来源：http://hz.chenlongwang.top/gtfjiwjibw.html

Py:   math.gcd(a, b)
来源：http://hz.yanxiufei.cn/gtxmbejrhv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.hnxiangtu.top/gtkljmcrhc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.shzxlz.cn/gtfdxvdnxe.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hfpthk.cn/gtbbdkiohe.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.aibaodan.cn/gtcnqxriul.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.hfpthk.cn/gtocymknuq.html

Ruby: a.gcd(b)
来源：http://hz.jinyuanbaomall.cn/gtkmmcppjl.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yj20258.top/gttifslvcf.html

[N06] 判断回文字符串
来源：http://hz.guowangkeji.top/gturirctrn.html

Py:   s == s[::-1]
来源：http://hz.ivvv.top/gthndoxgyt.html

PHP:  $s === strrev($s);
来源：http://hz.tianlin.xyz/gtvurgvhhi.html

JS:   s === [...s].reverse().join("")
来源：http://hz.zhongyouzk.top/gtincqqgqo.html

TS:   s === [...s].reverse().join("")
来源：http://hz.52xcode.cn/gtpqjicuki.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.ydjk.org.cn/gtjlarplck.html

Go:   // 双指针从两端比较
来源：http://hz.yj20258.top/gtahlksbef.html

Ruby: s == s.reverse
来源：http://hz.zhongyouzk.top/gtskakmsqr.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.mhx1999.top/gtzwlrrhip.html

[N07] 两数之和（返回下标）
来源：http://hz.9152youxi.cn/gtnyqlbknr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.mhx1999.top/gtvtvjqerk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.cheryme.top/gtuylrhqcb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.guannengcc.top/gtpaotaskk.html

TS:   // 手写 Map<string, number>
来源：http://hz.nanxinkj.top/gtlmhbhcdk.html

Java: // 手写 HashMap
来源：http://hz.jinghuilouyu.cn/gtkylryyzb.html

Go:   // 手写 map[int]int
来源：http://hz.tanke756.top/gtvzmyulzl.html

Ruby: // 手写 Hash
来源：http://hz.birdmap.top/gtffdhkcdc.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.fzhhl.top/gtysexddqc.html

[N08] 生成全排列
来源：http://hz.jiagoushi.top/gtkvnqwuop.html

Py:   itertools.permutations(arr)
来源：http://hz.kuanghao11.cn/gtdhrcdnia.html

PHP:  // 手写递归交换
来源：http://hz.ydjk.org.cn/gtoawsbjec.html

JS:   // 手写回溯递归
来源：http://hz.shzxlz.cn/gtieliupje.html

TS:   // 手写回溯递归
来源：http://hz.cheryme.top/gtxyykoliq.html

Java: // 手写回溯递归
来源：http://hz.pengpengdd.cyou/gtelqlqqlp.html

Go:   // 手写回溯递归
来源：http://hz.xuetiantiany.cn/gtozfvoxdv.html

Ruby: arr.permutation.to_a
来源：http://hz.jyoumei.cn/gtmmxxaxjb.html

C#:   // 手写回溯递归
来源：http://hz.dianchejie.cn/gtvyvvfnek.html

[N09] 栈与队列
来源：http://hz.svipenyu.cn/gtjuzeillf.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yonumen.top/gtqxuzvxfx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.jqgfzy.top/gtarvkllkr.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.ppjwa.cn/gtbhsurjsh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.svipenyu.cn/gtdtgpycdt.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.52xcode.cn/gtkmsrkyqr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.zhengqikj.top/gtxtpibdkz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.shanyushiyangtech.top/gtedcoopgk.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.cashguo.top/gtxfsgorho.html

[N10] 链表节点定义
来源：http://hz.meibo888.top/gtegjydmqw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.zycfv.cn/gtdjwrptll.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.redwolf501.top/gtjcpvmqts.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zhijiandao.cn/gtzzbunixt.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.havefunace.top/gtqzzfiwks.html

Java: class Node { int v; Node next; }
来源：http://hz.nwbrower.top/gtrfonwrju.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.xingfuxueyuan.xyz/gtolxabwzo.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.xinyue.icu/gtojtkzyqb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.jinghuilouyu.cn/gtcdvzkeew.html

[N11] 二叉树中序遍历
来源：http://hz.hnqzz.top/gtgorlawau.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.shanyushiyangtech.top/gtfuimsvbe.html

PHP:  // 手写递归函数
来源：http://hz.quarkkingdee.top/gtoumsdckq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.gogol.net.cn/gtbwrwfwnw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhijiandao.cn/gtotesgiok.html

Java: // 手写递归
来源：http://hz.tianlin.xyz/gtgaclzxgj.html

Go:   // 手写递归
来源：http://hz.yongpay.top/gtovzksrqv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.xuanzx.com/gtcyxebcvt.html

C#:   // 手写递归
来源：http://hz.jinqigfzy.top/gtnwdaujhl.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.kuanghao11.cn/gtvhdvwmwc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.hfpthk.cn/gthuadljga.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.gzhubu.top/gtffphzncw.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xuanzx.com/gtdprnielz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhixingplan.top/gtaoomwwjd.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.svipenyu.cn/gtcfujvcou.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.tianlin.xyz/gtntlpqsss.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.tanke756.top/gtymbybljj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yangfankeji.com/gtfhiwqijp.html

================================================================================
来源：http://hz.hammf.cn/gtknxbevxu.html

O. 并发与异步
来源：http://hz.gogol.net.cn/gtmlrwzlzv.html

================================================================================
来源：http://hz.xziqi.cn/gtoruvrpkf.html

[O01] 启动一个线程
来源：http://hz.aibaodan.cn/gtpabxslfi.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.wangshuangyany.cn/gtqemewzsa.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.gaohongyu789.top/gttfyxbgsm.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.daria6918.cn/gtxqujyvpn.html

TS:   // 同 JS
来源：http://hz.jqgufenzy.top/gtshtvfzuu.html

Java: new Thread(() -> f()).start()
来源：http://hz.jyoumei.cn/gtviyynuen.html

Go:   go f()
来源：http://hz.wangdashe.top/gtotgntdlr.html

Ruby: Thread.new { f }
来源：http://hz.zhongyouzk.top/gtgtgphgfa.html

C#:   Task.Run(() => F());
来源：http://hz.yongpay.top/gttmyiihfi.html

[O02] 使用线程池
来源：http://hz.jinqigufen.top/gtisiisadv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.wangdashe.top/gtuqicqvjz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.pycfn.com/gtepwtfqzc.html

JS:   // worker_threads 线程池
来源：http://hz.guowangkeji.top/gtwdvkzgel.html

TS:   // worker_threads 线程池
来源：http://hz.mhx1999.top/gtzfoprsqh.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yvedp.cn/gteqwbzcln.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.xuanzx.com/gtniatbyll.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.havefunace.top/gtlafdrrvb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.ydzc1.top/gtyrgeuxjw.html

[O03] 加锁保护共享数据
来源：http://hz.tianlin.xyz/gtnqtcmufl.html

Py:   with lock: shared += 1
来源：http://hz.yangfankeji.com/gtmzcagohq.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zhixingplan.top/gtyaobdkxz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.zhoulong.xyz/gtcwtfzatw.html

TS:   // 同 JS
来源：http://hz.mhx1999.top/gtgsogacye.html

Java: synchronized (this) { shared++; }
来源：http://hz.bjfxy.top/gttntwdujp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.cheryme.top/gtudnxamqe.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.yonumen.top/gtbjsxltbv.html

C#:   lock (gate) { shared++; }
来源：http://hz.yvedp.cn/gtsqelfyhg.html

[O04] 定义异步函数并等待
来源：http://hz.birdmap.top/gtbmdumfri.html

Py:   async def f():⏎    await g()
来源：http://hz.guowangkeji.top/gtusoyihcf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.nanxinkj.top/gthoxrvvia.html

JS:   async function f() { await g(); }
来源：http://hz.xuanzx.com/gtzcnbhgqq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.svipenyu.cn/gtgojahasz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.daxiang520.top/gticsokcjf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.ydjk.org.cn/gtkdcmvthq.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.jiagoushi.top/gtzpvhcjct.html

C#:   async Task F() { await G(); }
来源：http://hz.daxiang520.top/gtkojslazv.html

[O05] 并发执行并等待全部完成
来源：http://hz.feifeiyinyue.top/gtmunpdczb.html

Py:   asyncio.gather(*tasks)
来源：http://hz.nwbrower.top/gtbnjiaghn.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.snrcjt.cn/gtxpkrpawu.html

JS:   await Promise.all(tasks)
来源：http://hz.quarkkingdee.top/gtemquntqe.html

TS:   await Promise.all(tasks)
来源：http://hz.daxiang520.top/gtfbsjlgwk.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.feifeiyinyue.top/gtidosxcze.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yueranfly.top/gtzjildrfz.html

Ruby: threads.map(&:join)
来源：http://hz.yj20258888.top/gttzjywfro.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.9152youxi.cn/gtbpcvxecp.html

[O06] 使用进程池
来源：http://hz.tian-w.cn/gtfuamnrro.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.jqgfzy.top/gtiloxuqox.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.aibaodan.cn/gthuhnowqf.html

JS:   // child_process / cluster 模块
来源：http://hz.smart0.xyz/gtxrgcvqlw.html

TS:   // child_process / cluster 模块
来源：http://hz.ydzc1.top/gtbrkbwkhr.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.aizwys.cn/gtpqqhmpsw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.xuetiantiany.cn/gtzstunurw.html

Ruby: // fork 块
来源：http://hz.redwolf501.top/gttgxohmhb.html

C#:   Parallel.For
来源：http://hz.ivvv.top/gtbbccmnkm.html

================================================================================
来源：http://hz.sufxvd.cn/gtzebxtbnl.html

P. 常用工具函数
来源：http://hz.sweek.top/gtpizygekv.html

================================================================================
来源：http://hz.tianlin.xyz/gtfpjqanoe.html

[P01] 生成 UUID
来源：http://hz.yonumen.top/gtedlkpkcl.html

Py:   str(uuid.uuid4())
来源：http://hz.kuanghao11.cn/gtimdjdpsa.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.smart0.xyz/gtiaudgkso.html

JS:   crypto.randomUUID()
来源：http://hz.chenjidiqi.icu/gtnldaoais.html

TS:   crypto.randomUUID()
来源：http://hz.tian-w.cn/gteekprzys.html

Java: UUID.randomUUID().toString()
来源：http://hz.316326.xyz/gtxoewtkww.html

Go:   // 用 github.com/google/uuid
来源：http://hz.nanxuanxn.top/gtefbtkvvo.html

Ruby: SecureRandom.uuid
来源：http://hz.svipenyu.cn/gtqfwfgfds.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.shanyushiyangkeji.top/gtvjujbasu.html

[P02] MD5 / SHA256 摘要
来源：http://hz.ydzc1.top/gteezytnye.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.guowangkeji.top/gtzpngyvuu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.jinghuilouyu.cn/gtemxsbgqn.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yongpay.top/gtxpkimvxu.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.hywenlv.cn/gtoeyzsnyf.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.guannengcc.top/gtwszyvlly.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.sufxvd.cn/gtqtugknda.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.316326.xyz/gtxxiquwsp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.ydzc1.top/gtnbymrcqz.html

[P03] 生成短随机字符串
来源：http://hz.ehwqpu.com/gtcbsnhzuz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jinqigfzy.top/gtqsiljiix.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.hysaishi.cn/gtxrekooig.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.chenjidiqi.icu/gtcryrezjm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.birdmap.top/gtddvzunea.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yj20258888.top/gtjctnhayo.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.hnqzz.top/gtebrcaiov.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.ivvv.top/gtfgtjjufz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.hongshengwenyu.top/gtoegxgbud.html

[P04] 求长度
来源：http://hz.yueranfly.top/gtauodespl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.zhongyouzk.top/gtehyawdgk.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.9152youxi.cn/gtckciaaza.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yvedp.cn/gtdwnpqcgt.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jinyuanbaomall.cn/gthnopxnxg.html

Java: list.size();  map.size();  s.length()
来源：http://hz.iojbl.cn/gtvtyegsap.html

Go:   len(arr);  len(m)
来源：http://hz.zhaomingkeji.xyz/gttwzhtxuk.html

Ruby: x.length;  x.size
来源：http://hz.gogol.net.cn/gtphuefnbg.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.aibaodan.cn/gtiukzcqzo.html

[P05] 判断两个对象内容是否相等
来源：http://hz.sysykeji.top/gtelrwgwzp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.redwolf501.top/gttrdrbamh.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.ydjk.org.cn/gtpykujccq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.0kj1m.cn/gtnsrwmwxj.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.mhx1999.top/gtizjpjert.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.dashuyun.cn/gtgltujzpw.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.bjfxy.top/gtreqrzaww.html

Ruby: a == b
来源：http://hz.yonumen.top/gtxfmrmgog.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.sxryk.cn/gtgshqgkgx.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.fengsongda.top/gtzhpidlww.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.svipenyu.cn/gtzwfgzogn.html

PHP:  if (empty($x)) {}
来源：http://hz.quarkkingdee.top/gtlrjfpgui.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.ehwqpu.com/gtenmonlcx.html

TS:   if (x == null) {}
来源：http://hz.birdmap.top/gtvqxdxdii.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.hysaishi.cn/gtufrabsag.html

Go:   if x == nil {}
来源：http://hz.smart0.xyz/gtfivorjfi.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.yanxiufei.cn/gtjqfvqozx.html

C#:   if (x is null) {}
来源：http://hz.gzhubu.top/gtbntijheu.html

[P07] 防抖与节流
来源：http://hz.gaohongyu789.top/gttdmqvuaw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.nanxinkj.top/gtewopellc.html

PHP:  // 手写时间戳比较
来源：http://hz.9152youxi.cn/gtmfdclraa.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xinyue.icu/gtnoggfscn.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jqgfzy.top/gtlsbdkkqa.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.yangfankeji.com/gtfdguhyde.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.jinghuilouyu.cn/gtlbsopvie.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.nwbrower.top/gtsiecmgun.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.gogol.net.cn/gtafcodyde.html

[P08] 处理浮点精度问题
来源：http://hz.cqqwz.cn/gtsqahyvqx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.cdnleiting.top/gtzqozgggi.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.feifeiyinyue.top/gtxbpvvxix.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.yvedp.cn/gtylbwspev.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.sufxvd.cn/gtuerowaxg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yuanzhike.top/gthwibkcpi.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.chenjidiqi.icu/gtcuudmwxr.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.ppjwa.cn/gtbtehmexv.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.jqgufenzy.top/gtwxivvvzm.html

================================================================================
来源：http://hz.zhijiandao.cn/gtlhxymvfo.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.tanke756.top/gtniapqnek.html

================================================================================
来源：http://hz.cashguo.top/gtvffkyuzf.html

[Q01] 创建表
来源：http://hz.pengpengdd.cyou/gtojozptit.html

CREATE TABLE users (
来源：http://hz.cdnleiting.top/gtcupqyiir.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jinqigfzy.top/gtbowdicos.html

name VARCHAR(50) NOT NULL,
来源：http://hz.hysaishi.cn/gtdbudkhwq.html

email VARCHAR(100) UNIQUE,
来源：http://hz.dashuyun.cn/gtcovbovue.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.gotoacloud.top/gtmtycjzgu.html

);
来源：http://hz.yuxming.cn/gtxhrxsnga.html

[Q02] 创建带外键的表
来源：http://hz.c1oappe.top/gtgsyjekkr.html

CREATE TABLE orders (
来源：http://hz.ydzc1.top/gtzloocdrt.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.dianchejie.cn/gthrpmnaiq.html

user_id INT NOT NULL,
来源：http://hz.yuxming.cn/gtaprrklho.html

amount DECIMAL(10, 2),
来源：http://hz.hammf.cn/gtbibsdhhz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.wangdashe.top/gtlsnkrdbm.html

);
来源：http://hz.zhixingplan.top/gtapxidvzt.html

[Q03] 增加列
来源：http://hz.hfpthk.cn/gtnrozfnmq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.zhengqikj.top/gtupwkoujs.html

[Q04] 修改列类型
来源：http://hz.havefunace.top/gtjwtyghsw.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.yj20258888.top/gtwggsenth.html

[Q05] 重命名列
来源：http://hz.yvedp.cn/gtqekvxnal.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.guannengcc.top/gtgunbimji.html

[Q06] 删除列
来源：http://hz.gzhubu.top/gtnkjybwok.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.jiagoushi.top/gtmbtzvxtp.html

[Q07] 删除表
来源：http://hz.zhijiandao.cn/gtrttecpmv.html

DROP TABLE IF EXISTS orders;
来源：http://hz.yuanzhike.top/gtdourduvh.html

[Q08] 创建普通索引
来源：http://hz.vqdsnc.cn/gtmjfstruk.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.nanxinkj.top/gtaaodoeue.html

[Q09] 创建唯一索引
来源：http://hz.cqqwz.cn/gtvzmpkozd.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.nanxuanxn.top/gttjklpnjw.html

[Q10] 插入单行
来源：http://hz.nanxuanxn.top/gtqxkurjza.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.shanyushiyangtech.top/gtqfpqhpvh.html

[Q11] 一次插入多行
来源：http://hz.kuanghao11.cn/gtzwbexalu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yangfankeji.com/gtibspswqt.html

[Q12] 插入后取自增 ID
来源：http://hz.yuanzhike.top/gtyvnjnmxh.html


<!-- 参考信息 -->