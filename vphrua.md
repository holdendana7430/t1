代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.xylfe.cn/gtiklltyfq.html

JS:   console.error("err")
来源：http://hz.jinqigfzy.top/gtuwytfmin.html

TS:   console.error("err")
来源：http://hz.zycfv.cn/gtxsbpbner.html

Java: System.err.println("err")
来源：http://hz.daria6918.cn/gttfymermn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.0kj1m.cn/gtrfihzict.html

Ruby: warn "err"
来源：http://hz.jianghu66.top/gtaiwoelqf.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.shangyingyoupin.top/gtoubejakw.html

[M07] 判断是否为主入口
来源：http://hz.9152youxi.cn/gtogvzfevi.html

Py:   if __name__ == "__main__":
来源：http://hz.xylfe.cn/gtkqikrwms.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.0kj1m.cn/gticlhgahl.html

JS:   require.main === module
来源：http://hz.cqqwz.cn/gtuocarmoh.html

TS:   require.main === module
来源：http://hz.ydzc1.top/gtcbpdfftv.html

Java: public static void main(String[] args)
来源：http://hz.quarkkingdee.top/gtlyogqsux.html

Go:   func main()
来源：http://hz.316326.xyz/gtwwteqhlw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.xuetiantiany.cn/gtybzwgxui.html

C#:   static void Main(string[] args)
来源：http://hz.jinqigfzy.top/gtkaaflsfl.html

[M08] 获取系统与运行时信息
来源：http://hz.fengsongda.top/gtqioijnlk.html

Py:   platform.system();  platform.python_version()
来源：http://hz.9152youxi.cn/gtfcjtozzm.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.fzhhl.top/gtvlfgucrq.html

JS:   process.platform;  process.version
来源：http://hz.hywenlv.cn/gtdnbxprbo.html

TS:   process.platform;  process.version
来源：http://hz.jiagoushi.top/gthyhtjuyx.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.gotoacloud.top/gteujhgvfd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.aibaodan.cn/gtblshrgub.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.ivvv.top/gtjnewivab.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.jlsjyb.cn/gtwrgwvuod.html

================================================================================
来源：http://hz.c1oappe.top/gtbxkmizdh.html

N. 数据结构与算法
来源：http://hz.ywan-chungtsiang.top/gtjkxhiweo.html

================================================================================
来源：http://hz.xinyue.icu/gtwshlwsvs.html

[N01] 二分查找（有序数组）
来源：http://hz.316326.xyz/gtvxxqwatk.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.xinyue.icu/gtyxdemqow.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yuanzhike.top/gthqdmjgrq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.vqdsnc.cn/gtyostgeti.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.dashuyun.cn/gtkqbdewrc.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.zdqjudy.top/gtrsqdcrmc.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.kuanghao11.cn/gtiwefqhnn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jiagoushi.top/gtugortpso.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.snrcjt.cn/gtsmegwfjx.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.smart0.xyz/gtxnruluuf.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yj20258.top/gtxpvnbmtu.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yuanzhike.top/gtnppumbwr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yanxiufei.cn/gtfebsvbop.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.svipenyu.cn/gtditzxxts.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.wangdashe.top/gtiktnmzir.html

Go:   slices.Sort(arr)
来源：http://hz.cdnleiting.top/gtcmxiuywc.html

Ruby: arr.sort
来源：http://hz.ivvv.top/gtfvbdcykh.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.xingfuxueyuan.xyz/gtvsqajhkw.html

[N03] 快速排序（分治示例）
来源：http://hz.nanxuanxn.top/gthnbnqzdz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.aizwys.cn/gtnwxppkwn.html

PHP:  // 递归实现，或用 usort
来源：http://hz.meibo888.top/gthjiwyvxu.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xziqi.cn/gtkugghogw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.shanyushiyangkeji.top/gtdzrsfemh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.zhiwuduotai.top/gtkcqtpnvi.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.tianlin.xyz/gtneksjlrs.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.hnxiangtu.top/gtdtjjhwdv.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.smart0.xyz/gtlyuejrwl.html

[N04] 斐波那契数列
来源：http://hz.cqqwz.cn/gtwldpxuly.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.sysykeji.top/gtcmlkpfms.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.wangshuangyany.cn/gtjdufbrcd.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.quarkkingdee.top/gtanzwstpx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yuanzhike.top/gtbtdjgsbn.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.mhx1999.top/gtmmjsnrns.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jyoumei.cn/gtzfmhgkjw.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.sxryk.cn/gtkgiqhfqz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.nwbrower.top/gttcxnigao.html

