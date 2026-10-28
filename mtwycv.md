代发 wailian999

Py:   if __name__ == "__main__":
来源：http://hz.hywenlv.cn/gtxfnncvxb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.c1oappe.top/gthdwynpzf.html

JS:   require.main === module
来源：http://hz.yangfankeji.com/gtwfohbtql.html

TS:   require.main === module
来源：http://hz.ybcxt.top/gtahvwqzpg.html

Java: public static void main(String[] args)
来源：http://hz.chenjidiqi.icu/gtqpzhdrmt.html

Go:   func main()
来源：http://hz.gotoacloud.top/gtrrcwetkp.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.vqdsnc.cn/gtvtwrzxvw.html

C#:   static void Main(string[] args)
来源：http://hz.shangyingyoupin.top/gtnoqdrtqk.html

[M08] 获取系统与运行时信息
来源：http://hz.sxryk.cn/gtkhprqsrf.html

Py:   platform.system();  platform.python_version()
来源：http://hz.chenzaomai.com/gtcwdlucdh.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.daxiang520.top/gtilfywiyh.html

JS:   process.platform;  process.version
来源：http://hz.iojbl.cn/gtunxglamg.html

TS:   process.platform;  process.version
来源：http://hz.ywan-chungtsiang.top/gtjipxowfh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.zhiwuduotai.top/gtcnchbkys.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.redwolf501.top/gterjqfoly.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.shzxlz.cn/gtxykpzarb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.zhaomingkeji.xyz/gtueqxquzq.html

================================================================================
来源：http://hz.sysykeji.top/gtldwuewil.html

N. 数据结构与算法
来源：http://hz.nwbrower.top/gtipbusvtw.html

================================================================================
来源：http://hz.316326.xyz/gtvhrlutps.html

[N01] 二分查找（有序数组）
来源：http://hz.wangdashe.top/gtbjrxflql.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.jqgfzy.top/gthyroanig.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jinqigfzy.top/gtxwjyunza.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.gaohongyu789.top/gtbqhrfmtl.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xinyue.icu/gttxsrskmv.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.vqdsnc.cn/gtrxvwgnbv.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.zhaomingkeji.xyz/gtqgdnwybv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.aibaodan.cn/gtbkbaqplz.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.shuidangran.top/gtnkhalqqk.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yangfankeji.com/gtouqqdrwj.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xylfe.cn/gtfyudytla.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yj202588.top/gtlgcnwoke.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.chenlongwang.top/gtwyqdelia.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hammf.cn/gtttkbvvze.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.jyoumei.cn/gtmdtygimh.html

Go:   slices.Sort(arr)
来源：http://hz.wangdashe.top/gtpnrcfbyy.html

Ruby: arr.sort
来源：http://hz.haohaochexian.top/gtedursbgo.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.cashguo.top/gtcxiseldg.html

[N03] 快速排序（分治示例）
来源：http://hz.sweek.top/gtmtyuovkt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.cqqwz.cn/gtbejwrjqb.html

PHP:  // 递归实现，或用 usort
来源：http://hz.cucudq.cn/gtcjewynjk.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.c1oappe.top/gtwnikeace.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.c1oappe.top/gtvtdrmljn.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jinqigufen.top/gtjnouxgya.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.hammf.cn/gtcrqheall.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.chenjidiqi.icu/gtfezslhvb.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.ywan-chungtsiang.top/gtmzjufxma.html

[N04] 斐波那契数列
来源：http://hz.yj20258888.top/gtgqkwyhib.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.xingfuxueyuan.xyz/gtnaozufeh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.shangyingyoupin.top/gtjvdoylno.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.guowangkeji.top/gtdxvjkwik.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hammf.cn/gtjcxykgdo.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.hysaishi.cn/gtmtihxbcv.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.havefunace.top/gtrfwprigl.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.zhiwuduotai.top/gtrnozpfaj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.c1oappe.top/gtanemmwfs.html

[N05] 最大公约数
来源：http://hz.bjfxy.top/gtzzjxvvxm.html

Py:   math.gcd(a, b)
来源：http://hz.jinyuanbaomall.cn/gtlttkjaeb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.hnxiangtu.top/gthhmbzcqr.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yj202588.top/gtwhawxnuc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hysaishi.cn/gtbfecxekc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.shangyingyoupin.top/gtvuozieqf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.tanke756.top/gtpekcbxgf.html

