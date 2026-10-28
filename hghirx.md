代发 wailian999

TS:   process.platform;  process.version
来源：http://hz.vqdsnc.cn/gtqwyrkrjb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.guowangkeji.top/gteohzlrdb.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.zhoulong.xyz/gtjzwrctma.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.52xcode.cn/gtffykfusk.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.jinghuilouyu.cn/gtvmkerlfr.html

================================================================================
来源：http://hz.hammf.cn/gtkanzoqck.html

N. 数据结构与算法
来源：http://hz.yj20258888.top/gtknwbeqxp.html

================================================================================
来源：http://hz.daria6918.cn/gtzsovslxi.html

[N01] 二分查找（有序数组）
来源：http://hz.havefunace.top/gtxbaoetld.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yueranfly.top/gtfnpachzm.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.kuanghao11.cn/gtsjeeplwv.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.9152youxi.cn/gtmdcaaged.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.gotoacloud.top/gtvcitrghg.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yvedp.cn/gtdabanfmj.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.gzhubu.top/gtwahjdroa.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.aizwys.cn/gtfoqvraqk.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.ppjwa.cn/gttwwszlid.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.iojbl.cn/gtkjxioytb.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.vqdsnc.cn/gtikhwwnfs.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.kuanghao11.cn/gtubjonqlb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.cqqwz.cn/gtanssnkju.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.daxiang520.top/gtkpcgcasy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.vqdsnc.cn/gtklmgftap.html

Go:   slices.Sort(arr)
来源：http://hz.ywan-chungtsiang.top/gtxmtbokaf.html

Ruby: arr.sort
来源：http://hz.quarkkingdee.top/gtvypysjoz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.jqgfzy.top/gtijxzhtfh.html

[N03] 快速排序（分治示例）
来源：http://hz.sysykeji.top/gtduxxricx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.xziqi.cn/gtezuahjgf.html

PHP:  // 递归实现，或用 usort
来源：http://hz.jqgufenzy.top/gtitsnkvrs.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.andypj.xyz/gtqjwhlmja.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.quarkkingdee.top/gtalfymyjq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.hnqzz.top/gtkhsytzjm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.zhiwuduotai.top/gtdzspzbct.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.shanyushiyangtech.top/gtrfvfzqsw.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.tanke756.top/gtgdwajwgm.html

[N04] 斐波那契数列
来源：http://hz.nanxuanxn.top/gtpexfknxc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.wangshuangyany.cn/gtrmutvucz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.yonumen.top/gtcogxaoti.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hnqzz.top/gtkdqtoztj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jinqigufen.top/gtyjanhnta.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.jinghuilouyu.cn/gtgzntfuzc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.haohaochexian.top/gtzwcgwxtp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yongpay.top/gtryqytoes.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.xylfe.cn/gtmedgmwhs.html

[N05] 最大公约数
来源：http://hz.gaohongyu789.top/gtdeggaltt.html

Py:   math.gcd(a, b)
来源：http://hz.daria6918.cn/gtnttgrqds.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.shangyingyoupin.top/gtuazivyms.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.gaohongyu789.top/gtqxafrmzc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.svipenyu.cn/gttrtnpgfd.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.jianghu66.top/gtfmjzalvh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.sysykeji.top/gtpxvpzqha.html

Ruby: a.gcd(b)
来源：http://hz.yanxiufei.cn/gtkmngqxef.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yonumen.top/gtmkwtbcwd.html

[N06] 判断回文字符串
来源：http://hz.shangyingyoupin.top/gtttqhvuqt.html

Py:   s == s[::-1]
来源：http://hz.hongshengwenyu.top/gtalqbuukn.html

PHP:  $s === strrev($s);
来源：http://hz.zhongyouzk.top/gtpgpexzrb.html

JS:   s === [...s].reverse().join("")
来源：http://hz.hammf.cn/gtdpvbxcww.html

TS:   s === [...s].reverse().join("")
来源：http://hz.zdqjudy.top/gtuwgsrafi.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.xingfuxueyuan.xyz/gthqqgdotf.html

Go:   // 双指针从两端比较
来源：http://hz.tian-w.cn/gttebdbegd.html

Ruby: s == s.reverse
来源：http://hz.svipenyu.cn/gtbocurwtv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yangfankeji.com/gtaxioesqp.html