[N05] 最大公约数
来源：http://hz.ppjwa.cn/gtefuvrwnw.html

Py:   math.gcd(a, b)
来源：http://hz.jinqigufen.top/gtknkabjah.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.cucudq.cn/gtwkhrtofn.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.bjfxy.top/gtautvmxzi.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhongyouzk.top/gtyvqdbjww.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.tian-w.cn/gtdwmtgnoz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.aizwys.cn/gtptguwvki.html

Ruby: a.gcd(b)
来源：http://hz.nanxinkj.top/gtmcsrqles.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yonumen.top/gtclzdzybz.html

[N06] 判断回文字符串
来源：http://hz.bjfxy.top/gtkzrshdui.html

Py:   s == s[::-1]
来源：http://hz.jqgufenzy.top/gtzrgqzudm.html

PHP:  $s === strrev($s);
来源：http://hz.jqgfzy.top/gtkjjsudkm.html

JS:   s === [...s].reverse().join("")
来源：http://hz.shuidangran.top/gtgrvryekf.html

TS:   s === [...s].reverse().join("")
来源：http://hz.wangshuangyany.cn/gtpwtwijxx.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.zhoulong.xyz/gttptgrxze.html

Go:   // 双指针从两端比较
来源：http://hz.dianchejie.cn/gttiuljxum.html

Ruby: s == s.reverse
来源：http://hz.shzxlz.cn/gtknytvdzw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.guowangkeji.top/gtpfylnumi.html

[N07] 两数之和（返回下标）
来源：http://hz.nanxuanxn.top/gtgpypufkh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.nwbrower.top/gtmagmkacc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.jlsjyb.cn/gtzyftzkzp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.gogol.net.cn/gtuhurdqiz.html

TS:   // 手写 Map<string, number>
来源：http://hz.yangfankeji.com/gtidxxwjia.html

Java: // 手写 HashMap
来源：http://hz.nanxinkj.top/gtqbqaracc.html

Go:   // 手写 map[int]int
来源：http://hz.yj202588.top/gtvbmfywfe.html

Ruby: // 手写 Hash
来源：http://hz.dashuyun.cn/gtrgajjxqc.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.hysaishi.cn/gtorwzvgxf.html

[N08] 生成全排列
来源：http://hz.hammf.cn/gtklyfplvg.html

Py:   itertools.permutations(arr)
来源：http://hz.jianghu66.top/gtfiecihzp.html

PHP:  // 手写递归交换
来源：http://hz.tanke756.top/gtecptyifn.html

JS:   // 手写回溯递归
来源：http://hz.dianchejie.cn/gtrbdjgdyn.html

TS:   // 手写回溯递归
来源：http://hz.dashuyun.cn/gthsbbffsc.html

Java: // 手写回溯递归
来源：http://hz.wangdashe.top/gtkvrgjsoz.html

Go:   // 手写回溯递归
来源：http://hz.smart0.xyz/gtmlelguwp.html

Ruby: arr.permutation.to_a
来源：http://hz.dashuyun.cn/gtimpzqomu.html

C#:   // 手写回溯递归
来源：http://hz.zhengqikj.top/gtghoidxlc.html

[N09] 栈与队列
来源：http://hz.haohaochexian.top/gtuwxearjo.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.guannengcc.top/gthblzgwcs.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.yongpay.top/gteduvgccl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.xinyue.icu/gtupasendf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yuanzhike.top/gtyuifhbce.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.hfpthk.cn/gtthwdffiz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.cdnleiting.top/gtyjracbsa.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.52xcode.cn/gtojdxnneu.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yj20258.top/gtkuzgixzd.html

[N10] 链表节点定义
来源：http://hz.wangdashe.top/gtaovyucsw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.svipenyu.cn/gtdicxoqvc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.c1oappe.top/gtwuvfgyhv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.gogol.net.cn/gtmympuiyo.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.guowangkeji.top/gtmqepgcwm.html

Java: class Node { int v; Node next; }
来源：http://hz.quarkkingdee.top/gthlaiioyt.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.zhongyouzk.top/gtezrpawin.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.quarkkingdee.top/gtdicjrjpi.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.hnxiangtu.top/gtdlpjakjp.html

[N11] 二叉树中序遍历
来源：http://hz.jinqigufen.top/gtpyvqsptc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.yuxming.cn/gtssczwwua.html