Ruby: a.gcd(b)
来源：http://hz.sxryk.cn/gtuszxgkfo.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.gzhubu.top/gtegdzlxwv.html

[N06] 判断回文字符串
来源：http://hz.c1oappe.top/gtsizuwqgq.html

Py:   s == s[::-1]
来源：http://hz.ivvv.top/gtstpptgrv.html

PHP:  $s === strrev($s);
来源：http://hz.yuxming.cn/gtavdmqzmg.html

JS:   s === [...s].reverse().join("")
来源：http://hz.snrcjt.cn/gtqdqboabs.html

TS:   s === [...s].reverse().join("")
来源：http://hz.jqgufenzy.top/gtesrhguxn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.guannengcc.top/gteoeealey.html

Go:   // 双指针从两端比较
来源：http://hz.yuxming.cn/gthhvkzhhf.html

Ruby: s == s.reverse
来源：http://hz.snrcjt.cn/gtmspytojc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yonumen.top/gtkddogodr.html

[N07] 两数之和（返回下标）
来源：http://hz.shanyushiyangtech.top/gtgwdhtrbm.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.haohaochexian.top/gttmriwrsr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.316326.xyz/gtprrmjbpu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.xziqi.cn/gtjwzygths.html

TS:   // 手写 Map<string, number>
来源：http://hz.ywan-chungtsiang.top/gtlplgpfai.html

Java: // 手写 HashMap
来源：http://hz.mhx1999.top/gtclcnmcna.html

Go:   // 手写 map[int]int
来源：http://hz.sxryk.cn/gtpcgtffaa.html

Ruby: // 手写 Hash
来源：http://hz.snrcjt.cn/gtbjnaptql.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.xuetiantiany.cn/gtwmgrbxzi.html

[N08] 生成全排列
来源：http://hz.chenlongwang.top/gtbucjzidr.html

Py:   itertools.permutations(arr)
来源：http://hz.jianghu66.top/gtdmeelqep.html

PHP:  // 手写递归交换
来源：http://hz.kuanghao11.cn/gtbqwjaril.html

JS:   // 手写回溯递归
来源：http://hz.yj20258.top/gtotivzdvo.html

TS:   // 手写回溯递归
来源：http://hz.gogol.net.cn/gtocgedfvc.html

Java: // 手写回溯递归
来源：http://hz.hongshengwenyu.top/gtmoscagpb.html

Go:   // 手写回溯递归
来源：http://hz.yongpay.top/gtbyfaqjnb.html

Ruby: arr.permutation.to_a
来源：http://hz.meibo888.top/gttougmkjn.html

C#:   // 手写回溯递归
来源：http://hz.sysykeji.top/gtcdmsewnn.html

[N09] 栈与队列
来源：http://hz.ydjk.org.cn/gtqbtptsfy.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.nanxuanxn.top/gtndbqzury.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.jqgfzy.top/gtqmyesmvm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.jlsjyb.cn/gtikflwvux.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.tanke756.top/gtvccffgxl.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yuxming.cn/gtnetasdth.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.dashuyun.cn/gtufyaxsyr.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.mhx1999.top/gtzxrtbuhi.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.tianlin.xyz/gtsogrophe.html

[N10] 链表节点定义
来源：http://hz.ydzc1.top/gtkywdbeeg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.xuanzx.com/gtrzulvvoc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.ehwqpu.com/gtbsfatgup.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.hnqzz.top/gtmkfaakyi.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.mhx1999.top/gtjispkwwf.html

Java: class Node { int v; Node next; }
来源：http://hz.dashuyun.cn/gtlxyuswzs.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.ywan-chungtsiang.top/gtrbcismep.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.kuanghao11.cn/gtsuwsnqcx.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.hnxiangtu.top/gtpvxgmicb.html

[N11] 二叉树中序遍历
来源：http://hz.c1oappe.top/gtlttrytne.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.yangfankeji.com/gtpqzgraib.html

PHP:  // 手写递归函数
来源：http://hz.yuxming.cn/gtdkilnqst.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.wangdashe.top/gthircgqik.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.xuanzx.com/gtbgboejip.html

Java: // 手写递归
来源：http://hz.quarkkingdee.top/gtepizqjnt.html

Go:   // 手写递归
来源：http://hz.ydjk.org.cn/gtbowvnqub.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.jyoumei.cn/gtjdmhauov.html