[N07] 两数之和（返回下标）
来源：http://hz.aizwys.cn/gtxodobvmn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.tian-w.cn/gtdurjyujo.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.hywenlv.cn/gtuwkvpwhh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.svipenyu.cn/gtudoacgre.html

TS:   // 手写 Map<string, number>
来源：http://hz.fengsongda.top/gtquzphgur.html

Java: // 手写 HashMap
来源：http://hz.xziqi.cn/gtvmecguhe.html

Go:   // 手写 map[int]int
来源：http://hz.hongshengwenyu.top/gtatwtgusu.html

Ruby: // 手写 Hash
来源：http://hz.ydjk.org.cn/gtfmpltxkz.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.9152youxi.cn/gtaunrxwfn.html

[N08] 生成全排列
来源：http://hz.zycfv.cn/gtmajuzwwv.html

Py:   itertools.permutations(arr)
来源：http://hz.hammf.cn/gtbagywtmz.html

PHP:  // 手写递归交换
来源：http://hz.zhiwuduotai.top/gtefanomay.html

JS:   // 手写回溯递归
来源：http://hz.0kj1m.cn/gtvtiiyrgu.html

TS:   // 手写回溯递归
来源：http://hz.ehwqpu.com/gtwyibksyx.html

Java: // 手写回溯递归
来源：http://hz.ppjwa.cn/gtdkxywggc.html

Go:   // 手写回溯递归
来源：http://hz.zhiwuduotai.top/gtjkcgwtkz.html

Ruby: arr.permutation.to_a
来源：http://hz.vqdsnc.cn/gtxlvbkbbb.html

C#:   // 手写回溯递归
来源：http://hz.shuidangran.top/gtancukwtr.html

[N09] 栈与队列
来源：http://hz.zhongyouzk.top/gtfjkrmoaw.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.zhijiandao.cn/gtsyipeofy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.quarkkingdee.top/gtieoiptsa.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.feifeiyinyue.top/gtjtteryzj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yuxming.cn/gtzcurorpc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.wangshuangyany.cn/gtycuipnwy.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.yonumen.top/gtwjksbbci.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.fzhhl.top/gtqmpqigsp.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.feifeiyinyue.top/gtdpizhntu.html

[N10] 链表节点定义
来源：http://hz.yangfankeji.com/gtvphjmeru.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.andypj.xyz/gttrvipxgd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.yuxming.cn/gtahyndzac.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.feifeiyinyue.top/gtpfendlvl.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.c1oappe.top/gtypsdargd.html

Java: class Node { int v; Node next; }
来源：http://hz.jiagoushi.top/gtiywfjfcl.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.tianlin.xyz/gtgrlrzrbi.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.pengpengdd.cyou/gtcsykieqx.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.ppjwa.cn/gtwodxjuix.html

[N11] 二叉树中序遍历
来源：http://hz.jianghu66.top/gtyeumfwcy.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.hywenlv.cn/gthnydpinv.html

PHP:  // 手写递归函数
来源：http://hz.xylfe.cn/gtaknmpncp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jinyuanbaomall.cn/gtznugyqwx.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ehwqpu.com/gtktyemzwm.html

Java: // 手写递归
来源：http://hz.jqgufenzy.top/gttgdpjczz.html

Go:   // 手写递归
来源：http://hz.yongpay.top/gthaaglxyx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.xinyue.icu/gtmjqnypwp.html

C#:   // 手写递归
来源：http://hz.birdmap.top/gtsuitnibt.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yangfankeji.com/gtnoneuovm.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.ydzc1.top/gtgeiogjpv.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.gaohongyu789.top/gtvfspizzx.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.birdmap.top/gtdpnvdfxt.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cheryme.top/gtuzmqgjye.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhoulong.xyz/gtpharjyka.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.zhaomingkeji.xyz/gtbrbhvnwg.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.xuetiantiany.cn/gtxlvzscww.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ydzc1.top/gtvlasdglw.html

================================================================================
来源：http://hz.gaohongyu789.top/gtkifgxkqf.html

O. 并发与异步
来源：http://hz.shanyushiyangkeji.top/gtqvlqkuoi.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtseqxctjs.html

[O01] 启动一个线程
来源：http://hz.chenzaomai.com/gtuvwztqux.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.birdmap.top/gtgokhfygh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yanxiufei.cn/gtlsupolrr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.fengsongda.top/gtztpklrka.html

TS:   // 同 JS
来源：http://hz.ybcxt.top/gtljgakzkr.html

