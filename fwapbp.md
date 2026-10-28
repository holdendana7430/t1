代发 wailian999

TS:   process.platform;  process.version
来源：http://hz.0kj1m.cn/gtlfcgmfqf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.shangyingyoupin.top/gtyxqnilps.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.svipenyu.cn/gtulnclzgy.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.aizwys.cn/gtrfmorlao.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.52xcode.cn/gttwhyyoqf.html

================================================================================
来源：http://hz.yongpay.top/gtrqxaqmtp.html

N. 数据结构与算法
来源：http://hz.xinyue.icu/gtteotdwlj.html

================================================================================
来源：http://hz.daxiang520.top/gtwdovzqhv.html

[N01] 二分查找（有序数组）
来源：http://hz.guowangkeji.top/gtahkjmqka.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.jinghuilouyu.cn/gtqljtfjbn.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.daxiang520.top/gthzmtrfgz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yanxiufei.cn/gtuxuzgend.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.aibaodan.cn/gtuhxopcgm.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.zhixingplan.top/gtokbvkqvu.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.zhengqikj.top/gtbgpdbcec.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.aibaodan.cn/gtmuauqroj.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.yueranfly.top/gttwbagezd.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.ybcxt.top/gtmgdtirkw.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.c1oappe.top/gtttccfodu.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.zhijiandao.cn/gtydarhbnk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.aibaodan.cn/gtrjtdvhlf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.pycfn.com/gtbzofwffi.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.0kj1m.cn/gtroptjmwi.html

Go:   slices.Sort(arr)
来源：http://hz.cheryme.top/gtpykrxyaq.html

Ruby: arr.sort
来源：http://hz.birdmap.top/gtiwkqinqb.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.dianchejie.cn/gtxnrxelan.html

[N03] 快速排序（分治示例）
来源：http://hz.shangyingyoupin.top/gtgqughwky.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.52xcode.cn/gtyehdtfvc.html

PHP:  // 递归实现，或用 usort
来源：http://hz.sxryk.cn/gtmsdoxfap.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cucudq.cn/gtfypukxzx.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yonumen.top/gthfsidnlw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jqgufenzy.top/gtvmpxlncn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.pycfn.com/gtuflwiizd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.iojbl.cn/gtsnqbvyeo.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yj202588.top/gtrwshjysn.html

[N04] 斐波那契数列
来源：http://hz.hnqzz.top/gtdvtnhtpx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.cucudq.cn/gtdytehysz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.9152youxi.cn/gttqjtlvas.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jiagoushi.top/gtikacljos.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jinqigfzy.top/gteofufwyf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.zhengqikj.top/gtqcdfwnda.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yangfankeji.com/gtfenedcvp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.andypj.xyz/gtsbvzvaqt.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.ybcxt.top/gtskqmkygw.html

[N05] 最大公约数
来源：http://hz.quarkkingdee.top/gtfgzpzpki.html

Py:   math.gcd(a, b)
来源：http://hz.aibaodan.cn/gttpossqwm.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.ydjk.org.cn/gtjiwgievt.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.daria6918.cn/gtodyqbtuo.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jyoumei.cn/gtvqcmoixv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.daria6918.cn/gtwixbklil.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.hywenlv.cn/gtavwbtoje.html

Ruby: a.gcd(b)
来源：http://hz.hammf.cn/gtgbqcdzqm.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jinqigufen.top/gtgocseart.html

[N06] 判断回文字符串
来源：http://hz.yuanzhike.top/gthcgzkszc.html

Py:   s == s[::-1]
来源：http://hz.meibo888.top/gtkbfbmcbt.html

PHP:  $s === strrev($s);
来源：http://hz.hammf.cn/gtyaawiats.html

JS:   s === [...s].reverse().join("")
来源：http://hz.yj202588.top/gtcabellqk.html

TS:   s === [...s].reverse().join("")
来源：http://hz.vqdsnc.cn/gthiddmxck.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.daria6918.cn/gtqfvkitle.html

Go:   // 双指针从两端比较
来源：http://hz.xylfe.cn/gtpmcqrkan.html

Ruby: s == s.reverse
来源：http://hz.hammf.cn/gtcjoqrrhp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.cdnleiting.top/gtocsdnchz.html

[N07] 两数之和（返回下标）
来源：http://hz.svipenyu.cn/gtixpnezjv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.ehwqpu.com/gtxgnkxceu.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.hfpthk.cn/gtodkusckl.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.316326.xyz/gtllokyrdi.html

