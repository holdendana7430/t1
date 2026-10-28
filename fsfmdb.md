代发 wailian999

Java: public static void main(String[] args)
来源：http://hz.316326.xyz/gtyueifidb.html

Go:   func main()
来源：http://hz.vqdsnc.cn/gthyvoalun.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.316326.xyz/gtxtxkdcnu.html

C#:   static void Main(string[] args)
来源：http://hz.dianchejie.cn/gttajvawun.html

[M08] 获取系统与运行时信息
来源：http://hz.zhiwuduotai.top/gtyamnpkgy.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yj202588.top/gttmupokdo.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yuxming.cn/gtlgpiygcy.html

JS:   process.platform;  process.version
来源：http://hz.andypj.xyz/gtkdecbqts.html

TS:   process.platform;  process.version
来源：http://hz.hysaishi.cn/gttytlknzn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.cucudq.cn/gtqhhizegu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.cucudq.cn/gtqsgoiiod.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.c1oappe.top/gtijajiyja.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.52xcode.cn/gtgaxmucqd.html

================================================================================
来源：http://hz.ehwqpu.com/gtvhcczycb.html

N. 数据结构与算法
来源：http://hz.daria6918.cn/gtkdranolv.html

================================================================================
来源：http://hz.316326.xyz/gtljsuytpf.html

[N01] 二分查找（有序数组）
来源：http://hz.cashguo.top/gtytsfaogm.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.hfpthk.cn/gtzrkufjjj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.zhijiandao.cn/gtqemyjept.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.daria6918.cn/gtfbjxyubr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ivvv.top/gtcmkxlaci.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.ydzc1.top/gtanvyufat.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.dianchejie.cn/gtazqahgno.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jinqigufen.top/gtdqhyykvx.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.aibaodan.cn/gterehuwfh.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.snrcjt.cn/gtsyqhbdxn.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yangfankeji.com/gtqhhgqnsf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.redwolf501.top/gtiuwpsjvf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.nwbrower.top/gtshojfuep.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.52xcode.cn/gtforlxdjp.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.zhiwuduotai.top/gtogyfdhnf.html

Go:   slices.Sort(arr)
来源：http://hz.yonumen.top/gtoacjhgud.html

Ruby: arr.sort
来源：http://hz.gzhubu.top/gtwfofjewi.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.zhongyouzk.top/gtpfgzcvvv.html

[N03] 快速排序（分治示例）
来源：http://hz.ybcxt.top/gtmymxiogx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.hywenlv.cn/gthurxeybs.html

PHP:  // 递归实现，或用 usort
来源：http://hz.zhongyouzk.top/gtykhtgkdl.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jinghuilouyu.cn/gtesxgkvrm.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.shuidangran.top/gtujdenoqa.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.meibo888.top/gttiswpxsj.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jianghu66.top/gttqjxbjjp.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.sysykeji.top/gthfxhuukb.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.hysaishi.cn/gtyvlcmsyq.html

[N04] 斐波那契数列
来源：http://hz.0kj1m.cn/gtgdwvfegh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.52xcode.cn/gtzmluifve.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.zhiwuduotai.top/gtpxvbxdvf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.nwbrower.top/gtcykzwjxx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.sxryk.cn/gtnhtmpgva.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.shuidangran.top/gtdozdgkab.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.redwolf501.top/gtgppszxyv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.316326.xyz/gtstkvkpri.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.xuetiantiany.cn/gtfhqylrab.html

[N05] 最大公约数
来源：http://hz.smart0.xyz/gtqhdntpjj.html

Py:   math.gcd(a, b)
来源：http://hz.jiagoushi.top/gtgmxehftl.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.shuidangran.top/gtfwnynoun.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.0kj1m.cn/gtjbqpxxcg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.shangyingyoupin.top/gtkousgluh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.52xcode.cn/gtjunxgbjc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.shanyushiyangkeji.top/gtaziavzpf.html

Ruby: a.gcd(b)
来源：http://hz.hysaishi.cn/gtpgwsuhqp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yj20258.top/gtajierovq.html

[N06] 判断回文字符串
来源：http://hz.yj20258.top/gtqnsvrmpa.html

Py:   s == s[::-1]
来源：http://hz.cdnleiting.top/gtknsgvblm.html

PHP:  $s === strrev($s);
来源：http://hz.yongpay.top/gtzbwlplam.html