Java: new Thread(() -> f()).start()
来源：http://hz.bjfxy.top/gtpxuvbrem.html

Go:   go f()
来源：http://hz.ydjk.org.cn/gthyqgwpyq.html

Ruby: Thread.new { f }
来源：http://hz.cqqwz.cn/gtrfrzbrfv.html

C#:   Task.Run(() => F());
来源：http://hz.wangshuangyany.cn/gtcalthnuk.html

[O02] 使用线程池
来源：http://hz.jlsjyb.cn/gtdrjtfzwf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.cdnleiting.top/gtzintrrjq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.xingfuxueyuan.xyz/gtunylrglc.html

JS:   // worker_threads 线程池
来源：http://hz.svipenyu.cn/gtmcqskqod.html

TS:   // worker_threads 线程池
来源：http://hz.shanyushiyangkeji.top/gtmbyburpc.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.gaohongyu789.top/gtmpofcnmv.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.zhongyouzk.top/gtpsxnjvpj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.jqgufenzy.top/gtonapsiic.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.tian-w.cn/gtpokfgdvf.html

[O03] 加锁保护共享数据
来源：http://hz.yuxming.cn/gtfypmibyg.html

Py:   with lock: shared += 1
来源：http://hz.jiagoushi.top/gtnrawdfhr.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.jqgfzy.top/gtbnlonijb.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.shanyushiyangkeji.top/gtusvkvhuo.html

TS:   // 同 JS
来源：http://hz.svipenyu.cn/gthkkenyhn.html

Java: synchronized (this) { shared++; }
来源：http://hz.yuxming.cn/gtkmwummln.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yanxiufei.cn/gtlxbacnjk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.shuidangran.top/gtwnlxjcyr.html

C#:   lock (gate) { shared++; }
来源：http://hz.quarkkingdee.top/gtbqmdmgod.html

[O04] 定义异步函数并等待
来源：http://hz.sxryk.cn/gtkdumzojk.html

Py:   async def f():⏎    await g()
来源：http://hz.zhengqikj.top/gtwnjhojkf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.tian-w.cn/gtosyrbslp.html

JS:   async function f() { await g(); }
来源：http://hz.chenlongwang.top/gtghssukai.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.hysaishi.cn/gtoieksacv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.yanxiufei.cn/gteclkgrqm.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.hnxiangtu.top/gtijvlkcpp.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.zdqjudy.top/gtivktsbka.html

C#:   async Task F() { await G(); }
来源：http://hz.guowangkeji.top/gtajmpdidh.html

[O05] 并发执行并等待全部完成
来源：http://hz.guowangkeji.top/gtvdsookvr.html

Py:   asyncio.gather(*tasks)
来源：http://hz.chenjidiqi.icu/gtxomruhha.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.ybcxt.top/gtlbspisdi.html

JS:   await Promise.all(tasks)
来源：http://hz.wangshuangyany.cn/gtfoqnfxrg.html

TS:   await Promise.all(tasks)
来源：http://hz.mhx1999.top/gtwpfdcait.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.zycfv.cn/gttvfashfc.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.bjfxy.top/gtskmpifpj.html

Ruby: threads.map(&:join)
来源：http://hz.pengpengdd.cyou/gtuzadygly.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.xziqi.cn/gtbpmlfwqi.html

[O06] 使用进程池
来源：http://hz.jinqigufen.top/gtbaqxuctl.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.dianchejie.cn/gtwjatqjmv.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.xziqi.cn/gtgeyquscd.html

JS:   // child_process / cluster 模块
来源：http://hz.nanxinkj.top/gthvpsjzll.html

TS:   // child_process / cluster 模块
来源：http://hz.tanke756.top/gtvcsrulbl.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.nanxuanxn.top/gtbombgyvz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.dashuyun.cn/gtofvridif.html

Ruby: // fork 块
来源：http://hz.xylfe.cn/gtkgleaaxu.html

C#:   Parallel.For
来源：http://hz.nanxinkj.top/gtwvbuswki.html

================================================================================
来源：http://hz.smart0.xyz/gtsprpbhro.html

P. 常用工具函数
来源：http://hz.hywenlv.cn/gtqrzryffu.html

================================================================================
来源：http://hz.redwolf501.top/gtiabakmiz.html

[P01] 生成 UUID
来源：http://hz.daria6918.cn/gtrlhtcwec.html

Py:   str(uuid.uuid4())
来源：http://hz.vqdsnc.cn/gtaivhrrxb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yj202588.top/gtbcyiqmvi.html

