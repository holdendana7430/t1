代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.daria6918.cn/gtmujdrwjb.html

================================================================================
来源：http://hz.9152youxi.cn/gtgkrddevl.html

N. 数据结构与算法
来源：http://hz.birdmap.top/gtfgmlvmlz.html

================================================================================
来源：http://hz.hfpthk.cn/gtmudqgyuv.html

[N01] 二分查找（有序数组）
来源：http://hz.gzhubu.top/gtbaiwooct.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.guowangkeji.top/gtbtelbaot.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.dianchejie.cn/gtddihyatf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.gaohongyu789.top/gtzfmtexht.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.vqdsnc.cn/gtrbmpcmsb.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.gaohongyu789.top/gtopbefxgb.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.haohaochexian.top/gtcsihlcvr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.hammf.cn/gtbvekfmcu.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.gogol.net.cn/gtuwnlbxxf.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.daria6918.cn/gtkbukpzjs.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.pengpengdd.cyou/gtqotwlebo.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.birdmap.top/gtbtydlndi.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yueranfly.top/gticruhvqq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.cucudq.cn/gtcffhjheu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.zycfv.cn/gtryifyfpd.html

Go:   slices.Sort(arr)
来源：http://hz.tian-w.cn/gtbzxnumwv.html

Ruby: arr.sort
来源：http://hz.sysykeji.top/gtmynbzehy.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.quarkkingdee.top/gtoedahiwj.html

[N03] 快速排序（分治示例）
来源：http://hz.chenjidiqi.icu/gtchgafggx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.bjfxy.top/gtpxafcuiu.html

PHP:  // 递归实现，或用 usort
来源：http://hz.fzhhl.top/gtzjhhpoak.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.wangshuangyany.cn/gtznlrohgi.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.guowangkeji.top/gtxwgyocry.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.pengpengdd.cyou/gtqzjvpycr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.9152youxi.cn/gtfduyvxnk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.jqgfzy.top/gtmwwrfmao.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.ydjk.org.cn/gtuincxlpv.html

[N04] 斐波那契数列
来源：http://hz.hysaishi.cn/gtxqjajfuv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.guowangkeji.top/gtjvostcij.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.feifeiyinyue.top/gtsvetdzqc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.cdnleiting.top/gtztpyvryg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.wangdashe.top/gtvnuikitw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yuanzhike.top/gtezqsqyxs.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.sysykeji.top/gtqxfohify.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.shanyushiyangkeji.top/gtybcadjfi.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.gzhubu.top/gtrhqwaaxi.html

[N05] 最大公约数
来源：http://hz.hfpthk.cn/gtwtqlqmex.html

Py:   math.gcd(a, b)
来源：http://hz.smart0.xyz/gtivbyvzal.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.hywenlv.cn/gtukbyurfz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.chenlongwang.top/gtfqsjskrb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hysaishi.cn/gtvofuwdou.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.ivvv.top/gtdlpxfrzg.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.xingfuxueyuan.xyz/gtofssfort.html

Ruby: a.gcd(b)
来源：http://hz.yj20258888.top/gtxszpdmqb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.gaohongyu789.top/gtrnzrgwgu.html

[N06] 判断回文字符串
来源：http://hz.daxiang520.top/gteyqivijt.html

Py:   s == s[::-1]
来源：http://hz.jyoumei.cn/gtlioscdip.html

PHP:  $s === strrev($s);
来源：http://hz.ivvv.top/gtsmsihfck.html

JS:   s === [...s].reverse().join("")
来源：http://hz.shangyingyoupin.top/gtqvvycoug.html

TS:   s === [...s].reverse().join("")
来源：http://hz.hongshengwenyu.top/gtdjdsxybh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.sxryk.cn/gtxniizamo.html

Go:   // 双指针从两端比较
来源：http://hz.ppjwa.cn/gtmondglea.html

Ruby: s == s.reverse
来源：http://hz.hfpthk.cn/gtqpsmrzvy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.9152youxi.cn/gttnzgvend.html

[N07] 两数之和（返回下标）
来源：http://hz.dashuyun.cn/gtzzrsvbhi.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.yueranfly.top/gtciixeazb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.cashguo.top/gttnuukmtb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.ydzc1.top/gtyeazdein.html

TS:   // 手写 Map<string, number>
来源：http://hz.xuetiantiany.cn/gteimlqnvv.html

Java: // 手写 HashMap
来源：http://hz.yongpay.top/gtpqftgrqp.html

