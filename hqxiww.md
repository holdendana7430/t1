代发 wailian999

Java: public static void main(String[] args)
来源：http://hz.svipenyu.cn/gtcxlmylir.html

Go:   func main()
来源：http://hz.ppjwa.cn/gtdpucglrr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.xuetiantiany.cn/gtxzlqjicw.html

C#:   static void Main(string[] args)
来源：http://hz.hywenlv.cn/gtxkcwpmif.html

[M08] 获取系统与运行时信息
来源：http://hz.mhx1999.top/gtpsxtmtlp.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jlsjyb.cn/gtgjiexzhx.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.feifeiyinyue.top/gtchdoargz.html

JS:   process.platform;  process.version
来源：http://hz.wangdashe.top/gtcmcjzopd.html

TS:   process.platform;  process.version
来源：http://hz.shuidangran.top/gtfcbwplbx.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.zhijiandao.cn/gtdstbtswi.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.tanke756.top/gtyfgbqexb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.wangdashe.top/gtdaqrcejd.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yuxming.cn/gtfnltyxvv.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtijqulxbg.html

N. 数据结构与算法
来源：http://hz.0kj1m.cn/gtzwurespp.html

================================================================================
来源：http://hz.jinqigfzy.top/gtwjyvwhjc.html

[N01] 二分查找（有序数组）
来源：http://hz.hammf.cn/gtvagckdcu.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.hongshengwenyu.top/gtjsaqzgrs.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.gzhubu.top/gtoixwotgf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cucudq.cn/gtgfbemxgj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhoulong.xyz/gtxpjykqcz.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.cheryme.top/gtwbmwreuh.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.yj202588.top/gtpcuvehhv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.xuetiantiany.cn/gtoarubkah.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.zhoulong.xyz/gtjkndgdvo.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.52xcode.cn/gtnhqdhgyr.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhaomingkeji.xyz/gtzbksavgh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.tianlin.xyz/gtbjdpyzwx.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.bjfxy.top/gtlmeksxii.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ybcxt.top/gtjimbynuu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.xylfe.cn/gtdglcjkdw.html

Go:   slices.Sort(arr)
来源：http://hz.zhongyouzk.top/gtgxwukzjb.html

Ruby: arr.sort
来源：http://hz.hammf.cn/gtcwgbpznh.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.sysykeji.top/gtonorrogm.html

[N03] 快速排序（分治示例）
来源：http://hz.sufxvd.cn/gtllatfzsr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.hnxiangtu.top/gtxeantpez.html

PHP:  // 递归实现，或用 usort
来源：http://hz.kuanghao11.cn/gttiamaugb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.gotoacloud.top/gtcoohmath.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.chenjidiqi.icu/gtshnvxrah.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.sxryk.cn/gtncttsvqb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jiagoushi.top/gtqzfcvpdj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yangfankeji.com/gtxnpnvrlz.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.xuanzx.com/gtpzsuhtes.html

[N04] 斐波那契数列
来源：http://hz.sweek.top/gtscbohdce.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.andypj.xyz/gtzqepzszb.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.xylfe.cn/gtgojlzomp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.sufxvd.cn/gtaiqnslbd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ivvv.top/gtjizkgipn.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.bjfxy.top/gthkpemxbl.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.cqqwz.cn/gtirioikrc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.fzhhl.top/gtskysxfgd.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.jinyuanbaomall.cn/gtnnpneubp.html

[N05] 最大公约数
来源：http://hz.vqdsnc.cn/gtwtxvxmlv.html

Py:   math.gcd(a, b)
来源：http://hz.cucudq.cn/gttsitcwtz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yonumen.top/gtllrmptpz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jinyuanbaomall.cn/gtuxopuruv.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hysaishi.cn/gtocufrhsd.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.iojbl.cn/gtdjyrzzwr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.shanyushiyangtech.top/gtwyycpthp.html

Ruby: a.gcd(b)
来源：http://hz.nanxinkj.top/gtmwsanmed.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.tian-w.cn/gtpfkioahp.html

[N06] 判断回文字符串
来源：http://hz.nwbrower.top/gtkokfobay.html

Py:   s == s[::-1]
来源：http://hz.gotoacloud.top/gtqoojihka.html

PHP:  $s === strrev($s);
来源：http://hz.yangfankeji.com/gtfvvpprco.html

JS:   s === [...s].reverse().join("")
来源：http://hz.hnqzz.top/gtbcgyxuvv.html