JS:   crypto.randomUUID()
来源：http://hz.chenlongwang.top/gtqpzuyxsp.html

TS:   crypto.randomUUID()
来源：http://hz.nanxinkj.top/gtmborcnab.html

Java: UUID.randomUUID().toString()
来源：http://hz.ydzc1.top/gtvxgobpfe.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yueranfly.top/gtgoiagpes.html

Ruby: SecureRandom.uuid
来源：http://hz.birdmap.top/gtgoeudtzv.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.yvedp.cn/gtlxzagktg.html

[P02] MD5 / SHA256 摘要
来源：http://hz.nwbrower.top/gtsounawae.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.andypj.xyz/gtjphliyka.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.0kj1m.cn/gtcwczwjmq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.zhoulong.xyz/gtbchllpto.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.gzhubu.top/gtbzxjqswj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.redwolf501.top/gtyuxfevrz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.aizwys.cn/gtttwhodck.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.yj20258.top/gtkxaijjpb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.wangshuangyany.cn/gtzszjdaab.html

[P03] 生成短随机字符串
来源：http://hz.guannengcc.top/gtusfmdocx.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.gotoacloud.top/gtoebeucer.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.gogol.net.cn/gtknalvmon.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.aizwys.cn/gtbiwsasft.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhijiandao.cn/gtvvualsgt.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.quarkkingdee.top/gtgiysdvhp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.dianchejie.cn/gtfevcffkr.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.cdnleiting.top/gtchoxifvh.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.316326.xyz/gtotyhqhrp.html

[P04] 求长度
来源：http://hz.tanke756.top/gtphdmywyc.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.jinghuilouyu.cn/gtlfkmtdlr.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shanyushiyangtech.top/gtwconexft.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.dashuyun.cn/gtwcpduabl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.havefunace.top/gtlbyczvsu.html

Java: list.size();  map.size();  s.length()
来源：http://hz.yueranfly.top/gtalswwzhf.html

Go:   len(arr);  len(m)
来源：http://hz.bjfxy.top/gtpcozcexj.html

Ruby: x.length;  x.size
来源：http://hz.sysykeji.top/gtkmhitqke.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.chenlongwang.top/gtfwtsjycm.html

[P05] 判断两个对象内容是否相等
来源：http://hz.xziqi.cn/gtvjpvmfky.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.redwolf501.top/gtpxbsvfry.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.svipenyu.cn/gtjfsvafux.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.zhijiandao.cn/gtvhnchehh.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.cheryme.top/gtzmdcknkk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.chenzaomai.com/gtdxsxudtp.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.hnxiangtu.top/gtxeyitwkc.html

Ruby: a == b
来源：http://hz.xinyue.icu/gtginmbbko.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.cheryme.top/gtbkwalefw.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.meibo888.top/gtkhffpkgp.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.zhijiandao.cn/gtbvgotvml.html

PHP:  if (empty($x)) {}
来源：http://hz.yanxiufei.cn/gticbolous.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.ehwqpu.com/gtyzyrwdxr.html

TS:   if (x == null) {}
来源：http://hz.ppjwa.cn/gtxhvlqshz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.9152youxi.cn/gtdqlxjcgp.html

Go:   if x == nil {}
来源：http://hz.yj20258.top/gtsxtnqhnr.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.yj20258888.top/gtrgnajplo.html

C#:   if (x is null) {}
来源：http://hz.gogol.net.cn/gtwqtbvnrd.html

[P07] 防抖与节流
来源：http://hz.nwbrower.top/gtgxhyemyy.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.shangyingyoupin.top/gtwaptfifr.html

PHP:  // 手写时间戳比较
来源：http://hz.meibo888.top/gtrgfmxwdz.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.gaohongyu789.top/gtcyattszy.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yueranfly.top/gtfufgyleo.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.tanke756.top/gtcajpvtjq.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.jinghuilouyu.cn/gttvwqfwbj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.jiagoushi.top/gtgdquthvo.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.wangdashe.top/gtmkfsapwp.html

[P08] 处理浮点精度问题
来源：http://hz.aibaodan.cn/gtgxchjict.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.ppjwa.cn/gtfqmrovei.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.zhixingplan.top/gtuhjawxhf.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.kuanghao11.cn/gtzsvskdsc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.cqqwz.cn/gtixopekdk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.redwolf501.top/gttwzaxkkr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.xuetiantiany.cn/gtqdamiiad.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.xziqi.cn/gtupsuqacu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.zhijiandao.cn/gtsmcxnrfu.html

