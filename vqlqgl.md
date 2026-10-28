代发 wailian999

Java: public static void main(String[] args)
来源：http://hz.ehwqpu.com/gtyzchuyzg.html

Go:   func main()
来源：http://hz.jianghu66.top/gtezswaqxm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.cdnleiting.top/gtywwacfxq.html

C#:   static void Main(string[] args)
来源：http://hz.316326.xyz/gttgqljvpu.html

[M08] 获取系统与运行时信息
来源：http://hz.daxiang520.top/gtfdnlotsx.html

Py:   platform.system();  platform.python_version()
来源：http://hz.shanyushiyangkeji.top/gtnwycanwa.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.andypj.xyz/gtcpizhmwy.html

JS:   process.platform;  process.version
来源：http://hz.gogol.net.cn/gtattxpsea.html

TS:   process.platform;  process.version
来源：http://hz.ydzc1.top/gttplvdira.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.fengsongda.top/gtvqtzkcim.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.havefunace.top/gtcrkvbpil.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.aibaodan.cn/gtfjohochd.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.zdqjudy.top/gtkcqshjjk.html

================================================================================
来源：http://hz.zhijiandao.cn/gtxsvzrjwv.html

N. 数据结构与算法
来源：http://hz.gogol.net.cn/gtzbgdwfmd.html

================================================================================
来源：http://hz.guannengcc.top/gtttrtntsq.html

[N01] 二分查找（有序数组）
来源：http://hz.yonumen.top/gtqybhpway.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.nwbrower.top/gtsgieajkd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yj20258888.top/gtjkjytrhp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yj20258888.top/gtohwnswxv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yj20258888.top/gtbuwxlncz.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.jinyuanbaomall.cn/gtwnkrnldi.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jinyuanbaomall.cn/gtwmtgckji.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.birdmap.top/gteeasselb.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.xylfe.cn/gtnfzmitwj.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.tianlin.xyz/gtvxaamvlf.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.sweek.top/gtcgjtpygn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jianghu66.top/gtqdtgbrfu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.iojbl.cn/gtqicbatxo.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.sufxvd.cn/gtncenjqbv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.gaohongyu789.top/gtmulmqtmn.html

Go:   slices.Sort(arr)
来源：http://hz.shzxlz.cn/gtjzkmyfhs.html

Ruby: arr.sort
来源：http://hz.svipenyu.cn/gtbrpozewz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.jinghuilouyu.cn/gtruhmopxc.html

[N03] 快速排序（分治示例）
来源：http://hz.xziqi.cn/gtgivrsgdy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.haohaochexian.top/gtlgmztxef.html

PHP:  // 递归实现，或用 usort
来源：http://hz.ywan-chungtsiang.top/gtrwkuxcgn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hammf.cn/gtedmocmdl.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hongshengwenyu.top/gthphmfbfz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.shuidangran.top/gtnbaroytb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yj20258888.top/gthachvnon.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.svipenyu.cn/gtgtqbtqov.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.ydjk.org.cn/gtufmafunc.html

[N04] 斐波那契数列
来源：http://hz.tanke756.top/gtxriinyxe.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.sweek.top/gtlcepuwpw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.redwolf501.top/gtfafifpbb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yangfankeji.com/gttjdrcesz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.gotoacloud.top/gtrbjtfsme.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.bjfxy.top/gtjzdkjvwa.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yonumen.top/gtlmzrfnef.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.fengsongda.top/gtrtammzqu.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.cdnleiting.top/gthzrshegh.html

[N05] 最大公约数
来源：http://hz.quarkkingdee.top/gtffexkmdg.html

Py:   math.gcd(a, b)
来源：http://hz.cashguo.top/gtzhamrafy.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.birdmap.top/gtpwelzidy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hongshengwenyu.top/gtqtocfpci.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.sxryk.cn/gtifccjfdu.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.xuetiantiany.cn/gtawzjipgu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.xylfe.cn/gtxupsccct.html

Ruby: a.gcd(b)
来源：http://hz.jinqigufen.top/gtijfqixwg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yj20258.top/gtclkvgexi.html

[N06] 判断回文字符串
来源：http://hz.xinyue.icu/gttuufbftp.html

Py:   s == s[::-1]
来源：http://hz.c1oappe.top/gtrzbprtqx.html

PHP:  $s === strrev($s);
来源：http://hz.zhongyouzk.top/gtfqcedbhz.html

