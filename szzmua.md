代发 wailian999

TS:   process.platform;  process.version
来源：http://hz.xuanzx.com/gtsvoofcwz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.aizwys.cn/gtxqxhllkn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.cdnleiting.top/gtpojoueme.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.smart0.xyz/gtfzdreoho.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.chenlongwang.top/gtoaykatbg.html

================================================================================
来源：http://hz.zhoulong.xyz/gtefcnzsfy.html

N. 数据结构与算法
来源：http://hz.hywenlv.cn/gtozqnmuiw.html

================================================================================
来源：http://hz.hysaishi.cn/gtdbejrqmp.html

[N01] 二分查找（有序数组）
来源：http://hz.bjfxy.top/gtbdovzvzl.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.svipenyu.cn/gtgtbnkmzx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.cqqwz.cn/gttpgmltrn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.kuanghao11.cn/gtqqwttcbr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.sxryk.cn/gtgsjlxhrt.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.xuetiantiany.cn/gtrivzdwyd.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.bjfxy.top/gtiweihyoh.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.smart0.xyz/gtpyxlkvqg.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.wangshuangyany.cn/gtrrogouau.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.hysaishi.cn/gtjhkgndpk.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yuanzhike.top/gtfetksmxp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.gotoacloud.top/gtuxmoaksj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.kuanghao11.cn/gttcancwla.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.andypj.xyz/gtrkddgnbt.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.redwolf501.top/gtrbnoevje.html

Go:   slices.Sort(arr)
来源：http://hz.yongpay.top/gtvlomwnih.html

Ruby: arr.sort
来源：http://hz.shuidangran.top/gtvehlkfsa.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.cheryme.top/gtpnbpkwjv.html

[N03] 快速排序（分治示例）
来源：http://hz.dianchejie.cn/gtmxidewzt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.wangdashe.top/gtznutcbyn.html

PHP:  // 递归实现，或用 usort
来源：http://hz.xylfe.cn/gtybnwkqtz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.dianchejie.cn/gtqiawoein.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.shangyingyoupin.top/gtvomhpnhv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.nanxinkj.top/gtmicjgtgr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.zhengqikj.top/gtvvwfefgz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.sxryk.cn/gtestcqesq.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.nanxuanxn.top/gtoghnkjuu.html

[N04] 斐波那契数列
来源：http://hz.316326.xyz/gtedcbmcwj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.shzxlz.cn/gtjmbzfyfw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.ivvv.top/gteyhqmfva.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.birdmap.top/gtkdzgvsty.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jinghuilouyu.cn/gtrkojcljw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.shzxlz.cn/gtupgkczvw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.hongshengwenyu.top/gtbypqfedn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.guowangkeji.top/gtabtufkxp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.cdnleiting.top/gtwgjvzmzh.html

[N05] 最大公约数
来源：http://hz.cheryme.top/gtvynbtlgf.html

Py:   math.gcd(a, b)
来源：http://hz.chenjidiqi.icu/gtzadsrmix.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.aizwys.cn/gtdhmmzqsh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ehwqpu.com/gtfmcuznuj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yongpay.top/gtiiqmsrtm.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.xinyue.icu/gtgwhfmots.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.fengsongda.top/gtupnnlxxj.html

Ruby: a.gcd(b)
来源：http://hz.yanxiufei.cn/gtkxcjcbrb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.aibaodan.cn/gtzcmrezgs.html

[N06] 判断回文字符串
来源：http://hz.ppjwa.cn/gtefiyshrw.html

Py:   s == s[::-1]
来源：http://hz.zhengqikj.top/gtcdrbfzqf.html

PHP:  $s === strrev($s);
来源：http://hz.zycfv.cn/gtmaklpoxs.html

JS:   s === [...s].reverse().join("")
来源：http://hz.hnxiangtu.top/gtpgqpumvg.html

TS:   s === [...s].reverse().join("")
来源：http://hz.cqqwz.cn/gtmpsqatrk.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.cucudq.cn/gtvzuktiqu.html

Go:   // 双指针从两端比较
来源：http://hz.shzxlz.cn/gtpzzadgua.html

Ruby: s == s.reverse
来源：http://hz.zhongyouzk.top/gtsxmftcpq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.shangyingyoupin.top/gthgzyjkrs.html

[N07] 两数之和（返回下标）
来源：http://hz.tianlin.xyz/gtqffqgbhu.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.nanxinkj.top/gtqllmvfgm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.jinyuanbaomall.cn/gtssianzwe.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.hnxiangtu.top/gthfrracjj.html