TS:   // 手写 Map<string, number>
来源：http://hz.wangdashe.top/gtemfjwjlj.html

Java: // 手写 HashMap
来源：http://hz.0kj1m.cn/gthosxmgjx.html

Go:   // 手写 map[int]int
来源：http://hz.jinqigufen.top/gtgowlkzgm.html

Ruby: // 手写 Hash
来源：http://hz.meibo888.top/gtcskujvls.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.nanxuanxn.top/gtxxavzqlz.html

[N08] 生成全排列
来源：http://hz.cheryme.top/gtgvlsqmow.html

Py:   itertools.permutations(arr)
来源：http://hz.zhaomingkeji.xyz/gtsfytkjgr.html

PHP:  // 手写递归交换
来源：http://hz.havefunace.top/gtyzliqerr.html

JS:   // 手写回溯递归
来源：http://hz.jinqigufen.top/gtzufgqpah.html

TS:   // 手写回溯递归
来源：http://hz.yj202588.top/gtalagtoof.html

Java: // 手写回溯递归
来源：http://hz.cdnleiting.top/gtgmperuog.html

Go:   // 手写回溯递归
来源：http://hz.ybcxt.top/gtvaqtdjkr.html

Ruby: arr.permutation.to_a
来源：http://hz.sxryk.cn/gtjbqhkhpd.html

C#:   // 手写回溯递归
来源：http://hz.jinghuilouyu.cn/gtfufztkyi.html

[N09] 栈与队列
来源：http://hz.tianlin.xyz/gtptbvmebu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.ydzc1.top/gtlcqbwrox.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.yanxiufei.cn/gtguvevfab.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.feifeiyinyue.top/gtdarzetqk.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.hnxiangtu.top/gtrimjulga.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.fzhhl.top/gtkgmgmgfm.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.snrcjt.cn/gtictedlpl.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.hysaishi.cn/gtlxxfyekl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.birdmap.top/gtfyuszefv.html

[N10] 链表节点定义
来源：http://hz.sxryk.cn/gtqlmqqzou.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.redwolf501.top/gtynrobkrm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.redwolf501.top/gtvcioamrz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zhiwuduotai.top/gtmehwffbn.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.9152youxi.cn/gtliyqnmrc.html

Java: class Node { int v; Node next; }
来源：http://hz.ybcxt.top/gtxhbbwasr.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.shzxlz.cn/gtnzrmvmgu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.kuanghao11.cn/gtwamxzhqh.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yueranfly.top/gtnlxbkpgs.html

[N11] 二叉树中序遍历
来源：http://hz.jinqigufen.top/gtnfvnkhbj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.redwolf501.top/gtszydeoyx.html

PHP:  // 手写递归函数
来源：http://hz.fzhhl.top/gtdiwrsmsn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.sufxvd.cn/gtjioidtjy.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ydzc1.top/gtuvtkgnkn.html

Java: // 手写递归
来源：http://hz.daria6918.cn/gtrkvrfsfd.html

Go:   // 手写递归
来源：http://hz.c1oappe.top/gttvdwyedj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.shanyushiyangkeji.top/gtbgswmkhw.html

C#:   // 手写递归
来源：http://hz.ywan-chungtsiang.top/gttmxljazt.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.gogol.net.cn/gtaccdxbxj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.jqgfzy.top/gtbjljqobd.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.mhx1999.top/gtxpkmrzij.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.shzxlz.cn/gtfmrioeba.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yangfankeji.com/gtpmtcwwbv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.sxryk.cn/gtsowvcsyc.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.dianchejie.cn/gtbwqtylxy.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.sxryk.cn/gtlycphfoh.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.52xcode.cn/gtsfozqkxy.html

================================================================================
来源：http://hz.nanxuanxn.top/gtivkdywhd.html

O. 并发与异步
来源：http://hz.nwbrower.top/gtgjazkzga.html

================================================================================
来源：http://hz.jyoumei.cn/gtcexbszlo.html

[O01] 启动一个线程
来源：http://hz.yongpay.top/gtfjhaedtw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.tian-w.cn/gtmlsratxr.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.316326.xyz/gtajbsdrgy.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.ivvv.top/gtwgiukvlg.html

TS:   // 同 JS
来源：http://hz.hysaishi.cn/gtfaideirw.html