TS:   s === [...s].reverse().join("")
来源：http://hz.ybcxt.top/gtmiozfqly.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.yangfankeji.com/gtlzowlemo.html

Go:   // 双指针从两端比较
来源：http://hz.yj20258.top/gtnbrnkoph.html

Ruby: s == s.reverse
来源：http://hz.jinqigufen.top/gtrwsltodw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yuxming.cn/gtzqwhbvpo.html

[N07] 两数之和（返回下标）
来源：http://hz.yanxiufei.cn/gtybiibesz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.zhiwuduotai.top/gtimclshyq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.nanxinkj.top/gtxkvakqbl.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.hywenlv.cn/gtepginfsv.html

TS:   // 手写 Map<string, number>
来源：http://hz.redwolf501.top/gtwtahdndt.html

Java: // 手写 HashMap
来源：http://hz.yuxming.cn/gtbepajedq.html

Go:   // 手写 map[int]int
来源：http://hz.ywan-chungtsiang.top/gtprtbuslr.html

Ruby: // 手写 Hash
来源：http://hz.feifeiyinyue.top/gthgmafknh.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.ppjwa.cn/gteogodrdt.html

[N08] 生成全排列
来源：http://hz.svipenyu.cn/gtjrgbeaus.html

Py:   itertools.permutations(arr)
来源：http://hz.mhx1999.top/gtwwowjxfv.html

PHP:  // 手写递归交换
来源：http://hz.shanyushiyangkeji.top/gtpmekiedh.html

JS:   // 手写回溯递归
来源：http://hz.gaohongyu789.top/gtgxwvhmga.html

TS:   // 手写回溯递归
来源：http://hz.yvedp.cn/gtvjzerzrt.html

Java: // 手写回溯递归
来源：http://hz.xuanzx.com/gtjnvmfrfn.html

Go:   // 手写回溯递归
来源：http://hz.shzxlz.cn/gteustyhkp.html

Ruby: arr.permutation.to_a
来源：http://hz.yvedp.cn/gtkbdvjjqt.html

C#:   // 手写回溯递归
来源：http://hz.9152youxi.cn/gtffykzjlv.html

[N09] 栈与队列
来源：http://hz.zhijiandao.cn/gtrvfyehvx.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.9152youxi.cn/gtpxdjtizm.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.aizwys.cn/gtpayldizm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.nwbrower.top/gtuolkpksy.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yongpay.top/gtksgqgqva.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.zhongyouzk.top/gtantfxxva.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.gzhubu.top/gtanfswnra.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.havefunace.top/gtjcvvxgyy.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.zycfv.cn/gtjujaleqj.html

[N10] 链表节点定义
来源：http://hz.hongshengwenyu.top/gtayadjhhm.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.xingfuxueyuan.xyz/gtzykxlbqx.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.gaohongyu789.top/gtssslxieb.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zhixingplan.top/gtqciyblek.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.vqdsnc.cn/gtienkoqdq.html

Java: class Node { int v; Node next; }
来源：http://hz.hammf.cn/gtruzbayah.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.zycfv.cn/gtagsobnxk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.yuxming.cn/gttlondmso.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.xingfuxueyuan.xyz/gtcnjkungm.html

[N11] 二叉树中序遍历
来源：http://hz.ydzc1.top/gtzrdxevkr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.birdmap.top/gtrywshxsn.html

PHP:  // 手写递归函数
来源：http://hz.tian-w.cn/gtsttofatt.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.shangyingyoupin.top/gtevardkvk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.cashguo.top/gtzcozoikx.html

Java: // 手写递归
来源：http://hz.guannengcc.top/gtoavcpogn.html

Go:   // 手写递归
来源：http://hz.zhijiandao.cn/gtyaqtvkcb.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.svipenyu.cn/gtvqqhwsbv.html

C#:   // 手写递归
来源：http://hz.jyoumei.cn/gtssphvlmc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.jinqigufen.top/gtgfitmwhn.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.chenlongwang.top/gtgqgkgvzg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.chenzaomai.com/gttyglgwru.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jinghuilouyu.cn/gtsplwpnty.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ydjk.org.cn/gtewzsxjkt.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hongshengwenyu.top/gtwnmidoeo.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.cqqwz.cn/gtycqexygc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.ppjwa.cn/gtigeujtub.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jiagoushi.top/gtwsbszygo.html