JS:   s === [...s].reverse().join("")
来源：http://hz.aibaodan.cn/gtdzmkncfs.html

TS:   s === [...s].reverse().join("")
来源：http://hz.c1oappe.top/gtqpicspsg.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jinqigufen.top/gtivtaifnd.html

Go:   // 双指针从两端比较
来源：http://hz.yueranfly.top/gtyrkbyroy.html

Ruby: s == s.reverse
来源：http://hz.jinqigfzy.top/gtsbzmucfl.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.zhoulong.xyz/gtcsnxioff.html

[N07] 两数之和（返回下标）
来源：http://hz.tian-w.cn/gteekyoaml.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.xziqi.cn/gtfbcsmnhr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yuxming.cn/gtxtcxbfez.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.daria6918.cn/gtksvkhxoo.html

TS:   // 手写 Map<string, number>
来源：http://hz.daria6918.cn/gtymubshrl.html

Java: // 手写 HashMap
来源：http://hz.jyoumei.cn/gtmwsrlwxs.html

Go:   // 手写 map[int]int
来源：http://hz.yj20258.top/gtljniuolq.html

Ruby: // 手写 Hash
来源：http://hz.daxiang520.top/gtsotzvxds.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.fzhhl.top/gtxbsilcbo.html

[N08] 生成全排列
来源：http://hz.smart0.xyz/gtzadueold.html

Py:   itertools.permutations(arr)
来源：http://hz.zhoulong.xyz/gtfyzxzcis.html

PHP:  // 手写递归交换
来源：http://hz.sxryk.cn/gtebijudcc.html

JS:   // 手写回溯递归
来源：http://hz.ppjwa.cn/gtirjntxhs.html

TS:   // 手写回溯递归
来源：http://hz.yj20258.top/gtswegmfht.html

Java: // 手写回溯递归
来源：http://hz.cashguo.top/gtedgchkcq.html

Go:   // 手写回溯递归
来源：http://hz.9152youxi.cn/gtegrkgqtx.html

Ruby: arr.permutation.to_a
来源：http://hz.cucudq.cn/gtlvonaygx.html

C#:   // 手写回溯递归
来源：http://hz.smart0.xyz/gttqiqkxka.html

[N09] 栈与队列
来源：http://hz.316326.xyz/gtuemaqcrb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.birdmap.top/gtuikftvvc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.pycfn.com/gttewcmggr.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.jqgfzy.top/gtqzgbofpz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.quarkkingdee.top/gtdlrfcgtr.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.chenjidiqi.icu/gtwapzyjnd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.jiagoushi.top/gtwpnxcilb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.quarkkingdee.top/gtjenbghzh.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.shzxlz.cn/gtkudejiom.html

[N10] 链表节点定义
来源：http://hz.vqdsnc.cn/gtecgdnhex.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.tian-w.cn/gtguhymyak.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.hnqzz.top/gtvebnvcny.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zhiwuduotai.top/gtfmeertfd.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.vqdsnc.cn/gtrtvyclxs.html

Java: class Node { int v; Node next; }
来源：http://hz.shangyingyoupin.top/gtsbdbgxkm.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.316326.xyz/gtrpbzowmf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.quarkkingdee.top/gtbafbbagv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.jinghuilouyu.cn/gtaockztah.html

[N11] 二叉树中序遍历
来源：http://hz.aizwys.cn/gtyvexesel.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.chenlongwang.top/gtbwvcitby.html

PHP:  // 手写递归函数
来源：http://hz.yangfankeji.com/gtlgyvxhve.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ehwqpu.com/gtkjuqorux.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.aizwys.cn/gtzzduzfkh.html

Java: // 手写递归
来源：http://hz.hammf.cn/gthkhthfsx.html

Go:   // 手写递归
来源：http://hz.gzhubu.top/gtkliqqkqz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.cqqwz.cn/gtjptiifcr.html

C#:   // 手写递归
来源：http://hz.shangyingyoupin.top/gtexpgqsud.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.feifeiyinyue.top/gtiqrlowup.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.mhx1999.top/gtquqtzxtz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.zhijiandao.cn/gtnwlzsvno.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhaomingkeji.xyz/gtuvchdhvz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.quarkkingdee.top/gtkswpzyjp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ppjwa.cn/gtzlbsnlhs.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.redwolf501.top/gtuagfjkuo.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.gzhubu.top/gtsjtpuauw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xinyue.icu/gtvjwmmzps.html