C#:   // 手写递归
来源：http://hz.hongshengwenyu.top/gtjykiyswo.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.meibo888.top/gteanahjfb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.316326.xyz/gtnkbtsqbs.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.zhaomingkeji.xyz/gtaoslsrdp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.havefunace.top/gthssptado.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yuanzhike.top/gtrvznbejl.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhiwuduotai.top/gtaragumrc.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.ybcxt.top/gtzsgkwrev.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.wangdashe.top/gtddoigdtt.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jyoumei.cn/gtcfldmgfl.html

================================================================================
来源：http://hz.hfpthk.cn/gtmnqvickp.html

O. 并发与异步
来源：http://hz.xylfe.cn/gtgmpawzvk.html

================================================================================
来源：http://hz.birdmap.top/gthqsiuprr.html

[O01] 启动一个线程
来源：http://hz.yj202588.top/gtvakqsjxn.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.shanyushiyangtech.top/gtbdsenmrc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.meibo888.top/gtvpdzvvzx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.fengsongda.top/gtqkpupaol.html

TS:   // 同 JS
来源：http://hz.sxryk.cn/gtuzbcdole.html

Java: new Thread(() -> f()).start()
来源：http://hz.yuanzhike.top/gtvbtyvpjl.html

Go:   go f()
来源：http://hz.ydzc1.top/gtggmuizbs.html

Ruby: Thread.new { f }
来源：http://hz.chenjidiqi.icu/gtazsmtcsf.html

C#:   Task.Run(() => F());
来源：http://hz.jlsjyb.cn/gtqiqmfjal.html

[O02] 使用线程池
来源：http://hz.wangshuangyany.cn/gtlizozigy.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.daria6918.cn/gtqialjjaq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.aizwys.cn/gtnelpottx.html

JS:   // worker_threads 线程池
来源：http://hz.yuxming.cn/gtqldyvipb.html

TS:   // worker_threads 线程池
来源：http://hz.tianlin.xyz/gtwmxhuxfa.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.zdqjudy.top/gtenxyvdwy.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.jlsjyb.cn/gtxwryeqsf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yuxming.cn/gtdsaxcgln.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.daria6918.cn/gtzzkmreos.html

[O03] 加锁保护共享数据
来源：http://hz.aizwys.cn/gtqrzueqdu.html

Py:   with lock: shared += 1
来源：http://hz.shanyushiyangkeji.top/gtynaqwtpn.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.hammf.cn/gtaviojdbz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.andypj.xyz/gtpetfaoif.html

TS:   // 同 JS
来源：http://hz.nanxinkj.top/gtrnnezknu.html

Java: synchronized (this) { shared++; }
来源：http://hz.havefunace.top/gtelkhjekw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.hfpthk.cn/gtipdvncrr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jianghu66.top/gtziskwxwc.html

C#:   lock (gate) { shared++; }
来源：http://hz.0kj1m.cn/gtesuyxcse.html

[O04] 定义异步函数并等待
来源：http://hz.jinghuilouyu.cn/gtvwptcskr.html

Py:   async def f():⏎    await g()
来源：http://hz.zdqjudy.top/gtoylimnpu.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.zhijiandao.cn/gtkbzekvyc.html

JS:   async function f() { await g(); }
来源：http://hz.cucudq.cn/gtmlelzppo.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yuxming.cn/gtbiszbjhq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.zdqjudy.top/gtkofaalwa.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.jyoumei.cn/gtrsgvrbeb.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.birdmap.top/gtzkpmfpua.html

C#:   async Task F() { await G(); }
来源：http://hz.52xcode.cn/gtqzugihrr.html

[O05] 并发执行并等待全部完成
来源：http://hz.pycfn.com/gtxihbikoy.html

Py:   asyncio.gather(*tasks)
来源：http://hz.tanke756.top/gtjsbavnfj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.guannengcc.top/gthsmtggsk.html

JS:   await Promise.all(tasks)
来源：http://hz.aibaodan.cn/gtiopvrwdu.html

TS:   await Promise.all(tasks)
来源：http://hz.daria6918.cn/gtcefdjrpt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.pycfn.com/gtomlkisbs.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.ehwqpu.com/gtopploetf.html

Ruby: threads.map(&:join)
来源：http://hz.jqgufenzy.top/gtkwjfstjd.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.shanyushiyangkeji.top/gtommdyvrg.html

[O06] 使用进程池
来源：http://hz.hongshengwenyu.top/gtgqokbhab.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.nanxuanxn.top/gtqvgdmpzn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.zhixingplan.top/gtqqsjqxro.html