================================================================================
来源：http://hz.xziqi.cn/gtgyfhyruz.html

O. 并发与异步
来源：http://hz.sweek.top/gtwjadxjta.html

================================================================================
来源：http://hz.zhijiandao.cn/gtdwgylxta.html

[O01] 启动一个线程
来源：http://hz.chenjidiqi.icu/gtcvdzwnfj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.jianghu66.top/gtvgoekiub.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.kuanghao11.cn/gtluvggioj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.yanxiufei.cn/gtskijpgcb.html

TS:   // 同 JS
来源：http://hz.bjfxy.top/gtqxbnjluj.html

Java: new Thread(() -> f()).start()
来源：http://hz.gotoacloud.top/gthyeaxtza.html

Go:   go f()
来源：http://hz.hammf.cn/gtbtdzwyck.html

Ruby: Thread.new { f }
来源：http://hz.yuanzhike.top/gtipulqnxz.html

C#:   Task.Run(() => F());
来源：http://hz.mhx1999.top/gttgmmzsac.html

[O02] 使用线程池
来源：http://hz.jiagoushi.top/gtdxpfbmlo.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yanxiufei.cn/gtbcvktdtt.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.ydzc1.top/gtjeeouetr.html

JS:   // worker_threads 线程池
来源：http://hz.cqqwz.cn/gtjpieijdg.html

TS:   // worker_threads 线程池
来源：http://hz.yj20258.top/gtauwczdgl.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.xziqi.cn/gtvmnwickb.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.chenjidiqi.icu/gtcxdtyagj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.cdnleiting.top/gtjstfbpfh.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.jinyuanbaomall.cn/gtbbatfcdh.html

[O03] 加锁保护共享数据
来源：http://hz.cheryme.top/gtwzqdipoh.html

Py:   with lock: shared += 1
来源：http://hz.gzhubu.top/gtcmgqtydd.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.jinqigufen.top/gtbwmtaarm.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.yuanzhike.top/gtxuvpciut.html

TS:   // 同 JS
来源：http://hz.yanxiufei.cn/gterangjxr.html

Java: synchronized (this) { shared++; }
来源：http://hz.vqdsnc.cn/gthrmcnapt.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.c1oappe.top/gtbmwrngmp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.cashguo.top/gttluujsjz.html

C#:   lock (gate) { shared++; }
来源：http://hz.ywan-chungtsiang.top/gtxofuzoil.html

[O04] 定义异步函数并等待
来源：http://hz.daxiang520.top/gtuwfnhvza.html

Py:   async def f():⏎    await g()
来源：http://hz.cashguo.top/gtojqlobkc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.xuanzx.com/gtvoayuzze.html

JS:   async function f() { await g(); }
来源：http://hz.jqgfzy.top/gtpiiydvpu.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.ydzc1.top/gtrmfbmlzu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.shzxlz.cn/gtcqlabooj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.cdnleiting.top/gtwkqglrwa.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.jlsjyb.cn/gtfansvylc.html

C#:   async Task F() { await G(); }
来源：http://hz.jlsjyb.cn/gtaldzvrjh.html

[O05] 并发执行并等待全部完成
来源：http://hz.yonumen.top/gtabwqbdck.html

Py:   asyncio.gather(*tasks)
来源：http://hz.xuetiantiany.cn/gtwkkzfwvf.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.xuetiantiany.cn/gtkjkbfxii.html

JS:   await Promise.all(tasks)
来源：http://hz.aizwys.cn/gtjwqkxwoz.html

TS:   await Promise.all(tasks)
来源：http://hz.vqdsnc.cn/gtmirwrxjd.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.cdnleiting.top/gtvvawdnow.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.zhixingplan.top/gtqijncjhx.html

Ruby: threads.map(&:join)
来源：http://hz.pengpengdd.cyou/gtudldlqnu.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.xuetiantiany.cn/gtzbccryjx.html

[O06] 使用进程池
来源：http://hz.fengsongda.top/gtumaorqne.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.yvedp.cn/gtdcvdniaj.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.zycfv.cn/gtrcpnbdzq.html

JS:   // child_process / cluster 模块
来源：http://hz.cashguo.top/gtignpngqs.html

TS:   // child_process / cluster 模块
来源：http://hz.hysaishi.cn/gtynkzeawf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yueranfly.top/gtmtpvrymo.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.nanxuanxn.top/gtynlwqeaf.html