JS:   s === [...s].reverse().join("")
来源：http://hz.ehwqpu.com/gtenlflaic.html

TS:   s === [...s].reverse().join("")
来源：http://hz.hnqzz.top/gtvgyyekoq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.yvedp.cn/gtikadwcpb.html

Go:   // 双指针从两端比较
来源：http://hz.hywenlv.cn/gtagqkfhpv.html

Ruby: s == s.reverse
来源：http://hz.havefunace.top/gtmgwpsbwg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.jlsjyb.cn/gtdirhgzrt.html

[N07] 两数之和（返回下标）
来源：http://hz.nanxuanxn.top/gtzrwiskrg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.aizwys.cn/gtyijlyuhb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.xingfuxueyuan.xyz/gthqirddsv.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.zhixingplan.top/gtvixuwnsm.html

TS:   // 手写 Map<string, number>
来源：http://hz.vqdsnc.cn/gtzhfxzzlx.html

Java: // 手写 HashMap
来源：http://hz.gogol.net.cn/gtkdvbdpdp.html

Go:   // 手写 map[int]int
来源：http://hz.smart0.xyz/gtrvwbtkyi.html

Ruby: // 手写 Hash
来源：http://hz.nanxuanxn.top/gtqwxndbrs.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.shanyushiyangtech.top/gtcuitzzyn.html

[N08] 生成全排列
来源：http://hz.yj20258888.top/gtgnrovtbd.html

Py:   itertools.permutations(arr)
来源：http://hz.yj20258888.top/gtsihiykzb.html

PHP:  // 手写递归交换
来源：http://hz.316326.xyz/gtsnnyojlx.html

JS:   // 手写回溯递归
来源：http://hz.9152youxi.cn/gtjnenoail.html

TS:   // 手写回溯递归
来源：http://hz.hysaishi.cn/gtoyvcpytw.html

Java: // 手写回溯递归
来源：http://hz.daria6918.cn/gtdhhwuytw.html

Go:   // 手写回溯递归
来源：http://hz.chenlongwang.top/gtlgfxpifw.html

Ruby: arr.permutation.to_a
来源：http://hz.ppjwa.cn/gtqfzwjyuw.html

C#:   // 手写回溯递归
来源：http://hz.ehwqpu.com/gtdubfegxd.html

[N09] 栈与队列
来源：http://hz.dianchejie.cn/gtirtstjgb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.sxryk.cn/gtelnjvtul.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.zhaomingkeji.xyz/gtfootlxlb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.xuanzx.com/gtavzgrdrj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.chenjidiqi.icu/gtjawtnyby.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.shzxlz.cn/gtrlmqievq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.iojbl.cn/gtpikrzstb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.jinqigfzy.top/gtrxxkfayo.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.xuetiantiany.cn/gtkfbeydae.html

[N10] 链表节点定义
来源：http://hz.yonumen.top/gtnjnmlnhn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.wangshuangyany.cn/gtthpaesbs.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.cucudq.cn/gtjksejbhf.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.hammf.cn/gtlynzzyct.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.yj202588.top/gtkxvxpgyh.html

Java: class Node { int v; Node next; }
来源：http://hz.jlsjyb.cn/gtjekrkgeu.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.zycfv.cn/gtleuaeeke.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.yangfankeji.com/gtomgclehg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.jinghuilouyu.cn/gtdeflbbpf.html

[N11] 二叉树中序遍历
来源：http://hz.xuanzx.com/gtchkfzkic.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.shanyushiyangtech.top/gtsstistaj.html

PHP:  // 手写递归函数
来源：http://hz.tianlin.xyz/gtafcsaaqy.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jlsjyb.cn/gtqofokdyp.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yj20258888.top/gtufzoydcn.html

Java: // 手写递归
来源：http://hz.cqqwz.cn/gtipmfnxjl.html

Go:   // 手写递归
来源：http://hz.shzxlz.cn/gtazyaziaw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.feifeiyinyue.top/gtfdnnjhol.html

C#:   // 手写递归
来源：http://hz.jinyuanbaomall.cn/gteorwgdyc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.xziqi.cn/gtjclmlkhh.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.gotoacloud.top/gttlmymtrk.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.gotoacloud.top/gtndvidqbf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xuanzx.com/gtxiqjopvf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jqgfzy.top/gtsdpkaunm.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.gotoacloud.top/gtgxjoosbg.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.sysykeji.top/gtxjjxzziq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.yj202588.top/gtahdykckc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.shzxlz.cn/gtjawxpghg.html