Java: new Thread(() -> f()).start()
来源：http://hz.jinqigfzy.top/gtjvmjwvbi.html

Go:   go f()
来源：http://hz.0kj1m.cn/gtjtiecnys.html

Ruby: Thread.new { f }
来源：http://hz.nanxinkj.top/gtjkoujfup.html

C#:   Task.Run(() => F());
来源：http://hz.xingfuxueyuan.xyz/gtidsvvcxz.html

[O02] 使用线程池
来源：http://hz.zdqjudy.top/gtfvwknaqp.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yj202588.top/gtcmzlojhd.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.feifeiyinyue.top/gtfgryznjm.html

JS:   // worker_threads 线程池
来源：http://hz.jinghuilouyu.cn/gtabyzaszr.html

TS:   // worker_threads 线程池
来源：http://hz.wangdashe.top/gtgtwzkcem.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yangfankeji.com/gtptswgrgo.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yj20258.top/gtehcwmkgu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.ivvv.top/gtzdcjhufb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.quarkkingdee.top/gtxtlqwoqn.html

[O03] 加锁保护共享数据
来源：http://hz.zhiwuduotai.top/gtehhrmvkl.html

Py:   with lock: shared += 1
来源：http://hz.mhx1999.top/gtxxhmabdz.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.kuanghao11.cn/gtdefnncwh.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.hongshengwenyu.top/gtmxucwspj.html

TS:   // 同 JS
来源：http://hz.9152youxi.cn/gtftajtlik.html

Java: synchronized (this) { shared++; }
来源：http://hz.sweek.top/gtswthderi.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yonumen.top/gtqetojavg.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.yangfankeji.com/gtrirhcxms.html

C#:   lock (gate) { shared++; }
来源：http://hz.cucudq.cn/gtxcncedhi.html

[O04] 定义异步函数并等待
来源：http://hz.zycfv.cn/gtrufarwqn.html

Py:   async def f():⏎    await g()
来源：http://hz.nanxuanxn.top/gtqosbggze.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.zhaomingkeji.xyz/gtxpysmtgx.html

JS:   async function f() { await g(); }
来源：http://hz.quarkkingdee.top/gtsujrsjrp.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.bjfxy.top/gtxnrtwyru.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.svipenyu.cn/gtuxxzugec.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.0kj1m.cn/gtqxaxxgan.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.jlsjyb.cn/gtmhrbrezq.html

C#:   async Task F() { await G(); }
来源：http://hz.yj20258.top/gtgvrbahcc.html

[O05] 并发执行并等待全部完成
来源：http://hz.hysaishi.cn/gtqahccwnd.html

Py:   asyncio.gather(*tasks)
来源：http://hz.ehwqpu.com/gtvyotijrs.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.shzxlz.cn/gtliqfpzdj.html

JS:   await Promise.all(tasks)
来源：http://hz.316326.xyz/gthymrppui.html

TS:   await Promise.all(tasks)
来源：http://hz.gotoacloud.top/gtozridkas.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.mhx1999.top/gthfdqefsy.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.gaohongyu789.top/gtytpiqglx.html

Ruby: threads.map(&:join)
来源：http://hz.jqgufenzy.top/gtgjwzkwym.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.meibo888.top/gttlskcero.html

[O06] 使用进程池
来源：http://hz.svipenyu.cn/gtzvqnrqfo.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.fzhhl.top/gtvdogahwc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.fengsongda.top/gtfljyiwwo.html

JS:   // child_process / cluster 模块
来源：http://hz.52xcode.cn/gtyjjruzhg.html

TS:   // child_process / cluster 模块
来源：http://hz.aizwys.cn/gtpjrzbrxw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.svipenyu.cn/gtrughrliy.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.andypj.xyz/gtvstvcekg.html

Ruby: // fork 块
来源：http://hz.chenzaomai.com/gtbfgfgqxw.html

C#:   Parallel.For
来源：http://hz.316326.xyz/gtfnlpaxjb.html

================================================================================
来源：http://hz.ydjk.org.cn/gtpfbdpzwa.html

P. 常用工具函数
来源：http://hz.vqdsnc.cn/gtjtxsqbjn.html

================================================================================
来源：http://hz.pycfn.com/gtqosnnqqx.html

[P01] 生成 UUID
来源：http://hz.sufxvd.cn/gtlgasmane.html

Py:   str(uuid.uuid4())
来源：http://hz.yj20258888.top/gtkewbotsr.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.dashuyun.cn/gtivsupotn.html