Ruby: // fork 块
来源：http://hz.aibaodan.cn/gtiaxvhjds.html

C#:   Parallel.For
来源：http://hz.yongpay.top/gtrkcbtmwa.html

================================================================================
来源：http://hz.quarkkingdee.top/gturibofpa.html

P. 常用工具函数
来源：http://hz.yj202588.top/gtiothtkwz.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtgziyqyej.html

[P01] 生成 UUID
来源：http://hz.svipenyu.cn/gtietpgtmk.html

Py:   str(uuid.uuid4())
来源：http://hz.jinqigfzy.top/gtjfzbpkpn.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.shanyushiyangtech.top/gthuoeklwv.html

JS:   crypto.randomUUID()
来源：http://hz.hnxiangtu.top/gtnxlhczyf.html

TS:   crypto.randomUUID()
来源：http://hz.cucudq.cn/gtppaibzbq.html

Java: UUID.randomUUID().toString()
来源：http://hz.316326.xyz/gtkelqrmvi.html

Go:   // 用 github.com/google/uuid
来源：http://hz.hysaishi.cn/gtqfllazoe.html

Ruby: SecureRandom.uuid
来源：http://hz.xinyue.icu/gteeemnwgn.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.birdmap.top/gtkwdrbmhb.html

[P02] MD5 / SHA256 摘要
来源：http://hz.yuxming.cn/gthcqasyll.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.cashguo.top/gtecmomcge.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.shzxlz.cn/gthffkvibo.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.hywenlv.cn/gttqetxvsd.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.pengpengdd.cyou/gtukggppjt.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.xuanzx.com/gtcadxjtvs.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.hnxiangtu.top/gtntiasefp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.shuidangran.top/gtfwadskjw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.pengpengdd.cyou/gtcdhwqksp.html

[P03] 生成短随机字符串
来源：http://hz.fzhhl.top/gtysvjxazi.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.316326.xyz/gtlvpwckyx.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.sufxvd.cn/gtthlsxjuh.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hongshengwenyu.top/gtpkyjeuyl.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.pycfn.com/gtqzakrbjn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.andypj.xyz/gtinjbemir.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.jqgfzy.top/gtduedslhd.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.nwbrower.top/gtaxkpkioe.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jianghu66.top/gtffttvodc.html

[P04] 求长度
来源：http://hz.pycfn.com/gtrxiuhhwv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.316326.xyz/gthesqwycn.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.nwbrower.top/gtmrkhkefm.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jqgfzy.top/gtpgwpvccn.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhixingplan.top/gtrtwssbys.html

Java: list.size();  map.size();  s.length()
来源：http://hz.zhoulong.xyz/gtsfmqvjih.html

Go:   len(arr);  len(m)
来源：http://hz.yueranfly.top/gtoqnruijf.html

Ruby: x.length;  x.size
来源：http://hz.hysaishi.cn/gtotccmlol.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.jqgfzy.top/gtyqugfdtc.html

[P05] 判断两个对象内容是否相等
来源：http://hz.ydzc1.top/gtvfrpbdej.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.sysykeji.top/gtmaglyxeb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.sweek.top/gtuovoupae.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.zhiwuduotai.top/gtkmeejcxs.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.shuidangran.top/gtvvinzfgg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.hywenlv.cn/gtnpgequga.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yuxming.cn/gtbobjvhww.html

Ruby: a == b
来源：http://hz.ywan-chungtsiang.top/gtxyfzgpkl.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.gaohongyu789.top/gtjwerwpgh.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.wangshuangyany.cn/gtllvlpzsj.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.shuidangran.top/gtdzwvmxel.html

PHP:  if (empty($x)) {}
来源：http://hz.shangyingyoupin.top/gtfkuewhsx.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.c1oappe.top/gtkhvqlbem.html

TS:   if (x == null) {}
来源：http://hz.tianlin.xyz/gtzvrkrilk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.zhixingplan.top/gtujcvbcgd.html

Go:   if x == nil {}
来源：http://hz.ybcxt.top/gtvdvxqmzk.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.wangshuangyany.cn/gtlauxjuow.html

C#:   if (x is null) {}
来源：http://hz.sxryk.cn/gtyoxtmqqb.html

[P07] 防抖与节流
来源：http://hz.feifeiyinyue.top/gtysoynsoh.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.aibaodan.cn/gtxuzwekoc.html