================================================================================
来源：http://hz.yuxming.cn/gtwnezhniu.html

O. 并发与异步
来源：http://hz.yvedp.cn/gtvdkkqcyu.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtyunsnzam.html

[O01] 启动一个线程
来源：http://hz.aibaodan.cn/gtyjhifsrz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.jinqigfzy.top/gtzvotxuqa.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.dianchejie.cn/gtupeipnpl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.cdnleiting.top/gtdfoiywvb.html

TS:   // 同 JS
来源：http://hz.cheryme.top/gtmasdoyey.html

Java: new Thread(() -> f()).start()
来源：http://hz.fzhhl.top/gtdfjdsftn.html

Go:   go f()
来源：http://hz.jinqigfzy.top/gtphxholor.html

Ruby: Thread.new { f }
来源：http://hz.tian-w.cn/gtnnjlnwpl.html

C#:   Task.Run(() => F());
来源：http://hz.jinghuilouyu.cn/gtewythqwn.html

[O02] 使用线程池
来源：http://hz.jinqigufen.top/gtwsbdcgdm.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.jinyuanbaomall.cn/gtubyawiaq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.cashguo.top/gtvfrecret.html

JS:   // worker_threads 线程池
来源：http://hz.zhaomingkeji.xyz/gthugqsjcj.html

TS:   // worker_threads 线程池
来源：http://hz.tianlin.xyz/gtmtqfgtbf.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.hysaishi.cn/gtgexrqswv.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.fengsongda.top/gtfmasjcrq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.cheryme.top/gtnoyucfml.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.feifeiyinyue.top/gtupcfgyvq.html

[O03] 加锁保护共享数据
来源：http://hz.pengpengdd.cyou/gtevkeskgq.html

Py:   with lock: shared += 1
来源：http://hz.ywan-chungtsiang.top/gtjlnzvpge.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.cdnleiting.top/gtcvivynso.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.hfpthk.cn/gttyepnbff.html

TS:   // 同 JS
来源：http://hz.sysykeji.top/gtocvlzuda.html

Java: synchronized (this) { shared++; }
来源：http://hz.andypj.xyz/gtqzohjims.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.svipenyu.cn/gtjffsolaz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.gogol.net.cn/gtafzydgin.html

C#:   lock (gate) { shared++; }
来源：http://hz.guowangkeji.top/gtumoouyed.html

[O04] 定义异步函数并等待
来源：http://hz.hfpthk.cn/gtpqncviem.html

Py:   async def f():⏎    await g()
来源：http://hz.jiagoushi.top/gtvbufzuvo.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.sysykeji.top/gtdoxfnshe.html

JS:   async function f() { await g(); }
来源：http://hz.quarkkingdee.top/gtyusltdod.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.xingfuxueyuan.xyz/gttoewznaf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.jlsjyb.cn/gtjtprxifx.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.quarkkingdee.top/gtqkdwlexv.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yueranfly.top/gtgvoqjnvb.html

C#:   async Task F() { await G(); }
来源：http://hz.sysykeji.top/gtulppryjw.html

[O05] 并发执行并等待全部完成
来源：http://hz.tian-w.cn/gtprjnbchj.html

Py:   asyncio.gather(*tasks)
来源：http://hz.havefunace.top/gtmzzcesdv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.iojbl.cn/gtafltdnnj.html

JS:   await Promise.all(tasks)
来源：http://hz.hfpthk.cn/gtenqzdtqp.html

TS:   await Promise.all(tasks)
来源：http://hz.hywenlv.cn/gtsdgwheue.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.gotoacloud.top/gtnpsgiaoy.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.nwbrower.top/gtduxnpoap.html

Ruby: threads.map(&:join)
来源：http://hz.xziqi.cn/gtibgkskdn.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yvedp.cn/gtqeytzvqf.html

[O06] 使用进程池
来源：http://hz.guowangkeji.top/gtnzslhqsp.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.jinghuilouyu.cn/gtqnnovuus.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.zhixingplan.top/gttzdcwyql.html

JS:   // child_process / cluster 模块
来源：http://hz.chenzaomai.com/gtmysxsnge.html

TS:   // child_process / cluster 模块
来源：http://hz.yueranfly.top/gtfgmrrsrk.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.9152youxi.cn/gtiejfxcfp.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.zycfv.cn/gtxibkgwym.html

Ruby: // fork 块
来源：http://hz.chenjidiqi.icu/gtsgbalyts.html