TS:   // 手写 Map<string, number>
来源：http://hz.yj20258888.top/gtdqzgtzpn.html

Java: // 手写 HashMap
来源：http://hz.cqqwz.cn/gtcvxlusnu.html

Go:   // 手写 map[int]int
来源：http://hz.sysykeji.top/gtkjmoozlq.html

Ruby: // 手写 Hash
来源：http://hz.zhijiandao.cn/gtntwtfair.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yueranfly.top/gtpyfsnqfw.html

[N08] 生成全排列
来源：http://hz.cucudq.cn/gtpznikein.html

Py:   itertools.permutations(arr)
来源：http://hz.gogol.net.cn/gtocvhlsiz.html

PHP:  // 手写递归交换
来源：http://hz.guannengcc.top/gtxdvkuvbm.html

JS:   // 手写回溯递归
来源：http://hz.shanyushiyangkeji.top/gtqyweelxc.html

TS:   // 手写回溯递归
来源：http://hz.jlsjyb.cn/gtubhzysoj.html

Java: // 手写回溯递归
来源：http://hz.gotoacloud.top/gthwnmrfbt.html

Go:   // 手写回溯递归
来源：http://hz.cqqwz.cn/gtksspmttx.html

Ruby: arr.permutation.to_a
来源：http://hz.kuanghao11.cn/gtebugjspj.html

C#:   // 手写回溯递归
来源：http://hz.xuetiantiany.cn/gtmptulrjv.html

[N09] 栈与队列
来源：http://hz.nanxinkj.top/gtxhmuddvc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yj20258.top/gtsbxkkmdk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.jlsjyb.cn/gturauhfrg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.aizwys.cn/gtstzttalz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.haohaochexian.top/gtkyqdfznf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.ydjk.org.cn/gtypinkyvc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.daxiang520.top/gtpqwsmmgh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yangfankeji.com/gttdeqsdbq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.shanyushiyangtech.top/gtzkwlbhoi.html

[N10] 链表节点定义
来源：http://hz.yuxming.cn/gttiwrlrhs.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.shuidangran.top/gtwdioswoq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.yvedp.cn/gtirbxwxuq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.ybcxt.top/gtdnvtqwlt.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.xuetiantiany.cn/gtdkcwrutk.html

Java: class Node { int v; Node next; }
来源：http://hz.daria6918.cn/gtvomrunvk.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.hysaishi.cn/gtylgxerwa.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.svipenyu.cn/gtwjdpczvf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.ivvv.top/gtmnyvmbhz.html

[N11] 二叉树中序遍历
来源：http://hz.zhoulong.xyz/gtsfsmoxsg.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.ywan-chungtsiang.top/gtqthtijhw.html

PHP:  // 手写递归函数
来源：http://hz.xuanzx.com/gtncvldsfi.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.cashguo.top/gtechbnzkg.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.nanxinkj.top/gtzyiomjvk.html

Java: // 手写递归
来源：http://hz.jiagoushi.top/gtrgyodekk.html

Go:   // 手写递归
来源：http://hz.hammf.cn/gtahfvpugu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.yj20258888.top/gtvajjotvw.html

C#:   // 手写递归
来源：http://hz.nanxinkj.top/gtyrhraaht.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.wangshuangyany.cn/gtvrljfnbg.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.316326.xyz/gtkewjevgu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.daria6918.cn/gttlqzsonl.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hywenlv.cn/gtilavnwpo.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.birdmap.top/gtogtarmui.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.snrcjt.cn/gtthtfzgfa.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.svipenyu.cn/gtecerdtmd.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.yj202588.top/gtoomelvrp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xuetiantiany.cn/gtynzcoudw.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtlixoqmwz.html

O. 并发与异步
来源：http://hz.ydzc1.top/gtgzhgtklj.html

================================================================================
来源：http://hz.snrcjt.cn/gtqvnpbjqg.html

[O01] 启动一个线程
来源：http://hz.gogol.net.cn/gtkoefymob.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.9152youxi.cn/gtqxrelfsv.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.jqgfzy.top/gtlmziukji.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.ivvv.top/gtxavabylc.html

TS:   // 同 JS
来源：http://hz.daxiang520.top/gtcuzpvuti.html

Java: new Thread(() -> f()).start()
来源：http://hz.chenlongwang.top/gtxowoqqeu.html