================================================================================
来源：http://hz.hfpthk.cn/gtladepulq.html

O. 并发与异步
来源：http://hz.zycfv.cn/gtulntkeov.html

================================================================================
来源：http://hz.birdmap.top/gtjhfomrcd.html

[O01] 启动一个线程
来源：http://hz.gaohongyu789.top/gtppoggizt.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.nanxinkj.top/gtsdgrjgab.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.zhongyouzk.top/gtcuoftrnn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.cdnleiting.top/gtevcikvij.html

TS:   // 同 JS
来源：http://hz.zhixingplan.top/gtouzltokk.html

Java: new Thread(() -> f()).start()
来源：http://hz.wangshuangyany.cn/gtzcygodkt.html

Go:   go f()
来源：http://hz.zhoulong.xyz/gtzsnuaior.html

Ruby: Thread.new { f }
来源：http://hz.nwbrower.top/gtzuuipcri.html

C#:   Task.Run(() => F());
来源：http://hz.jqgfzy.top/gtgalwfhmb.html

[O02] 使用线程池
来源：http://hz.cqqwz.cn/gtnsrqevgc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yj20258.top/gtwxwkzpna.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.9152youxi.cn/gtrofombxg.html

JS:   // worker_threads 线程池
来源：http://hz.yuxming.cn/gtmnykwnjc.html

TS:   // worker_threads 线程池
来源：http://hz.jlsjyb.cn/gtugifhrxo.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.nwbrower.top/gtefsjcpzc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.xingfuxueyuan.xyz/gtixkpbinu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.shangyingyoupin.top/gtmalczwkg.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.xuanzx.com/gtolzuajfy.html

[O03] 加锁保护共享数据
来源：http://hz.jqgfzy.top/gtjolbpowu.html

Py:   with lock: shared += 1
来源：http://hz.tanke756.top/gtowhcikia.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.sufxvd.cn/gtnnxptunc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.pycfn.com/gtvryvrphq.html

TS:   // 同 JS
来源：http://hz.jiagoushi.top/gtleztoquk.html

Java: synchronized (this) { shared++; }
来源：http://hz.zycfv.cn/gtwlbndnku.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.smart0.xyz/gtuiusejsk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.zhoulong.xyz/gtaxvwipny.html

C#:   lock (gate) { shared++; }
来源：http://hz.yuxming.cn/gtrwefscnz.html

[O04] 定义异步函数并等待
来源：http://hz.gzhubu.top/gtpjlrsttk.html

Py:   async def f():⏎    await g()
来源：http://hz.bjfxy.top/gtxmfmovsr.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.shanyushiyangkeji.top/gtvmhizjon.html

JS:   async function f() { await g(); }
来源：http://hz.dianchejie.cn/gtwaibqhlb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.cdnleiting.top/gtkxrnmlzn.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.sxryk.cn/gthcswoqdw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.wangdashe.top/gtpuvyfuri.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.smart0.xyz/gtitmggmtg.html

C#:   async Task F() { await G(); }
来源：http://hz.9152youxi.cn/gtvjihvbzt.html

[O05] 并发执行并等待全部完成
来源：http://hz.xuetiantiany.cn/gtdjlwubuj.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jqgfzy.top/gthppmmxwy.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.ydjk.org.cn/gtcbbhfhlg.html

JS:   await Promise.all(tasks)
来源：http://hz.9152youxi.cn/gtzfwxojzn.html

TS:   await Promise.all(tasks)
来源：http://hz.dashuyun.cn/gtxyarewas.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.snrcjt.cn/gtoicctslf.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.jiagoushi.top/gtbkgmrnia.html

Ruby: threads.map(&:join)
来源：http://hz.mhx1999.top/gtngotnbiw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.tanke756.top/gtvrlghzvw.html

[O06] 使用进程池
来源：http://hz.ywan-chungtsiang.top/gtltatoili.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.yanxiufei.cn/gtpmsnufkt.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.hnxiangtu.top/gtdnvdcskg.html

JS:   // child_process / cluster 模块
来源：http://hz.cheryme.top/gtloempgzj.html

TS:   // child_process / cluster 模块
来源：http://hz.xuanzx.com/gtvfgmetkf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.chenzaomai.com/gtxylffuzg.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.xingfuxueyuan.xyz/gtvfnkpxnt.html