Go:   // 手写 map[int]int
来源：http://hz.ivvv.top/gttpjfdrsi.html

Ruby: // 手写 Hash
来源：http://hz.xingfuxueyuan.xyz/gtrdigdwvy.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.zycfv.cn/gtlhtkujve.html

[N08] 生成全排列
来源：http://hz.sxryk.cn/gtorlshzye.html

Py:   itertools.permutations(arr)
来源：http://hz.yj20258888.top/gtjuagxcdv.html

PHP:  // 手写递归交换
来源：http://hz.dashuyun.cn/gtdpobzbri.html

JS:   // 手写回溯递归
来源：http://hz.gzhubu.top/gtmdfxluul.html

TS:   // 手写回溯递归
来源：http://hz.aizwys.cn/gtzmbzkqev.html

Java: // 手写回溯递归
来源：http://hz.gzhubu.top/gtqisvpjvc.html

Go:   // 手写回溯递归
来源：http://hz.fengsongda.top/gtjodjnhik.html

Ruby: arr.permutation.to_a
来源：http://hz.shangyingyoupin.top/gtqexbxodv.html

C#:   // 手写回溯递归
来源：http://hz.snrcjt.cn/gtzynvegih.html

[N09] 栈与队列
来源：http://hz.yj20258.top/gtaouawvss.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yongpay.top/gtguwfqotg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.cheryme.top/gtrfvzyqhb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.aibaodan.cn/gtsjrmmqmy.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.xziqi.cn/gtzexbkzod.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.jiagoushi.top/gthlcnajih.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.yuanzhike.top/gtomtzqbnu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.daxiang520.top/gtoyiqlkhd.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yj202588.top/gtxxiextoa.html

[N10] 链表节点定义
来源：http://hz.guannengcc.top/gtmzibzawv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.52xcode.cn/gtmuoanofe.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.daxiang520.top/gtuostykwn.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.hammf.cn/gtomnkznjl.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.meibo888.top/gtwkwegryc.html

Java: class Node { int v; Node next; }
来源：http://hz.snrcjt.cn/gtxqoiyaeu.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.sysykeji.top/gtfdgbmkhg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.cashguo.top/gttsintupj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.ydjk.org.cn/gtudowisbz.html

[N11] 二叉树中序遍历
来源：http://hz.quarkkingdee.top/gthxsudvzd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.vqdsnc.cn/gtagejegml.html

PHP:  // 手写递归函数
来源：http://hz.svipenyu.cn/gtywzfxcbc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.haohaochexian.top/gtagmumqah.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.chenjidiqi.icu/gtayksnowu.html

Java: // 手写递归
来源：http://hz.9152youxi.cn/gtemjcbfub.html

Go:   // 手写递归
来源：http://hz.svipenyu.cn/gtowjgeerc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.chenjidiqi.icu/gtlbgeqlyy.html

C#:   // 手写递归
来源：http://hz.zhiwuduotai.top/gthcquycbn.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yangfankeji.com/gtfvqpbzwe.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.guowangkeji.top/gtckbjykjf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.sysykeji.top/gtabbolqll.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zycfv.cn/gtttahqtjl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jinghuilouyu.cn/gtbjarkumw.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hysaishi.cn/gtvvdcyqkf.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.jinqigufen.top/gtjhdegkci.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.jqgufenzy.top/gtwiwvdxql.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jqgufenzy.top/gtbnqylilz.html

================================================================================
来源：http://hz.iojbl.cn/gthgdheews.html

O. 并发与异步
来源：http://hz.jinyuanbaomall.cn/gtmnbhmphc.html

================================================================================
来源：http://hz.ehwqpu.com/gtmrdieypj.html

[O01] 启动一个线程
来源：http://hz.kuanghao11.cn/gthixmygna.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.ydjk.org.cn/gthngumwqz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.birdmap.top/gtlndnlrgq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.iojbl.cn/gtbdtzjtcl.html

TS:   // 同 JS
来源：http://hz.zhixingplan.top/gtamugyjso.html

Java: new Thread(() -> f()).start()
来源：http://hz.jlsjyb.cn/gtrayfgrmv.html

Go:   go f()
来源：http://hz.yanxiufei.cn/gtqsxwuphs.html

Ruby: Thread.new { f }
来源：http://hz.tanke756.top/gtjixofypp.html

C#:   Task.Run(() => F());
来源：http://hz.hysaishi.cn/gtwlanpiyd.html