C#:   Parallel.For
来源：http://hz.hnxiangtu.top/gtpzdortlg.html

================================================================================
来源：http://hz.fzhhl.top/gthjprjizz.html

P. 常用工具函数
来源：http://hz.haohaochexian.top/gtjudodrts.html

================================================================================
来源：http://hz.gaohongyu789.top/gtroytiaqq.html

[P01] 生成 UUID
来源：http://hz.wangshuangyany.cn/gtzckcglez.html

Py:   str(uuid.uuid4())
来源：http://hz.c1oappe.top/gtevfvrpee.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.daria6918.cn/gtedsoruzl.html

JS:   crypto.randomUUID()
来源：http://hz.zhijiandao.cn/gtzbitsqqp.html

TS:   crypto.randomUUID()
来源：http://hz.hnxiangtu.top/gtvddqeuwx.html

Java: UUID.randomUUID().toString()
来源：http://hz.yj20258.top/gtlsdzpcmv.html

Go:   // 用 github.com/google/uuid
来源：http://hz.xingfuxueyuan.xyz/gtmkvruuki.html

Ruby: SecureRandom.uuid
来源：http://hz.guannengcc.top/gtryupqjfd.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.hysaishi.cn/gtkenvvnkm.html

[P02] MD5 / SHA256 摘要
来源：http://hz.daria6918.cn/gtoehvneln.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.hywenlv.cn/gtejbarjjy.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.tianlin.xyz/gtbtdhcqwj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.nanxuanxn.top/gtsabxmjqm.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.9152youxi.cn/gtsntkpwtq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.sysykeji.top/gtzxqievij.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.zycfv.cn/gtorzwemqj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.gogol.net.cn/gthentqexg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.xinyue.icu/gtkygtuoie.html

[P03] 生成短随机字符串
来源：http://hz.jqgfzy.top/gtkuvgciry.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.yanxiufei.cn/gtkitexxup.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.tianlin.xyz/gtbkxltjte.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jyoumei.cn/gtzhiircxh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yongpay.top/gtfaqqjnbr.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.zhoulong.xyz/gtfyblvigp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yuxming.cn/gtbdxvgsau.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.yj20258.top/gtgegevyxc.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.ybcxt.top/gtsompmldk.html

[P04] 求长度
来源：http://hz.jinqigfzy.top/gttiuvytof.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.shanyushiyangtech.top/gtwskuftap.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.chenzaomai.com/gtftgzbwss.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.sweek.top/gtytaeryqc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xingfuxueyuan.xyz/gtlpkzqoma.html

Java: list.size();  map.size();  s.length()
来源：http://hz.dianchejie.cn/gtjdvqgffd.html

Go:   len(arr);  len(m)
来源：http://hz.xuetiantiany.cn/gtiztzpdyb.html

Ruby: x.length;  x.size
来源：http://hz.xinyue.icu/gtqotjufpo.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.jinqigufen.top/gtpianohra.html

[P05] 判断两个对象内容是否相等
来源：http://hz.ehwqpu.com/gtcspngkxt.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.cheryme.top/gtqaxvugrb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.bjfxy.top/gtrojyfidt.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.yuanzhike.top/gtuvgmnytp.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.chenlongwang.top/gtxmwbsqyh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.xylfe.cn/gtkwryadkg.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.fzhhl.top/gtrqgtcdwm.html

Ruby: a == b
来源：http://hz.feifeiyinyue.top/gtuzeesrdu.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.mhx1999.top/gtqzqbhutd.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.zhoulong.xyz/gtydtpqvin.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.gotoacloud.top/gttdngpcls.html

PHP:  if (empty($x)) {}
来源：http://hz.nanxinkj.top/gtrycqihug.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.tian-w.cn/gtpinrlyjt.html

TS:   if (x == null) {}
来源：http://hz.zhoulong.xyz/gtzcqzkosr.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.ydzc1.top/gtqgpzwaau.html

Go:   if x == nil {}
来源：http://hz.316326.xyz/gtxtuqhdtx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.cdnleiting.top/gtnnklanmo.html

C#:   if (x is null) {}
来源：http://hz.sweek.top/gttnksvyod.html

[P07] 防抖与节流
来源：http://hz.0kj1m.cn/gtouiqslxm.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.zhixingplan.top/gtqsiogwof.html