Go:   go f()
来源：http://hz.gogol.net.cn/gtuunswgqd.html

Ruby: Thread.new { f }
来源：http://hz.gaohongyu789.top/gtyzwnohvo.html

C#:   Task.Run(() => F());
来源：http://hz.yuanzhike.top/gtsykvgafr.html

[O02] 使用线程池
来源：http://hz.jiagoushi.top/gtneygqmhy.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.zhaomingkeji.xyz/gtsrjfymte.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.0kj1m.cn/gtpgtsvwtp.html

JS:   // worker_threads 线程池
来源：http://hz.dashuyun.cn/gtkfmfkxya.html

TS:   // worker_threads 线程池
来源：http://hz.xingfuxueyuan.xyz/gtzebsiohl.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.tianlin.xyz/gtyxbdbwmy.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.jinqigufen.top/gtabzzlmbs.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.guowangkeji.top/gtxswypvaz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.jqgfzy.top/gthcbfyjxp.html

[O03] 加锁保护共享数据
来源：http://hz.jinqigufen.top/gtrhvnqgho.html

Py:   with lock: shared += 1
来源：http://hz.guannengcc.top/gtwohkxevz.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.dianchejie.cn/gtvwkgnuln.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.ehwqpu.com/gtdoczdzyv.html

TS:   // 同 JS
来源：http://hz.wangdashe.top/gtlqfmtwmd.html

Java: synchronized (this) { shared++; }
来源：http://hz.tianlin.xyz/gtlktvqgoj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.jiagoushi.top/gtnzcccuxz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.cqqwz.cn/gtkrtepnsw.html

C#:   lock (gate) { shared++; }
来源：http://hz.yangfankeji.com/gtvdvzleae.html

[O04] 定义异步函数并等待
来源：http://hz.chenjidiqi.icu/gtyixydxhb.html

Py:   async def f():⏎    await g()
来源：http://hz.jinghuilouyu.cn/gtorhmdcli.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.yj20258888.top/gtlydwflnr.html

JS:   async function f() { await g(); }
来源：http://hz.shuidangran.top/gteflovtjk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.ydjk.org.cn/gtpoyvmksr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.yonumen.top/gtlcqrkokc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.yuanzhike.top/gtdlxtymeb.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.chenzaomai.com/gtlsxbgzys.html

C#:   async Task F() { await G(); }
来源：http://hz.pengpengdd.cyou/gtvqyhwywr.html

[O05] 并发执行并等待全部完成
来源：http://hz.zhongyouzk.top/gtdkltqfgh.html

Py:   asyncio.gather(*tasks)
来源：http://hz.yuanzhike.top/gthzxkpnvz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.yvedp.cn/gtzkhlmtfg.html

JS:   await Promise.all(tasks)
来源：http://hz.yonumen.top/gtmiqnrqmv.html

TS:   await Promise.all(tasks)
来源：http://hz.hnxiangtu.top/gtynzwfukt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.meibo888.top/gtduzxcygp.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.guannengcc.top/gtsoihdojx.html

Ruby: threads.map(&:join)
来源：http://hz.jinghuilouyu.cn/gtlwwvgwow.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.shzxlz.cn/gtkckminma.html

[O06] 使用进程池
来源：http://hz.yongpay.top/gtherhuhcf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.ybcxt.top/gtgdjvnvkw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.ivvv.top/gtkqsozbil.html

JS:   // child_process / cluster 模块
来源：http://hz.daria6918.cn/gtgxyzqtpo.html

TS:   // child_process / cluster 模块
来源：http://hz.cqqwz.cn/gtwjyszgyr.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jlsjyb.cn/gtgulqtqhu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.yj20258.top/gtqsvjudfh.html

Ruby: // fork 块
来源：http://hz.gotoacloud.top/gtfpjcpvlg.html

C#:   Parallel.For
来源：http://hz.shangyingyoupin.top/gtlrgnnacv.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtxdmbbsoq.html

P. 常用工具函数
来源：http://hz.9152youxi.cn/gtbaimddie.html

================================================================================
来源：http://hz.jqgufenzy.top/gtctlloirx.html

[P01] 生成 UUID
来源：http://hz.vqdsnc.cn/gtzttkautg.html

Py:   str(uuid.uuid4())
来源：http://hz.jinqigufen.top/gtxdhkuhxn.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jinqigfzy.top/gtzpeqsijc.html