[O02] 使用线程池
来源：http://hz.ywan-chungtsiang.top/gtefuhgacc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.kuanghao11.cn/gtjidvdkun.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.wangdashe.top/gtkrumgtgy.html

JS:   // worker_threads 线程池
来源：http://hz.sweek.top/gtjxdlbeqj.html

TS:   // worker_threads 线程池
来源：http://hz.yj202588.top/gtvwnjmewn.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.gotoacloud.top/gtmmeihver.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.snrcjt.cn/gtrrpgnsdx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yj20258.top/gtwmtezmfm.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.bjfxy.top/gtcoachmzk.html

[O03] 加锁保护共享数据
来源：http://hz.wangdashe.top/gtdpbccexn.html

Py:   with lock: shared += 1
来源：http://hz.daria6918.cn/gtspzoqbtk.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.andypj.xyz/gtqplbschu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.meibo888.top/gtzlkihxzi.html

TS:   // 同 JS
来源：http://hz.gaohongyu789.top/gtmnwoudwi.html

Java: synchronized (this) { shared++; }
来源：http://hz.52xcode.cn/gthamulyuw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.pycfn.com/gtgxlxfvgf.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.gzhubu.top/gtqxrcylfb.html

C#:   lock (gate) { shared++; }
来源：http://hz.sweek.top/gtyvmtyxax.html

[O04] 定义异步函数并等待
来源：http://hz.dianchejie.cn/gteujqmjkr.html

Py:   async def f():⏎    await g()
来源：http://hz.xingfuxueyuan.xyz/gtnwwnrkpl.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.havefunace.top/gttchrfpbu.html

JS:   async function f() { await g(); }
来源：http://hz.smart0.xyz/gtvaffxjdw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.cdnleiting.top/gtqzuoepev.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.snrcjt.cn/gttzdhrdsl.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.yvedp.cn/gtmkpnzimz.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.mhx1999.top/gtbsqwkogy.html

C#:   async Task F() { await G(); }
来源：http://hz.ywan-chungtsiang.top/gthqvwmlsf.html

[O05] 并发执行并等待全部完成
来源：http://hz.guannengcc.top/gttbslvjzh.html

Py:   asyncio.gather(*tasks)
来源：http://hz.chenzaomai.com/gtwfiepyrx.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.xylfe.cn/gtyvjtxxpm.html

JS:   await Promise.all(tasks)
来源：http://hz.chenjidiqi.icu/gtachncjtk.html

TS:   await Promise.all(tasks)
来源：http://hz.tanke756.top/gtzzwulmkl.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.zhiwuduotai.top/gthubidqez.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.9152youxi.cn/gtybsaflke.html

Ruby: threads.map(&:join)
来源：http://hz.gzhubu.top/gtetdeoqvn.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.dashuyun.cn/gtxkrcyhqw.html

[O06] 使用进程池
来源：http://hz.quarkkingdee.top/gttdgiynxo.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.snrcjt.cn/gtqzodsdsb.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.chenlongwang.top/gtextoinuk.html

JS:   // child_process / cluster 模块
来源：http://hz.yueranfly.top/gtpikhansf.html

TS:   // child_process / cluster 模块
来源：http://hz.ywan-chungtsiang.top/gthcehgqdr.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.ywan-chungtsiang.top/gtqceqbofr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.smart0.xyz/gtxfyqscwl.html

Ruby: // fork 块
来源：http://hz.sxryk.cn/gtrrzvkpdt.html

C#:   Parallel.For
来源：http://hz.shanyushiyangkeji.top/gtcqadpkfy.html

================================================================================
来源：http://hz.zhengqikj.top/gtwxgjvfmb.html

P. 常用工具函数
来源：http://hz.ybcxt.top/gtvkpmsetn.html

================================================================================
来源：http://hz.sweek.top/gtbkwxpcrr.html

[P01] 生成 UUID
来源：http://hz.zdqjudy.top/gtqdlvjmvu.html

Py:   str(uuid.uuid4())
来源：http://hz.sysykeji.top/gtnajbbclr.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.zhijiandao.cn/gtyaskudpr.html

JS:   crypto.randomUUID()
来源：http://hz.shanyushiyangkeji.top/gtxuguyjjl.html

TS:   crypto.randomUUID()
来源：http://hz.kuanghao11.cn/gtgsedjtqq.html