PHP:  // 手写递归函数
来源：http://hz.c1oappe.top/gtkonsekje.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.pycfn.com/gtkvtyrhdq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.tianlin.xyz/gtkrxkhjme.html

Java: // 手写递归
来源：http://hz.tianlin.xyz/gtirhhudpu.html

Go:   // 手写递归
来源：http://hz.xylfe.cn/gtxpoyzqyu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.ydjk.org.cn/gtsodzusjj.html

C#:   // 手写递归
来源：http://hz.jqgufenzy.top/gtqcpzoiri.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.9152youxi.cn/gtrtiezmjh.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.sufxvd.cn/gtikavjfmc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.ydzc1.top/gtxixoqunj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.wangdashe.top/gttobwrdcv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yuxming.cn/gtfhrscfmi.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yj202588.top/gtnnjigxek.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.ydzc1.top/gtghbehrzv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.yueranfly.top/gtjxmfhtjy.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xingfuxueyuan.xyz/gtniqqsjir.html

================================================================================
来源：http://hz.birdmap.top/gtbrfcskwu.html

O. 并发与异步
来源：http://hz.chenzaomai.com/gtltbfpiaf.html

================================================================================
来源：http://hz.andypj.xyz/gtqxehcgfo.html

[O01] 启动一个线程
来源：http://hz.jiagoushi.top/gtfzujxaoo.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.jqgufenzy.top/gtnuubotjn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.52xcode.cn/gtapifyugz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.hongshengwenyu.top/gtzurvwxjp.html

TS:   // 同 JS
来源：http://hz.jianghu66.top/gtgkzqiscj.html

Java: new Thread(() -> f()).start()
来源：http://hz.hfpthk.cn/gtjyljlafq.html

Go:   go f()
来源：http://hz.shangyingyoupin.top/gtssdxbytt.html

Ruby: Thread.new { f }
来源：http://hz.chenlongwang.top/gtqiwjslrb.html

C#:   Task.Run(() => F());
来源：http://hz.chenlongwang.top/gtktjfkjjj.html

[O02] 使用线程池
来源：http://hz.gzhubu.top/gtvfhfuoaa.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.meibo888.top/gtbrhbxhrz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.zhijiandao.cn/gtlkxkjrpq.html

JS:   // worker_threads 线程池
来源：http://hz.chenzaomai.com/gtnrfwgqca.html

TS:   // worker_threads 线程池
来源：http://hz.snrcjt.cn/gttllmffkc.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.zhiwuduotai.top/gtscvviqak.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.shanyushiyangkeji.top/gtbbweishz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.chenjidiqi.icu/gtvjnwkxor.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.jinqigfzy.top/gtrsjcflnk.html

[O03] 加锁保护共享数据
来源：http://hz.xziqi.cn/gtzjlyfpdq.html

Py:   with lock: shared += 1
来源：http://hz.zhixingplan.top/gtkyypsssx.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.jqgufenzy.top/gtzaciyobe.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.cheryme.top/gtohpwqyqj.html

TS:   // 同 JS
来源：http://hz.quarkkingdee.top/gtvvjnopco.html

Java: synchronized (this) { shared++; }
来源：http://hz.zhaomingkeji.xyz/gtvcgbymya.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.zhengqikj.top/gtzciyzlpe.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.sufxvd.cn/gtwezrbcfp.html

C#:   lock (gate) { shared++; }
来源：http://hz.ybcxt.top/gtggeoclsm.html

[O04] 定义异步函数并等待
来源：http://hz.gzhubu.top/gtwmzafoeq.html

Py:   async def f():⏎    await g()
来源：http://hz.chenlongwang.top/gtpydmeqyg.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.sxryk.cn/gtnijialwc.html

JS:   async function f() { await g(); }
来源：http://hz.jiagoushi.top/gtxnlryngt.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yueranfly.top/gtxltgzugr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.yuanzhike.top/gtyypavdpu.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.cashguo.top/gttwkarzei.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.quarkkingdee.top/gtnvpmrzzy.html

C#:   async Task F() { await G(); }
来源：http://hz.yonumen.top/gtxdgwmolc.html

[O05] 并发执行并等待全部完成
来源：http://hz.tian-w.cn/gtmmmiumem.html

Py:   asyncio.gather(*tasks)
来源：http://hz.xuanzx.com/gtgqifdpfq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.yongpay.top/gtcpbtmdgc.html