JS:   crypto.randomUUID()
来源：http://hz.yueranfly.top/gtyrxvmlyn.html

TS:   crypto.randomUUID()
来源：http://hz.c1oappe.top/gtfcogydia.html

Java: UUID.randomUUID().toString()
来源：http://hz.shanyushiyangkeji.top/gtpskqfrqb.html

Go:   // 用 github.com/google/uuid
来源：http://hz.pycfn.com/gtduqvfowm.html

Ruby: SecureRandom.uuid
来源：http://hz.jinqigfzy.top/gtusnmoasn.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.jinqigufen.top/gtzxzvhffm.html

[P02] MD5 / SHA256 摘要
来源：http://hz.hywenlv.cn/gtlscpkyft.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.birdmap.top/gtngzpidto.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.shanyushiyangkeji.top/gtjqscbuhf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.52xcode.cn/gtrsrjvrkn.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.gzhubu.top/gtptypcqjb.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.zhijiandao.cn/gtulzmpacm.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.yj202588.top/gtodqtoyzr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.yanxiufei.cn/gtbxfktslk.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yuanzhike.top/gtdwbqykrd.html

[P03] 生成短随机字符串
来源：http://hz.tianlin.xyz/gtypjlkbjp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jianghu66.top/gtnebiddpk.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.zhoulong.xyz/gtplfmcfxc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jinqigfzy.top/gtehjlogaf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yueranfly.top/gtbpiduzro.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.dashuyun.cn/gtzbofaqhy.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.haohaochexian.top/gtnfpufsku.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.fzhhl.top/gtqtjkdzws.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.daria6918.cn/gtgkzwngoc.html

[P04] 求长度
来源：http://hz.zhengqikj.top/gtmpfecdhk.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.cucudq.cn/gtzkcxxzru.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yangfankeji.com/gtgrektjjd.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.shangyingyoupin.top/gtcmnfpbpr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ybcxt.top/gtzbwngrpo.html

Java: list.size();  map.size();  s.length()
来源：http://hz.9152youxi.cn/gtzosiqgnn.html

Go:   len(arr);  len(m)
来源：http://hz.yvedp.cn/gtjnzwbhiq.html

Ruby: x.length;  x.size
来源：http://hz.kuanghao11.cn/gthvvobpev.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.dashuyun.cn/gtetglohxw.html

[P05] 判断两个对象内容是否相等
来源：http://hz.yonumen.top/gtcparepnk.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.shanyushiyangkeji.top/gtwfmhwacy.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.cqqwz.cn/gtpkjjcmeu.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.yj202588.top/gtqgnelczy.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.svipenyu.cn/gtjpnevwii.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.xuanzx.com/gtmmsgulna.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.0kj1m.cn/gtyoplcuhk.html

Ruby: a == b
来源：http://hz.chenlongwang.top/gtmipwlbwi.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.guowangkeji.top/gtcfgdggip.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.chenlongwang.top/gtuchziblu.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.9152youxi.cn/gtbrwckkow.html

PHP:  if (empty($x)) {}
来源：http://hz.shanyushiyangkeji.top/gtvrkipqsf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.ydjk.org.cn/gtdjljkeis.html

TS:   if (x == null) {}
来源：http://hz.daria6918.cn/gtlmqwauck.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.nanxuanxn.top/gtwlzradoh.html

Go:   if x == nil {}
来源：http://hz.cheryme.top/gtqizkvkps.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jinyuanbaomall.cn/gtsexwblwj.html

C#:   if (x is null) {}
来源：http://hz.hywenlv.cn/gtnpzxfmyo.html

[P07] 防抖与节流
来源：http://hz.bjfxy.top/gtaixfrpmn.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.xinyue.icu/gtsczkqadq.html

PHP:  // 手写时间戳比较
来源：http://hz.gzhubu.top/gtaacxdxgw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.quarkkingdee.top/gtkisdhglu.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cucudq.cn/gtzqrptwjm.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.kuanghao11.cn/gtlqwqzsyu.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.hammf.cn/gtjnpzguvx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.cashguo.top/gtdfagubxl.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.xinyue.icu/gtglxcypji.html

[P08] 处理浮点精度问题
来源：http://hz.pengpengdd.cyou/gtriisxgya.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.sufxvd.cn/gtyoxrpoar.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.aizwys.cn/gtfyncawgr.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.gaohongyu789.top/gttvxjyjtk.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.dianchejie.cn/gtnetjwich.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.ydzc1.top/gtwlfjwjvz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.jqgfzy.top/gtbbhkwnuq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.guowangkeji.top/gtoytimvbu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.wangdashe.top/gtmdxqvffr.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtvihwgrpv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.pengpengdd.cyou/gtusgvodbn.html