Java: UUID.randomUUID().toString()
来源：http://hz.zhaomingkeji.xyz/gtnnihwhli.html

Go:   // 用 github.com/google/uuid
来源：http://hz.mhx1999.top/gtbyyaurcz.html

Ruby: SecureRandom.uuid
来源：http://hz.hnxiangtu.top/gthbprddzn.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.ybcxt.top/gtnciauniw.html

[P02] MD5 / SHA256 摘要
来源：http://hz.zhijiandao.cn/gtuxgzosie.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.316326.xyz/gtijuwbpvz.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.jinqigufen.top/gtkymiaeel.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.nanxuanxn.top/gtlfikhiwe.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.hnxiangtu.top/gtnbdihsqw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.316326.xyz/gtjdibcsec.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.kuanghao11.cn/gtyaqbtmtf.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.pycfn.com/gthhsecexm.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.xinyue.icu/gtvauanylg.html

[P03] 生成短随机字符串
来源：http://hz.wangdashe.top/gtnypxratl.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.mhx1999.top/gtxamsoayd.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.guowangkeji.top/gtsuqkljaj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ydzc1.top/gtctiesqal.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.0kj1m.cn/gtypbqqqbg.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.ydzc1.top/gtdttiyehb.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.ivvv.top/gtpmvwaovv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.yj20258888.top/gtuynxhksx.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.cashguo.top/gtnqkisozx.html

[P04] 求长度
来源：http://hz.ydzc1.top/gtqhdiipoe.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.hfpthk.cn/gtcmrznbgd.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.nwbrower.top/gtbbwgkknp.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.nanxuanxn.top/gtiexdzimk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.gogol.net.cn/gttphdmirp.html

Java: list.size();  map.size();  s.length()
来源：http://hz.yangfankeji.com/gtqojgrirv.html

Go:   len(arr);  len(m)
来源：http://hz.zhixingplan.top/gtsieubflx.html

Ruby: x.length;  x.size
来源：http://hz.jiagoushi.top/gtdkayuszf.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.redwolf501.top/gtkccsjixv.html

[P05] 判断两个对象内容是否相等
来源：http://hz.jinghuilouyu.cn/gtpqmtkqvu.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.shangyingyoupin.top/gtwvlsedap.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.wangdashe.top/gtfmmeiiub.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.mhx1999.top/gtcuvrgfiw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.xuanzx.com/gtcjeneoja.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.9152youxi.cn/gtwoghjkey.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.ydjk.org.cn/gtuhgtrftn.html

Ruby: a == b
来源：http://hz.xinyue.icu/gtayjxkatp.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.0kj1m.cn/gthnkzfadl.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.xingfuxueyuan.xyz/gtsdqzksvv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.fengsongda.top/gtsgysyelh.html

PHP:  if (empty($x)) {}
来源：http://hz.birdmap.top/gthfhbwpqi.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.316326.xyz/gttecexbnm.html

TS:   if (x == null) {}
来源：http://hz.sweek.top/gtkwbxlaac.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.316326.xyz/gttctapvcy.html

Go:   if x == nil {}
来源：http://hz.316326.xyz/gtizgamqwu.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.xuetiantiany.cn/gtmznxmjqe.html

C#:   if (x is null) {}
来源：http://hz.yueranfly.top/gtysfdanil.html

[P07] 防抖与节流
来源：http://hz.pengpengdd.cyou/gtenfjncsw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.52xcode.cn/gtmritaxyi.html

PHP:  // 手写时间戳比较
来源：http://hz.zhiwuduotai.top/gtoceltdno.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhiwuduotai.top/gtpubtslvq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xinyue.icu/gtkkwjrhrp.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.ydjk.org.cn/gtcpofyszc.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.jinghuilouyu.cn/gtxsubdedu.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yj202588.top/gtavxdqhcj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.tianlin.xyz/gtoxefaaos.html

[P08] 处理浮点精度问题
来源：http://hz.yuanzhike.top/gttvftsfik.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.yangfankeji.com/gtpdhuyive.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.dianchejie.cn/gtqovyriws.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.tanke756.top/gtxftncoso.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.pengpengdd.cyou/gtbndslsif.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.jinqigufen.top/gtoinzccki.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.chenzaomai.com/gtvgnbkgrd.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.chenjidiqi.icu/gtroehzkct.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.haohaochexian.top/gtgomsybdb.html

================================================================================
来源：http://hz.xziqi.cn/gtrwqujiwx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.iojbl.cn/gtsgqnkcss.html