JS:   await Promise.all(tasks)
来源：http://hz.mhx1999.top/gtmkvfgwar.html

TS:   await Promise.all(tasks)
来源：http://hz.havefunace.top/gtanyqofgt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.iojbl.cn/gtcjcnyqxw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.haohaochexian.top/gtyvvywzyo.html

Ruby: threads.map(&:join)
来源：http://hz.zycfv.cn/gtlwzgffaf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.aibaodan.cn/gtzwcaizsq.html

[O06] 使用进程池
来源：http://hz.ydzc1.top/gtxqvcwvsh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.aizwys.cn/gtiwqfyisc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.yangfankeji.com/gtkoepaslq.html

JS:   // child_process / cluster 模块
来源：http://hz.ydzc1.top/gtttszrhqn.html

TS:   // child_process / cluster 模块
来源：http://hz.hnqzz.top/gtitymlebb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jinqigfzy.top/gtehzrzuct.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.xuanzx.com/gtbgeqqeeb.html

Ruby: // fork 块
来源：http://hz.ybcxt.top/gtsvoaqtxu.html

C#:   Parallel.For
来源：http://hz.chenjidiqi.icu/gtnbraahtt.html

================================================================================
来源：http://hz.yj20258.top/gtxftkwyst.html

P. 常用工具函数
来源：http://hz.shzxlz.cn/gtfqywjtvl.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtsueitgan.html

[P01] 生成 UUID
来源：http://hz.smart0.xyz/gtjrzyxeqs.html

Py:   str(uuid.uuid4())
来源：http://hz.52xcode.cn/gtddbtttih.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yonumen.top/gtegwpjnax.html

JS:   crypto.randomUUID()
来源：http://hz.feifeiyinyue.top/gtrqterotb.html

TS:   crypto.randomUUID()
来源：http://hz.ydjk.org.cn/gtefowmzgl.html

Java: UUID.randomUUID().toString()
来源：http://hz.ydjk.org.cn/gtzndatyft.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yuxming.cn/gtzlqmomcb.html

Ruby: SecureRandom.uuid
来源：http://hz.yueranfly.top/gtxzvfhhdw.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.ybcxt.top/gtcbpnbqkp.html

[P02] MD5 / SHA256 摘要
来源：http://hz.zhaomingkeji.xyz/gtmhwcpvie.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.sufxvd.cn/gtxmebeqha.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.0kj1m.cn/gtxbwiuqof.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.pycfn.com/gtolvetgbm.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.sysykeji.top/gtxdpotaoa.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.yonumen.top/gtcmhmfyqy.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.mhx1999.top/gtrdfsqcrq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.sweek.top/gtprwvvlnk.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.xylfe.cn/gtxyitbala.html

[P03] 生成短随机字符串
来源：http://hz.nanxuanxn.top/gtyildqdif.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.hnqzz.top/gtcanqpzdk.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.zdqjudy.top/gttutrkalw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.shzxlz.cn/gtzmexdpak.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ybcxt.top/gtphaarypr.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.hongshengwenyu.top/gtpmsjevsv.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.quarkkingdee.top/gtbmhrfkir.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.hammf.cn/gtyaesxtbw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.wangshuangyany.cn/gtyzdoqohq.html

[P04] 求长度
来源：http://hz.yj20258.top/gtaprgeelp.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.zdqjudy.top/gtoqnhauvo.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhiwuduotai.top/gtdpmtbzxc.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.shzxlz.cn/gtdhuvoejn.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hnxiangtu.top/gtoaabmsck.html

Java: list.size();  map.size();  s.length()
来源：http://hz.quarkkingdee.top/gtgwnrndjp.html

Go:   len(arr);  len(m)
来源：http://hz.jianghu66.top/gtgjsvwxgb.html

Ruby: x.length;  x.size
来源：http://hz.sweek.top/gtqlfljxop.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.xuanzx.com/gtrstyczut.html

[P05] 判断两个对象内容是否相等
来源：http://hz.gotoacloud.top/gtbxafuqwe.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.shangyingyoupin.top/gtpwidnvoa.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.ybcxt.top/gtqpkktsgu.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.jinqigfzy.top/gterswsrub.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.daxiang520.top/gtjxsdvixv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.0kj1m.cn/gterqnjhsm.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yuanzhike.top/gtltoxagav.html

Ruby: a == b
来源：http://hz.dashuyun.cn/gtkyessbre.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.ivvv.top/gtsvbxzhhs.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.hongshengwenyu.top/gtfshnmeic.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.fengsongda.top/gtbuygexvj.html