================================================================================
来源：http://hz.dashuyun.cn/gtcjggwjlh.html

[Q01] 创建表
来源：http://hz.wangshuangyany.cn/gtfemvquln.html

CREATE TABLE users (
来源：http://hz.hysaishi.cn/gtauhkehzc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yj20258.top/gttxkkdwlq.html

name VARCHAR(50) NOT NULL,
来源：http://hz.zhiwuduotai.top/gtjvernyhc.html

email VARCHAR(100) UNIQUE,
来源：http://hz.zdqjudy.top/gtaoxfheef.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.tianlin.xyz/gtyhxtutya.html

);
来源：http://hz.xingfuxueyuan.xyz/gttbgzlfqh.html

[Q02] 创建带外键的表
来源：http://hz.cheryme.top/gtecdwgukj.html

CREATE TABLE orders (
来源：http://hz.xingfuxueyuan.xyz/gtptdjpawd.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.gotoacloud.top/gtkcegzukv.html

user_id INT NOT NULL,
来源：http://hz.shanyushiyangtech.top/gtnqvoibba.html

amount DECIMAL(10, 2),
来源：http://hz.aibaodan.cn/gtcnnrjdcw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.pycfn.com/gtlduzynyb.html

);
来源：http://hz.shzxlz.cn/gtxltdruyj.html

[Q03] 增加列
来源：http://hz.xingfuxueyuan.xyz/gtwxsezclx.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.sxryk.cn/gtkpueupkw.html

[Q04] 修改列类型
来源：http://hz.svipenyu.cn/gtmaoafvmi.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.havefunace.top/gtgquhwdar.html

[Q05] 重命名列
来源：http://hz.shuidangran.top/gtfuskhsic.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.havefunace.top/gtmumsogdg.html

[Q06] 删除列
来源：http://hz.jinghuilouyu.cn/gtaistufpu.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.zhiwuduotai.top/gtulcwqqky.html

[Q07] 删除表
来源：http://hz.gzhubu.top/gtyuyrpnwz.html

DROP TABLE IF EXISTS orders;
来源：http://hz.gogol.net.cn/gtwachuntx.html

[Q08] 创建普通索引
来源：http://hz.hammf.cn/gtqcbkpbmc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.redwolf501.top/gthxcbcimd.html

[Q09] 创建唯一索引
来源：http://hz.hfpthk.cn/gtdqktywri.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.pycfn.com/gtsiedgjab.html

[Q10] 插入单行
来源：http://hz.haohaochexian.top/gtelmrkedq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.havefunace.top/gtjmmfepfe.html

[Q11] 一次插入多行
来源：http://hz.gaohongyu789.top/gtrhtvbhiy.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.gaohongyu789.top/gtmrckfarh.html

[Q12] 插入后取自增 ID
来源：http://hz.jiagoushi.top/gthmdjssul.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.tian-w.cn/gtonzzikxq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.jinqigfzy.top/gtpyalkhae.html

[Q13] 忽略重复插入
来源：http://hz.yj202588.top/gtpnmsksyv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.sweek.top/gtyehlaalx.html

[Q14] 存在则更新（upsert）
来源：http://hz.gotoacloud.top/gtmguqccjn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.sufxvd.cn/gtylnzhehg.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.haohaochexian.top/gtsbejzvdp.html

[Q15] 查询全部
来源：http://hz.wangdashe.top/gtfaunnmsq.html

SELECT * FROM users;
来源：http://hz.jyoumei.cn/gtckkevmic.html

[Q16] 查询指定列
来源：http://hz.andypj.xyz/gtsfkgenpv.html

SELECT id, name FROM users;
来源：http://hz.0kj1m.cn/gtevsjklrp.html

[Q17] 条件查询
来源：http://hz.jinyuanbaomall.cn/gtgrkzwtjt.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.redwolf501.top/gtqqytbytr.html

[Q18] 模糊匹配
来源：http://hz.daxiang520.top/gttlzrgbhc.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yonumen.top/gthmupfkeh.html

[Q19] 范围查询
来源：http://hz.hfpthk.cn/gtrqvqfcyf.html


<!-- 参考信息 -->