PHP:  // 手写时间戳比较
来源：http://hz.xingfuxueyuan.xyz/gtcohjadwc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yangfankeji.com/gtdxugxrxz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ppjwa.cn/gtkmcnjqhi.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.xingfuxueyuan.xyz/gtjoczdnug.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.mhx1999.top/gtodnokedi.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.aizwys.cn/gtqgwmhkta.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.316326.xyz/gtienxjper.html

[P08] 处理浮点精度问题
来源：http://hz.kuanghao11.cn/gtvtugyxhh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.yj20258888.top/gtgifnokse.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.kuanghao11.cn/gtfgyzqegg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.hammf.cn/gtvocuwyje.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.yuanzhike.top/gtnbjccivz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.dianchejie.cn/gtbgmhcjur.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.bjfxy.top/gtxplaccgy.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.jiagoushi.top/gtzshwbwgi.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.nanxinkj.top/gtqwmwyghs.html

================================================================================
来源：http://hz.nanxinkj.top/gtnkzoqjeg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.birdmap.top/gtudfzoyzd.html

================================================================================
来源：http://hz.zdqjudy.top/gtsaivdgyx.html

[Q01] 创建表
来源：http://hz.kuanghao11.cn/gtugnvntkg.html

CREATE TABLE users (
来源：http://hz.xylfe.cn/gtludfhjhz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.sxryk.cn/gtxjxjspyq.html

name VARCHAR(50) NOT NULL,
来源：http://hz.zhijiandao.cn/gtanugfgzg.html

email VARCHAR(100) UNIQUE,
来源：http://hz.svipenyu.cn/gtjlvcbvee.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.feifeiyinyue.top/gtgksfnrzb.html

);
来源：http://hz.gaohongyu789.top/gtomdoqsst.html

[Q02] 创建带外键的表
来源：http://hz.yanxiufei.cn/gttvzerubo.html

CREATE TABLE orders (
来源：http://hz.sufxvd.cn/gtdreimxjl.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hongshengwenyu.top/gtbezlqege.html

user_id INT NOT NULL,
来源：http://hz.bjfxy.top/gtzzhhfamx.html

amount DECIMAL(10, 2),
来源：http://hz.yj202588.top/gtglvcmtcw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.zycfv.cn/gtzbnjqfkc.html

);
来源：http://hz.cheryme.top/gtyomfkbye.html

[Q03] 增加列
来源：http://hz.xuetiantiany.cn/gtxmqysveg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.hammf.cn/gtmbixclgx.html

[Q04] 修改列类型
来源：http://hz.jiagoushi.top/gtdaebnfgp.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.quarkkingdee.top/gtgolnquii.html

[Q05] 重命名列
来源：http://hz.ydzc1.top/gthznyusoi.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.ybcxt.top/gtjgejgzhn.html

[Q06] 删除列
来源：http://hz.zhengqikj.top/gteuypmjzn.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.sxryk.cn/gtqtxduxze.html

[Q07] 删除表
来源：http://hz.ydjk.org.cn/gtbrsrnlqw.html

DROP TABLE IF EXISTS orders;
来源：http://hz.mhx1999.top/gtvrclbglw.html

[Q08] 创建普通索引
来源：http://hz.yonumen.top/gtqeztwbhh.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.vqdsnc.cn/gtieanehvx.html

[Q09] 创建唯一索引
来源：http://hz.gogol.net.cn/gthlwcwtiq.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.yuxming.cn/gtqvaovzww.html

[Q10] 插入单行
来源：http://hz.9152youxi.cn/gtwsoaistd.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.cheryme.top/gttgdhdnqg.html

[Q11] 一次插入多行
来源：http://hz.zhijiandao.cn/gtwftkcqxp.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.hfpthk.cn/gtvrxybdgg.html

[Q12] 插入后取自增 ID
来源：http://hz.yanxiufei.cn/gtnyoyhnbo.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.ydzc1.top/gtwdjtcddh.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yuanzhike.top/gtssqqifyd.html

[Q13] 忽略重复插入
来源：http://hz.svipenyu.cn/gtlkjhdrts.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.yueranfly.top/gtmqusgvwq.html

[Q14] 存在则更新（upsert）
来源：http://hz.snrcjt.cn/gtuiwbrjok.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.ybcxt.top/gtnvlnvyfn.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.aibaodan.cn/gtpefajdky.html

[Q15] 查询全部
来源：http://hz.sweek.top/gtfdwomrmy.html


<!-- 参考信息 -->