================================================================================
来源：http://hz.cdnleiting.top/gtmtahcdme.html

[Q01] 创建表
来源：http://hz.sweek.top/gtsgxfiyfm.html

CREATE TABLE users (
来源：http://hz.yongpay.top/gtuhgdhxfz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.smart0.xyz/gtvxkrkmjm.html

name VARCHAR(50) NOT NULL,
来源：http://hz.shanyushiyangtech.top/gtwcttokdo.html

email VARCHAR(100) UNIQUE,
来源：http://hz.sufxvd.cn/gtttbwfdry.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.gogol.net.cn/gtyjhfprul.html

);
来源：http://hz.shanyushiyangtech.top/gthpmesijx.html

[Q02] 创建带外键的表
来源：http://hz.meibo888.top/gtsefzxsyh.html

CREATE TABLE orders (
来源：http://hz.wangshuangyany.cn/gtggafyvjq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jiagoushi.top/gtfcaadwtj.html

user_id INT NOT NULL,
来源：http://hz.smart0.xyz/gtzqxdordx.html

amount DECIMAL(10, 2),
来源：http://hz.c1oappe.top/gtiljfviqy.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.aizwys.cn/gtcwrpnrin.html

);
来源：http://hz.vqdsnc.cn/gtrynxyvct.html

[Q03] 增加列
来源：http://hz.daxiang520.top/gtptnshffw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.yj20258888.top/gtujamakup.html

[Q04] 修改列类型
来源：http://hz.fengsongda.top/gtecxfkarq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.yangfankeji.com/gtefjsxmwa.html

[Q05] 重命名列
来源：http://hz.jinqigfzy.top/gtauzqsmot.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.gogol.net.cn/gtzbblfssz.html

[Q06] 删除列
来源：http://hz.havefunace.top/gtrslnhumz.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.jinqigfzy.top/gtwmqgbfpc.html

[Q07] 删除表
来源：http://hz.c1oappe.top/gtmmewelcs.html

DROP TABLE IF EXISTS orders;
来源：http://hz.tian-w.cn/gtsistpmko.html

[Q08] 创建普通索引
来源：http://hz.cheryme.top/gtxeuyibed.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.ydzc1.top/gthjqniwjl.html

[Q09] 创建唯一索引
来源：http://hz.shanyushiyangkeji.top/gtgeuxchcq.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.yj202588.top/gtvkghhlfm.html

[Q10] 插入单行
来源：http://hz.vqdsnc.cn/gtyiawyhbg.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.yongpay.top/gtruemgkgh.html

[Q11] 一次插入多行
来源：http://hz.c1oappe.top/gtfndldygl.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.nwbrower.top/gtucjwienq.html

[Q12] 插入后取自增 ID
来源：http://hz.yj20258888.top/gtocmehgwe.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yvedp.cn/gtufjujfyj.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.tanke756.top/gtrfozyfgw.html

[Q13] 忽略重复插入
来源：http://hz.xinyue.icu/gtktmpchlr.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.cdnleiting.top/gtcfzqtged.html

[Q14] 存在则更新（upsert）
来源：http://hz.shuidangran.top/gtjpqxylgx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.hongshengwenyu.top/gtkpahrezx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.shzxlz.cn/gtkggeetqa.html

[Q15] 查询全部
来源：http://hz.hfpthk.cn/gtgatmssxp.html

SELECT * FROM users;
来源：http://hz.jinqigfzy.top/gtxozxtygf.html

[Q16] 查询指定列
来源：http://hz.tanke756.top/gtgadgohim.html

SELECT id, name FROM users;
来源：http://hz.zhongyouzk.top/gtopsayjit.html

[Q17] 条件查询
来源：http://hz.guannengcc.top/gtxgiuoksg.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.316326.xyz/gtpxqwgcxp.html

[Q18] 模糊匹配
来源：http://hz.sufxvd.cn/gtdiitvziu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yongpay.top/gtdrknbxlh.html

[Q19] 范围查询
来源：http://hz.jiagoushi.top/gtuwzrvthu.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.zhiwuduotai.top/gtdbntuuru.html

[Q20] IN 列表
来源：http://hz.haohaochexian.top/gtvjrrejgn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.wangdashe.top/gtnygykpxw.html

[Q21] 空值判断
来源：http://hz.snrcjt.cn/gtjsbbejvy.html


<!-- 参考信息 -->