JS:   crypto.randomUUID()
来源：http://hz.jinghuilouyu.cn/gtlbrikuqv.html

TS:   crypto.randomUUID()
来源：http://hz.tianlin.xyz/gtzwvnjugs.html

Java: UUID.randomUUID().toString()
来源：http://hz.zycfv.cn/gtvmaaldyq.html

Go:   // 用 github.com/google/uuid
来源：http://hz.fzhhl.top/gtlqiflqxr.html

Ruby: SecureRandom.uuid
来源：http://hz.daxiang520.top/gtmlgogkky.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.aizwys.cn/gtyvnvlxcr.html

[P02] MD5 / SHA256 摘要
来源：http://hz.andypj.xyz/gtgelzjalx.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.jyoumei.cn/gtanjausrz.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.redwolf501.top/gtvefjwckw.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.shuidangran.top/gtsilcfgzv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.hysaishi.cn/gtkxisimrt.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.cqqwz.cn/gtdptozrjf.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.ehwqpu.com/gtazwjkbam.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.yvedp.cn/gtwasqxmby.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.guowangkeji.top/gtcbulpqtu.html

[P03] 生成短随机字符串
来源：http://hz.zycfv.cn/gtmsqckveh.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.zhiwuduotai.top/gtmkyejazn.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.bjfxy.top/gtnmfidjks.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jinyuanbaomall.cn/gtycfwofqy.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hywenlv.cn/gtzdmrvusc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.nanxuanxn.top/gtvskofldb.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.tianlin.xyz/gtmbpelycs.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.zhongyouzk.top/gtjeokbbbh.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.andypj.xyz/gtjbzuxxnj.html

[P04] 求长度
来源：http://hz.shanyushiyangtech.top/gtqhvhiueh.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.fzhhl.top/gtfihqgwag.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.vqdsnc.cn/gtvnzbjwyl.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hysaishi.cn/gtcuwvozrl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.mhx1999.top/gtnnygrkay.html

Java: list.size();  map.size();  s.length()
来源：http://hz.smart0.xyz/gtlbowlntk.html

Go:   len(arr);  len(m)
来源：http://hz.yj20258888.top/gtdugssqgo.html

Ruby: x.length;  x.size
来源：http://hz.ydzc1.top/gtuggsunpm.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.sweek.top/gtlxtdwexd.html

[P05] 判断两个对象内容是否相等
来源：http://hz.sysykeji.top/gtuqnrcnyo.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.feifeiyinyue.top/gtdqlengce.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.daxiang520.top/gtjmadkuru.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.jinghuilouyu.cn/gtorczlokx.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zdqjudy.top/gtvptltfcq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.zycfv.cn/gtikwcimam.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.xylfe.cn/gtiwhnoyhi.html

Ruby: a == b
来源：http://hz.redwolf501.top/gtckwmwsud.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.cucudq.cn/gtpqagtwwo.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.xziqi.cn/gtwsbqudos.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.yj20258888.top/gtfhxgrdds.html

PHP:  if (empty($x)) {}
来源：http://hz.yj20258888.top/gtcxbrzxsg.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.yj20258.top/gtpqcjwdtb.html

TS:   if (x == null) {}
来源：http://hz.snrcjt.cn/gtpndoehqn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.tian-w.cn/gtsuhnndmo.html

Go:   if x == nil {}
来源：http://hz.hongshengwenyu.top/gtdenvljtf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.quarkkingdee.top/gtjmftqxkm.html

C#:   if (x is null) {}
来源：http://hz.gotoacloud.top/gtzfxguphk.html

[P07] 防抖与节流
来源：http://hz.jiagoushi.top/gtbkdhesyw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.andypj.xyz/gtvsmypgjd.html

PHP:  // 手写时间戳比较
来源：http://hz.chenlongwang.top/gtouyofdqt.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yongpay.top/gtgqpewoql.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhiwuduotai.top/gtjcwoibgw.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.cqqwz.cn/gtklorxhle.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.yj20258.top/gtyyqopgzd.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.316326.xyz/gtrljompmo.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.xinyue.icu/gtbuyzsvow.html