Ruby: // fork 块
来源：http://hz.dashuyun.cn/gtxlqolzad.html

C#:   Parallel.For
来源：http://hz.havefunace.top/gtqozpwebw.html

================================================================================
来源：http://hz.9152youxi.cn/gtzbdgbrfe.html

P. 常用工具函数
来源：http://hz.shzxlz.cn/gtujzvldxg.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtgkvvrdjj.html

[P01] 生成 UUID
来源：http://hz.vqdsnc.cn/gtaepsxcex.html

Py:   str(uuid.uuid4())
来源：http://hz.pengpengdd.cyou/gtwrrckvub.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jinqigfzy.top/gtlxmryhxj.html

JS:   crypto.randomUUID()
来源：http://hz.xingfuxueyuan.xyz/gthqduiwok.html

TS:   crypto.randomUUID()
来源：http://hz.vqdsnc.cn/gtkxwbwjul.html

Java: UUID.randomUUID().toString()
来源：http://hz.316326.xyz/gtbjcriqxg.html

Go:   // 用 github.com/google/uuid
来源：http://hz.chenjidiqi.icu/gtvtqwgjwb.html

Ruby: SecureRandom.uuid
来源：http://hz.birdmap.top/gtlrjxtxvx.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.shuidangran.top/gtsghmfeoq.html

[P02] MD5 / SHA256 摘要
来源：http://hz.xuanzx.com/gtyzxftpqy.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.jianghu66.top/gtqdhjdwua.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.zhixingplan.top/gtuksayfho.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.nwbrower.top/gtzlctywez.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jyoumei.cn/gtlgkvbntb.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.zdqjudy.top/gtsxwthodz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.0kj1m.cn/gttavsvpiv.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.svipenyu.cn/gtaquhlxxx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.xingfuxueyuan.xyz/gthedixiha.html

[P03] 生成短随机字符串
来源：http://hz.fzhhl.top/gtayksgjgc.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.gaohongyu789.top/gtzndfelyh.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.svipenyu.cn/gtzqwrgurh.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhongyouzk.top/gtoizzxaph.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jinghuilouyu.cn/gtivvoadxl.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.snrcjt.cn/gtjivrjzfh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.zdqjudy.top/gtiwrdfxze.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jinqigfzy.top/gtokptlxcv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.hywenlv.cn/gtnoddptsn.html

[P04] 求长度
来源：http://hz.andypj.xyz/gtntucfwbb.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.yuxming.cn/gtuwazuriu.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zdqjudy.top/gtmaaudkcz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.daria6918.cn/gtixadbhiq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.sweek.top/gtzquapove.html

Java: list.size();  map.size();  s.length()
来源：http://hz.hammf.cn/gtidamkgir.html

Go:   len(arr);  len(m)
来源：http://hz.nwbrower.top/gtggdcletg.html

Ruby: x.length;  x.size
来源：http://hz.xuanzx.com/gtpomqbbaq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.tianlin.xyz/gtpkhoxtll.html

[P05] 判断两个对象内容是否相等
来源：http://hz.jinyuanbaomall.cn/gtyqugahqt.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.xylfe.cn/gtzpupxmzq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.nwbrower.top/gtgatdiowi.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.nanxinkj.top/gtadokfcck.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.316326.xyz/gtkwerhhxo.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.hywenlv.cn/gtfsklievj.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yangfankeji.com/gtzfamewrf.html

Ruby: a == b
来源：http://hz.vqdsnc.cn/gtbuckaojb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.hnqzz.top/gtvhpjrhbe.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.yuxming.cn/gtwgbytlse.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.ybcxt.top/gtopuclaop.html

PHP:  if (empty($x)) {}
来源：http://hz.cheryme.top/gtvqpnexwd.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jinghuilouyu.cn/gtoxhlatwd.html

TS:   if (x == null) {}
来源：http://hz.shanyushiyangkeji.top/gtopmgsqup.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.jlsjyb.cn/gtlxvupbrn.html

Go:   if x == nil {}
来源：http://hz.jinqigufen.top/gtgmvcgypy.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.yj20258.top/gtpbdulnuc.html

C#:   if (x is null) {}
来源：http://hz.zycfv.cn/gtxkfuabko.html

[P07] 防抖与节流
来源：http://hz.jlsjyb.cn/gtorythurc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jyoumei.cn/gtgjzzvffl.html