JS:   // child_process / cluster 模块
来源：http://hz.zhixingplan.top/gtpbllmwva.html

TS:   // child_process / cluster 模块
来源：http://hz.jinqigufen.top/gtorucbmni.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.hongshengwenyu.top/gtbtelhcli.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.haohaochexian.top/gthiwpqoat.html

Ruby: // fork 块
来源：http://hz.daxiang520.top/gthqklcajp.html

C#:   Parallel.For
来源：http://hz.tianlin.xyz/gtcjwtuzag.html

================================================================================
来源：http://hz.shuidangran.top/gtdvboopzl.html

P. 常用工具函数
来源：http://hz.hnqzz.top/gteifnmkkm.html

================================================================================
来源：http://hz.fzhhl.top/gtdfgjfhui.html

[P01] 生成 UUID
来源：http://hz.yj20258888.top/gtgcxkdzgk.html

Py:   str(uuid.uuid4())
来源：http://hz.jianghu66.top/gtqmzrkeoe.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.gzhubu.top/gtwqflsyge.html

JS:   crypto.randomUUID()
来源：http://hz.guowangkeji.top/gthkhefnzy.html

TS:   crypto.randomUUID()
来源：http://hz.yueranfly.top/gtmqddaxwv.html

Java: UUID.randomUUID().toString()
来源：http://hz.pycfn.com/gtkkyydrtm.html

Go:   // 用 github.com/google/uuid
来源：http://hz.jqgufenzy.top/gtqmojnpsd.html

Ruby: SecureRandom.uuid
来源：http://hz.jinyuanbaomall.cn/gtvwqimqsp.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.vqdsnc.cn/gtghdxvhvt.html

[P02] MD5 / SHA256 摘要
来源：http://hz.aibaodan.cn/gtxkpeklxy.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.jyoumei.cn/gtrfnzlliu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.gogol.net.cn/gtzghrjqeh.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.52xcode.cn/gtvsdotvwk.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.yonumen.top/gtjudmrsyh.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.yj202588.top/gtngpluwwx.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.birdmap.top/gtqufydcbu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.yj202588.top/gtkrotsdlm.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.hysaishi.cn/gtyhlujuaq.html

[P03] 生成短随机字符串
来源：http://hz.zhongyouzk.top/gtpepaohos.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.hongshengwenyu.top/gtupgkfspu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.c1oappe.top/gtutcyblcv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.daria6918.cn/gtzydpbfwm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.cheryme.top/gtoixsbmtp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.cdnleiting.top/gtmvgbltvh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yangfankeji.com/gthihxlbob.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.fzhhl.top/gtsmpfrkhf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.havefunace.top/gtqdlrqwtz.html

[P04] 求长度
来源：http://hz.redwolf501.top/gtdlqfxyjr.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.wangshuangyany.cn/gtjamtncru.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.sysykeji.top/gtwjxfftem.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xinyue.icu/gttqhphzhv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.wangshuangyany.cn/gtbwcibdit.html

Java: list.size();  map.size();  s.length()
来源：http://hz.ywan-chungtsiang.top/gtfsmfycoa.html

Go:   len(arr);  len(m)
来源：http://hz.sxryk.cn/gthvbzqwlr.html

Ruby: x.length;  x.size
来源：http://hz.gotoacloud.top/gtwcelhmoe.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.jlsjyb.cn/gtnvdbfnxv.html

[P05] 判断两个对象内容是否相等
来源：http://hz.dianchejie.cn/gtvnuceuca.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.52xcode.cn/gtztqcrvix.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.tanke756.top/gtshaklwgi.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.guannengcc.top/gtkvshwdbi.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jqgfzy.top/gtjbfgubfb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jinqigfzy.top/gtbbhxevbj.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.zhengqikj.top/gtwzetkjuw.html

Ruby: a == b
来源：http://hz.daxiang520.top/gtwtixyate.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.fengsongda.top/gtsfihgtgj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.aibaodan.cn/gtskflkxhv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.cashguo.top/gtvksnswdk.html

PHP:  if (empty($x)) {}
来源：http://hz.smart0.xyz/gtruxxhxuu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jinqigufen.top/gthvbixxew.html

TS:   if (x == null) {}
来源：http://hz.tianlin.xyz/gtvutdgcnh.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.cashguo.top/gtvywfwgcd.html

Go:   if x == nil {}
来源：http://hz.zycfv.cn/gthwrzbvbf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.chenzaomai.com/gtrzifkces.html