[P08] 处理浮点精度问题
来源：http://hz.ydzc1.top/gtmdbpnfuy.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.tanke756.top/gtzrhuabeq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.andypj.xyz/gtdyqjnaxs.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.ivvv.top/gtsqgdfost.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.shanyushiyangkeji.top/gtiiryvzio.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yangfankeji.com/gtfvcjjwse.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.jqgufenzy.top/gtnhnvmigw.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.daria6918.cn/gtwqfkxouq.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.yongpay.top/gtzlbygnyp.html

================================================================================
来源：http://hz.hammf.cn/gtkanuzndc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.havefunace.top/gtnhstccvb.html

================================================================================
来源：http://hz.xinyue.icu/gtzftigzpp.html

[Q01] 创建表
来源：http://hz.yuxming.cn/gtlvjcpxot.html

CREATE TABLE users (
来源：http://hz.hnqzz.top/gthufuvack.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.feifeiyinyue.top/gtqeehonfd.html

name VARCHAR(50) NOT NULL,
来源：http://hz.sufxvd.cn/gtcngnenlx.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jqgfzy.top/gtrfilwmyu.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.tianlin.xyz/gtxjrfimak.html

);
来源：http://hz.sufxvd.cn/gtmkyckhgk.html

[Q02] 创建带外键的表
来源：http://hz.0kj1m.cn/gtcwgsyzie.html

CREATE TABLE orders (
来源：http://hz.guannengcc.top/gtuykbdvou.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yj20258.top/gtmxmdautr.html

user_id INT NOT NULL,
来源：http://hz.shangyingyoupin.top/gtdxqjtavn.html

amount DECIMAL(10, 2),
来源：http://hz.pengpengdd.cyou/gtsbjwvbsb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.jlsjyb.cn/gtlndglfym.html

);
来源：http://hz.sxryk.cn/gtnezvbtdi.html

[Q03] 增加列
来源：http://hz.xylfe.cn/gttgmecohl.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.chenjidiqi.icu/gtgarlvode.html

[Q04] 修改列类型
来源：http://hz.daxiang520.top/gtjqzmbnqv.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.tanke756.top/gtthmxinhi.html

[Q05] 重命名列
来源：http://hz.316326.xyz/gtrprqvgdb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.gzhubu.top/gtqnzzwysi.html

[Q06] 删除列
来源：http://hz.haohaochexian.top/gtzowgaalh.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.quarkkingdee.top/gtvpewczpr.html

[Q07] 删除表
来源：http://hz.52xcode.cn/gtmkygkehm.html

DROP TABLE IF EXISTS orders;
来源：http://hz.bjfxy.top/gtepluplbb.html

[Q08] 创建普通索引
来源：http://hz.kuanghao11.cn/gtsojgucub.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.316326.xyz/gtxgykmsre.html

[Q09] 创建唯一索引
来源：http://hz.ydjk.org.cn/gtfddnvqac.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.jianghu66.top/gtysraimns.html

[Q10] 插入单行
来源：http://hz.xinyue.icu/gtyijkqdap.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.hnqzz.top/gthbclmbmf.html

[Q11] 一次插入多行
来源：http://hz.zhengqikj.top/gtbkpxhiwj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.svipenyu.cn/gtoimsoqvb.html

[Q12] 插入后取自增 ID
来源：http://hz.svipenyu.cn/gtguoeqkwh.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.zhengqikj.top/gtkvqsretj.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.birdmap.top/gtwepwhexj.html

[Q13] 忽略重复插入
来源：http://hz.tanke756.top/gtntvirxac.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.fengsongda.top/gtbgrfcvnv.html

[Q14] 存在则更新（upsert）
来源：http://hz.jinqigufen.top/gtgeygbzrw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.sysykeji.top/gtldxdodbx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.yanxiufei.cn/gtpwvqpjef.html

[Q15] 查询全部
来源：http://hz.yangfankeji.com/gtgfalevqv.html

SELECT * FROM users;
来源：http://hz.zdqjudy.top/gtpbigfnyc.html

[Q16] 查询指定列
来源：http://hz.xinyue.icu/gtdvupgfwy.html

SELECT id, name FROM users;
来源：http://hz.dashuyun.cn/gtgfmmugmc.html

[Q17] 条件查询
来源：http://hz.nwbrower.top/gtpsggfvtx.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.kuanghao11.cn/gtpwxotlal.html

[Q18] 模糊匹配
来源：http://hz.yuanzhike.top/gtjmsatyhk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.hywenlv.cn/gtzamispmt.html

[Q19] 范围查询
来源：http://hz.iojbl.cn/gtijllcplu.html


<!-- 参考信息 -->