PHP:  // 手写时间戳比较
来源：http://hz.yj202588.top/gtoahexhme.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ybcxt.top/gtdvrndphw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hongshengwenyu.top/gtekhgalaq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.52xcode.cn/gtgvvoyvvm.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.yangfankeji.com/gtlrsnynye.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.gotoacloud.top/gtvdqzfeqk.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.guowangkeji.top/gthxlclrfs.html

[P08] 处理浮点精度问题
来源：http://hz.aizwys.cn/gthiavzgwu.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.ydzc1.top/gtpxuthmfn.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.kuanghao11.cn/gtwmotavwy.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.haohaochexian.top/gtegshylqg.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.andypj.xyz/gtixzmywca.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.chenzaomai.com/gtatjpamww.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.jlsjyb.cn/gtmxywdwjg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.nanxuanxn.top/gtbmkqdlod.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.gzhubu.top/gtiaavbnfz.html

================================================================================
来源：http://hz.redwolf501.top/gtcltyzixa.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.bjfxy.top/gtirztziku.html

================================================================================
来源：http://hz.cdnleiting.top/gtwbwpscrm.html

[Q01] 创建表
来源：http://hz.guannengcc.top/gtcmfeeixm.html

CREATE TABLE users (
来源：http://hz.zhengqikj.top/gtthfwvjpb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jianghu66.top/gtpopbofmj.html

name VARCHAR(50) NOT NULL,
来源：http://hz.vqdsnc.cn/gtfnhscczn.html

email VARCHAR(100) UNIQUE,
来源：http://hz.kuanghao11.cn/gtwusiswfx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.gaohongyu789.top/gttmnlukcf.html

);
来源：http://hz.shanyushiyangtech.top/gtkuwtjcys.html

[Q02] 创建带外键的表
来源：http://hz.xuanzx.com/gtbmjkbmpe.html

CREATE TABLE orders (
来源：http://hz.xuetiantiany.cn/gtsffmxsuq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hnxiangtu.top/gtlmzzwmae.html

user_id INT NOT NULL,
来源：http://hz.nanxinkj.top/gtmltljrda.html

amount DECIMAL(10, 2),
来源：http://hz.chenzaomai.com/gtzeabbscp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.chenjidiqi.icu/gtdgvyoerx.html

);
来源：http://hz.yj20258.top/gtmpijlwfl.html

[Q03] 增加列
来源：http://hz.shzxlz.cn/gtmodkajeh.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.daxiang520.top/gtpbnzjpru.html

[Q04] 修改列类型
来源：http://hz.52xcode.cn/gtlpwkeqzn.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.jyoumei.cn/gtdvjrkjil.html

[Q05] 重命名列
来源：http://hz.yueranfly.top/gtnfxsufmp.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.zhijiandao.cn/gtipmisypw.html

[Q06] 删除列
来源：http://hz.316326.xyz/gtstsxqpwh.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.ehwqpu.com/gtqammwwua.html

[Q07] 删除表
来源：http://hz.cashguo.top/gtpciituau.html

DROP TABLE IF EXISTS orders;
来源：http://hz.xuetiantiany.cn/gtregfshnr.html

[Q08] 创建普通索引
来源：http://hz.jyoumei.cn/gtyedcvitk.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.ivvv.top/gtzjkltrqv.html

[Q09] 创建唯一索引
来源：http://hz.tian-w.cn/gtpomimier.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.zdqjudy.top/gtdtvrsvvi.html

[Q10] 插入单行
来源：http://hz.quarkkingdee.top/gtpypnglth.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.cheryme.top/gthtohwnxc.html

[Q11] 一次插入多行
来源：http://hz.jinqigufen.top/gtfpxsmecd.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.shangyingyoupin.top/gtwaueoppz.html

[Q12] 插入后取自增 ID
来源：http://hz.zhijiandao.cn/gtekgiquxt.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.snrcjt.cn/gtxzchfqaa.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.nwbrower.top/gtyxmkynrq.html

[Q13] 忽略重复插入
来源：http://hz.gotoacloud.top/gtvulorqbm.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.birdmap.top/gtgyuevhgg.html

[Q14] 存在则更新（upsert）
来源：http://hz.kuanghao11.cn/gteaighatb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.sxryk.cn/gtdmmqtvwl.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.zhongyouzk.top/gtouyewyba.html

[Q15] 查询全部
来源：http://hz.fengsongda.top/gtvyammvhh.html


<!-- 参考信息 -->