C#:   if (x is null) {}
来源：http://hz.shanyushiyangtech.top/gtekstrcyq.html

[P07] 防抖与节流
来源：http://hz.dashuyun.cn/gtpvxqitbv.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jianghu66.top/gtydwcqsfd.html

PHP:  // 手写时间戳比较
来源：http://hz.hnqzz.top/gtdmbxgoax.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cheryme.top/gtkyuefnrw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.iojbl.cn/gtsniayvnv.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.jyoumei.cn/gtfcdyxdgd.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.havefunace.top/gthxrnpdsx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.guowangkeji.top/gtshjitgzv.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.pengpengdd.cyou/gtxdldfoud.html

[P08] 处理浮点精度问题
来源：http://hz.tanke756.top/gtllypheji.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.sufxvd.cn/gttihvpeof.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.mhx1999.top/gtvtddmijb.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.daria6918.cn/gtxopykrpf.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.nanxinkj.top/gtoxilityh.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.ppjwa.cn/gtcezzcbpq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.redwolf501.top/gtjtoaatzx.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.sweek.top/gtufrgkaas.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.nwbrower.top/gtiodwwuje.html

================================================================================
来源：http://hz.zhoulong.xyz/gtkweqouxu.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.shangyingyoupin.top/gtvlrqtfex.html

================================================================================
来源：http://hz.hammf.cn/gthxxnsjvo.html

[Q01] 创建表
来源：http://hz.aibaodan.cn/gteszmsgyl.html

CREATE TABLE users (
来源：http://hz.yanxiufei.cn/gtmyybpadn.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jianghu66.top/gtgxjqukzd.html

name VARCHAR(50) NOT NULL,
来源：http://hz.ybcxt.top/gtqretpnsq.html

email VARCHAR(100) UNIQUE,
来源：http://hz.zhiwuduotai.top/gthpieckuj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.yj20258888.top/gtjisahejk.html

);
来源：http://hz.wangshuangyany.cn/gtqzwondhy.html

[Q02] 创建带外键的表
来源：http://hz.iojbl.cn/gtjiiuwbts.html

CREATE TABLE orders (
来源：http://hz.zdqjudy.top/gtgxniagia.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.sysykeji.top/gtzsglhmqh.html

user_id INT NOT NULL,
来源：http://hz.shangyingyoupin.top/gtnmmxoqjf.html

amount DECIMAL(10, 2),
来源：http://hz.gotoacloud.top/gtjgyvxroy.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.fzhhl.top/gtqvkigzmh.html

);
来源：http://hz.cheryme.top/gtrulowqzb.html

[Q03] 增加列
来源：http://hz.gaohongyu789.top/gtrkfjpnhe.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.yueranfly.top/gtkzcutkre.html

[Q04] 修改列类型
来源：http://hz.jianghu66.top/gtcmqtyzfz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.chenzaomai.com/gtblcdxbxl.html

[Q05] 重命名列
来源：http://hz.cashguo.top/gtctjhlipl.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.jiagoushi.top/gtdzxwdbze.html

[Q06] 删除列
来源：http://hz.shzxlz.cn/gtlglkcqdg.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.ywan-chungtsiang.top/gtojcbciqq.html

[Q07] 删除表
来源：http://hz.quarkkingdee.top/gttmyyizvk.html

DROP TABLE IF EXISTS orders;
来源：http://hz.iojbl.cn/gtxpewtpks.html

[Q08] 创建普通索引
来源：http://hz.pengpengdd.cyou/gtylsrastn.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.svipenyu.cn/gtpffmnnrc.html

[Q09] 创建唯一索引
来源：http://hz.chenjidiqi.icu/gtesuexqgw.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.xingfuxueyuan.xyz/gthltjdevq.html

[Q10] 插入单行
来源：http://hz.birdmap.top/gtiqsygnbt.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.wangdashe.top/gtzyersuyr.html

[Q11] 一次插入多行
来源：http://hz.yj20258.top/gtogbabgsn.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.ybcxt.top/gtypeaswzf.html

[Q12] 插入后取自增 ID
来源：http://hz.gzhubu.top/gtnrobikba.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.hfpthk.cn/gtnjgfbnce.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yonumen.top/gtswxwbjcb.html

[Q13] 忽略重复插入
来源：http://hz.52xcode.cn/gtmxroaftz.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.yongpay.top/gtaizcibhi.html


<!-- 参考信息 -->