PHP:  if (empty($x)) {}
来源：http://hz.shanyushiyangtech.top/gtdlyxuhrm.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.hnqzz.top/gtslrdhwkv.html

TS:   if (x == null) {}
来源：http://hz.zhongyouzk.top/gtqxaeggrx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.xinyue.icu/gtsfrmhadf.html

Go:   if x == nil {}
来源：http://hz.yangfankeji.com/gtjiexcmdk.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.sxryk.cn/gthrtytghz.html

C#:   if (x is null) {}
来源：http://hz.sxryk.cn/gtkrenoaif.html

[P07] 防抖与节流
来源：http://hz.0kj1m.cn/gtlzkcmakf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.dashuyun.cn/gthljiqxxi.html

PHP:  // 手写时间戳比较
来源：http://hz.hnxiangtu.top/gtgqgblrhc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.bjfxy.top/gtkedwttqj.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ivvv.top/gtmucqytky.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.gogol.net.cn/gtdvuphbto.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.yanxiufei.cn/gtpldcvhbg.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yj202588.top/gtfcpscdyl.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.jqgfzy.top/gtmabtzhcl.html

[P08] 处理浮点精度问题
来源：http://hz.xuanzx.com/gtyknvleda.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.hywenlv.cn/gtprtsetog.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.xylfe.cn/gtdlvbkwbq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.sufxvd.cn/gtiuguqcnw.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.yanxiufei.cn/gtvgywoaog.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.zhoulong.xyz/gtvsvmxwry.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.kuanghao11.cn/gtklzzcuht.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.gaohongyu789.top/gtkqwbhuwb.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.zhengqikj.top/gtbsiqxpca.html

================================================================================
来源：http://hz.jianghu66.top/gtqerxhwsn.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.zhaomingkeji.xyz/gtszbxerom.html

================================================================================
来源：http://hz.cheryme.top/gtzlxbkaaz.html

[Q01] 创建表
来源：http://hz.c1oappe.top/gtoxlsgffc.html

CREATE TABLE users (
来源：http://hz.kuanghao11.cn/gtxluctgii.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.guowangkeji.top/gtkpibeyln.html

name VARCHAR(50) NOT NULL,
来源：http://hz.sysykeji.top/gtjcjugnfx.html

email VARCHAR(100) UNIQUE,
来源：http://hz.guowangkeji.top/gtzihigthx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.ivvv.top/gtjpzselmo.html

);
来源：http://hz.ydzc1.top/gtbhkxyqwr.html

[Q02] 创建带外键的表
来源：http://hz.yangfankeji.com/gtivlbzqls.html

CREATE TABLE orders (
来源：http://hz.xuetiantiany.cn/gtqaiiyqda.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.0kj1m.cn/gtxjshedjb.html

user_id INT NOT NULL,
来源：http://hz.wangshuangyany.cn/gttgqrwsup.html

amount DECIMAL(10, 2),
来源：http://hz.zhongyouzk.top/gtwudjscks.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.gaohongyu789.top/gtawhxfzyl.html

);
来源：http://hz.fzhhl.top/gtnmerohrt.html

[Q03] 增加列
来源：http://hz.zhoulong.xyz/gtzfbpjltf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.gzhubu.top/gtzzzcmlgu.html

[Q04] 修改列类型
来源：http://hz.shzxlz.cn/gtzhcmqdsl.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.ehwqpu.com/gtssgmaeix.html

[Q05] 重命名列
来源：http://hz.svipenyu.cn/gtbmrplpzp.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.iojbl.cn/gtzuinhrag.html

[Q06] 删除列
来源：http://hz.nanxuanxn.top/gtnfmmnwsk.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.jinyuanbaomall.cn/gtdcxshctr.html

[Q07] 删除表
来源：http://hz.kuanghao11.cn/gtsjizswue.html

DROP TABLE IF EXISTS orders;
来源：http://hz.ydjk.org.cn/gtfkcjlnwk.html

[Q08] 创建普通索引
来源：http://hz.xingfuxueyuan.xyz/gtrwzxhdtk.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.kuanghao11.cn/gtzssediyi.html

[Q09] 创建唯一索引
来源：http://hz.jinqigfzy.top/gtefdxldhx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.chenzaomai.com/gtxsybifmp.html

[Q10] 插入单行
来源：http://hz.fzhhl.top/gtwmmpztxe.html


<!-- 参考信息 -->