PHP:  // 手写时间戳比较
来源：http://hz.ehwqpu.com/gtrelsjnvc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.andypj.xyz/gtbkyxadlc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hfpthk.cn/gtceepbhej.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.hfpthk.cn/gtuzaniliw.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.nanxinkj.top/gtvhummjdo.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.guowangkeji.top/gtszzcefut.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.jyoumei.cn/gtbplzvplw.html

[P08] 处理浮点精度问题
来源：http://hz.sxryk.cn/gtfwdjiwlh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.yuxming.cn/gtmmwwbrpw.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.wangshuangyany.cn/gtadrvjmpk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.hongshengwenyu.top/gtfgbqevih.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.pycfn.com/gtitknfmod.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.gotoacloud.top/gtvupoqnyk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.xinyue.icu/gtzyeqxdsv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.yueranfly.top/gtqkgzuehb.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.zhixingplan.top/gtgbvltxgp.html

================================================================================
来源：http://hz.yangfankeji.com/gtaqhmsive.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.vqdsnc.cn/gteokjbwcb.html

================================================================================
来源：http://hz.316326.xyz/gtxbstftyp.html

[Q01] 创建表
来源：http://hz.ehwqpu.com/gtmtwxeega.html

CREATE TABLE users (
来源：http://hz.sweek.top/gtilcxmvoh.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.nanxuanxn.top/gtishsdugm.html

name VARCHAR(50) NOT NULL,
来源：http://hz.yuanzhike.top/gtucxopsaj.html

email VARCHAR(100) UNIQUE,
来源：http://hz.hongshengwenyu.top/gtsgwzqhnj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.ywan-chungtsiang.top/gtwbftgkdl.html

);
来源：http://hz.vqdsnc.cn/gtxlhuetxn.html

[Q02] 创建带外键的表
来源：http://hz.wangshuangyany.cn/gtbhzbxvec.html

CREATE TABLE orders (
来源：http://hz.fengsongda.top/gthremvhib.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.shanyushiyangkeji.top/gtrmskguux.html

user_id INT NOT NULL,
来源：http://hz.xinyue.icu/gtnwrhammf.html

amount DECIMAL(10, 2),
来源：http://hz.yueranfly.top/gtriqfwach.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.shangyingyoupin.top/gtsygzttrn.html

);
来源：http://hz.zhaomingkeji.xyz/gtocjxaasx.html

[Q03] 增加列
来源：http://hz.chenlongwang.top/gtrnqixsqw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.zhengqikj.top/gthamdaiwi.html

[Q04] 修改列类型
来源：http://hz.yangfankeji.com/gtkcjeqlod.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.fengsongda.top/gtbutrzydd.html

[Q05] 重命名列
来源：http://hz.xingfuxueyuan.xyz/gtjwnxegev.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.tianlin.xyz/gtmgghuahz.html

[Q06] 删除列
来源：http://hz.zycfv.cn/gtpcxjxwql.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.gotoacloud.top/gtsmgazfwa.html

[Q07] 删除表
来源：http://hz.kuanghao11.cn/gtrhkjimnl.html

DROP TABLE IF EXISTS orders;
来源：http://hz.chenlongwang.top/gtfxpnhgir.html

[Q08] 创建普通索引
来源：http://hz.nanxuanxn.top/gtlyfeaocu.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.ehwqpu.com/gtcdrzfjpq.html

[Q09] 创建唯一索引
来源：http://hz.ivvv.top/gtxwoaqwnm.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.sysykeji.top/gtbvhmmckb.html

[Q10] 插入单行
来源：http://hz.jianghu66.top/gtsfwxnfbg.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.guannengcc.top/gtakqwffvp.html

[Q11] 一次插入多行
来源：http://hz.jinqigufen.top/gtfqwunepx.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yongpay.top/gtajyztjvu.html

[Q12] 插入后取自增 ID
来源：http://hz.shuidangran.top/gtyreqeaqc.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.zhijiandao.cn/gthvuekkwf.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.ydzc1.top/gtrvqlmqwz.html

[Q13] 忽略重复插入
来源：http://hz.zhixingplan.top/gtggmuphzx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.bjfxy.top/gtxegawhnq.html

[Q14] 存在则更新（upsert）
来源：http://hz.dashuyun.cn/gtryuuqwxr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.gogol.net.cn/gtwwvvwpim.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.xziqi.cn/gtgeylzreo.html

[Q15] 查询全部
来源：http://hz.hysaishi.cn/gtjfticxbg.html


<!-- 参考信息 -->