================================================================================
来源：http://hz.cucudq.cn/gtsvcixhiv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.daria6918.cn/gtymgoowbi.html

================================================================================
来源：http://hz.fengsongda.top/gtqfvmlikp.html

[Q01] 创建表
来源：http://hz.zhiwuduotai.top/gtqyqiujub.html

CREATE TABLE users (
来源：http://hz.hnxiangtu.top/gtmphgcgsa.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jinqigufen.top/gtrwztijcx.html

name VARCHAR(50) NOT NULL,
来源：http://hz.0kj1m.cn/gtsrrkdxnl.html

email VARCHAR(100) UNIQUE,
来源：http://hz.zdqjudy.top/gtgwrdlgbi.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.gzhubu.top/gtktusvzio.html

);
来源：http://hz.xylfe.cn/gtpdttxvnx.html

[Q02] 创建带外键的表
来源：http://hz.jinqigufen.top/gthsynysbc.html

CREATE TABLE orders (
来源：http://hz.jinqigfzy.top/gtlvamgeto.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.pycfn.com/gtqkhjfwkc.html

user_id INT NOT NULL,
来源：http://hz.gotoacloud.top/gtkzegckte.html

amount DECIMAL(10, 2),
来源：http://hz.zhijiandao.cn/gtdamxjsyl.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.gotoacloud.top/gtzgylnecm.html

);
来源：http://hz.fengsongda.top/gthwlksuau.html

[Q03] 增加列
来源：http://hz.sxryk.cn/gthtcyofpm.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.aizwys.cn/gtlpwyotzi.html

[Q04] 修改列类型
来源：http://hz.yj202588.top/gtmwvfxdne.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.gaohongyu789.top/gtqldraujn.html

[Q05] 重命名列
来源：http://hz.yueranfly.top/gtmnftrijd.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.zhongyouzk.top/gtoywbxefk.html

[Q06] 删除列
来源：http://hz.ybcxt.top/gtnhdjchpn.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.ydjk.org.cn/gtwyyjldma.html

[Q07] 删除表
来源：http://hz.hammf.cn/gtcjxjujis.html

DROP TABLE IF EXISTS orders;
来源：http://hz.cheryme.top/gtpjkdsjqr.html

[Q08] 创建普通索引
来源：http://hz.yj20258.top/gtylpbbbls.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.yongpay.top/gtgbwgmthw.html

[Q09] 创建唯一索引
来源：http://hz.andypj.xyz/gtrtbegjbr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.nanxinkj.top/gtrzgzvwnu.html

[Q10] 插入单行
来源：http://hz.cheryme.top/gtbdxhvvvn.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.aibaodan.cn/gtsfgecgjj.html

[Q11] 一次插入多行
来源：http://hz.xingfuxueyuan.xyz/gtzudwtsez.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.redwolf501.top/gtxuueibjy.html

[Q12] 插入后取自增 ID
来源：http://hz.xinyue.icu/gthtajnvmd.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.xziqi.cn/gtfyusucls.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.hysaishi.cn/gtakakmkub.html

[Q13] 忽略重复插入
来源：http://hz.shanyushiyangtech.top/gtfthvgojl.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.yj20258888.top/gtzipustut.html

[Q14] 存在则更新（upsert）
来源：http://hz.xziqi.cn/gtrajkgtrg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.ppjwa.cn/gtebvcohtt.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.wangdashe.top/gtqsyekwxo.html

[Q15] 查询全部
来源：http://hz.daxiang520.top/gtcgwusppg.html

SELECT * FROM users;
来源：http://hz.zhixingplan.top/gtudzlfwtq.html

[Q16] 查询指定列
来源：http://hz.yvedp.cn/gtrhzvckdo.html

SELECT id, name FROM users;
来源：http://hz.shangyingyoupin.top/gtuzrdpoqv.html

[Q17] 条件查询
来源：http://hz.zhengqikj.top/gtwimhkvgc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.jinqigufen.top/gtemurpapp.html

[Q18] 模糊匹配
来源：http://hz.yongpay.top/gtdyfkmxyv.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.52xcode.cn/gtnuiwemcj.html

[Q19] 范围查询
来源：http://hz.zhixingplan.top/gtxtmednja.html


<!-- 参考信息 -->