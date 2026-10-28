代发 wailian999

TS:   process.platform;  process.version
来源：http://hz.hongshengwenyu.top/gtnlasljve.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.cdnleiting.top/gtveypcdsi.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yuxming.cn/gtzwabospj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.hnxiangtu.top/gtkdxfinme.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.iojbl.cn/gtgvejpsfy.html

================================================================================
来源：http://hz.ivvv.top/gtcuqcrifl.html

N. 数据结构与算法
来源：http://hz.sweek.top/gtyanmtjuq.html

================================================================================
来源：http://hz.jinqigufen.top/gtninxmtdz.html

[N01] 二分查找（有序数组）
来源：http://hz.fengsongda.top/gtsdtwkcrl.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.wangshuangyany.cn/gtunzjxpsr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.ywan-chungtsiang.top/gtbenxcypu.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.aizwys.cn/gtumtzcigt.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jqgfzy.top/gtlaifjywd.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.nwbrower.top/gtkidgnhla.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.birdmap.top/gtbzpglwww.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.wangshuangyany.cn/gtguugtonb.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.hnxiangtu.top/gtnqdjcned.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.fzhhl.top/gtjsbyvwux.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.redwolf501.top/gtshnyteve.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.shuidangran.top/gtqcjqquas.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.chenlongwang.top/gtzekkjvep.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yuanzhike.top/gtjqzsekqv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.jinyuanbaomall.cn/gtpgjqargp.html

Go:   slices.Sort(arr)
来源：http://hz.sweek.top/gtavjuojkr.html

Ruby: arr.sort
来源：http://hz.52xcode.cn/gtoxcxvfpm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.hnqzz.top/gtfbpcdbby.html

[N03] 快速排序（分治示例）
来源：http://hz.pycfn.com/gttqeuxogx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.gotoacloud.top/gtetpbsvwo.html

PHP:  // 递归实现，或用 usort
来源：http://hz.wangshuangyany.cn/gtatpmtenz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yj20258.top/gtjllhrkvj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.redwolf501.top/gtqbonjzxz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yvedp.cn/gtvnxgmabn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.fengsongda.top/gthqpdqett.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.cqqwz.cn/gtjrbsffos.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.dianchejie.cn/gtwxipjier.html

[N04] 斐波那契数列
来源：http://hz.jiagoushi.top/gtzbapfuoh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.feifeiyinyue.top/gtijshqfkg.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.yvedp.cn/gthobktign.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yanxiufei.cn/gtxekefusu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ybcxt.top/gtytxrsazx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.shanyushiyangtech.top/gtnxowttft.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.feifeiyinyue.top/gttaqvjwfw.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.nanxuanxn.top/gtvoqtflvl.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.c1oappe.top/gtznypannc.html

[N05] 最大公约数
来源：http://hz.jqgufenzy.top/gtoigtkmcr.html

Py:   math.gcd(a, b)
来源：http://hz.yvedp.cn/gtcqygzuoi.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yvedp.cn/gtrhinioiv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.shzxlz.cn/gtcavjkxxx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.kuanghao11.cn/gtzltyzwzw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.wangdashe.top/gtezmqsiqj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.jinqigfzy.top/gtyioaoobr.html

Ruby: a.gcd(b)
来源：http://hz.dianchejie.cn/gtqqteovxx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.quarkkingdee.top/gttjizueiu.html

[N06] 判断回文字符串
来源：http://hz.ehwqpu.com/gtzgrivmce.html

Py:   s == s[::-1]
来源：http://hz.hammf.cn/gtlwtioate.html

PHP:  $s === strrev($s);
来源：http://hz.xylfe.cn/gtdjyorflf.html

JS:   s === [...s].reverse().join("")
来源：http://hz.cheryme.top/gtsucxmfax.html

TS:   s === [...s].reverse().join("")
来源：http://hz.smart0.xyz/gtcjttcvtd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.hfpthk.cn/gtcaijulef.html

Go:   // 双指针从两端比较
来源：http://hz.cheryme.top/gtnmypwote.html

Ruby: s == s.reverse
来源：http://hz.52xcode.cn/gtpkijrjok.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.tianlin.xyz/gtddfjgddl.html

[N07] 两数之和（返回下标）
来源：http://hz.xingfuxueyuan.xyz/gtjenwuaax.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.yvedp.cn/gtsbwetxbg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.gaohongyu789.top/gthzmkmxxs.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.cashguo.top/gtovpvvmyx.html

TS:   // 手写 Map<string, number>
来源：http://hz.ydzc1.top/gtqvjpbcgi.html

Java: // 手写 HashMap
来源：http://hz.svipenyu.cn/gtqtigcxvs.html

Go:   // 手写 map[int]int
来源：http://hz.ivvv.top/gtoexqaelf.html

Ruby: // 手写 Hash
来源：http://hz.zhoulong.xyz/gtvstiuuea.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.snrcjt.cn/gtbwggxatu.html

[N08] 生成全排列
来源：http://hz.yj20258.top/gtdkqnigmk.html

Py:   itertools.permutations(arr)
来源：http://hz.vqdsnc.cn/gtrgegxyhy.html

PHP:  // 手写递归交换
来源：http://hz.hongshengwenyu.top/gtobxxkbda.html

JS:   // 手写回溯递归
来源：http://hz.gogol.net.cn/gtlfadhzpv.html

TS:   // 手写回溯递归
来源：http://hz.jlsjyb.cn/gtkkllrnco.html

Java: // 手写回溯递归
来源：http://hz.vqdsnc.cn/gtxzcwmcit.html

Go:   // 手写回溯递归
来源：http://hz.nanxinkj.top/gtvckxamow.html

Ruby: arr.permutation.to_a
来源：http://hz.gotoacloud.top/gttwuvyoec.html

C#:   // 手写回溯递归
来源：http://hz.zhixingplan.top/gtpzbuqcii.html

[N09] 栈与队列
来源：http://hz.xinyue.icu/gtzknnvmjf.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.zhijiandao.cn/gtllykypxb.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.fengsongda.top/gtfiviytdu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.xuetiantiany.cn/gtdnwolsch.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jianghu66.top/gtyklkqqll.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.zhongyouzk.top/gtwamcpsfz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.tian-w.cn/gtznzrlkoi.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.nanxuanxn.top/gtmgcblzwf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.hfpthk.cn/gtntnaecuu.html

[N10] 链表节点定义
来源：http://hz.sysykeji.top/gtvnmnkmlj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.wangdashe.top/gtztchyxkj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.tanke756.top/gtkzbjzytr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zhijiandao.cn/gtocmkyvga.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.zhixingplan.top/gtmahvmpbq.html

Java: class Node { int v; Node next; }
来源：http://hz.xylfe.cn/gtvdzdufka.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.svipenyu.cn/gtodwxwpzr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.chenlongwang.top/gtyffajpnp.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.meibo888.top/gtiakzmivz.html

[N11] 二叉树中序遍历
来源：http://hz.svipenyu.cn/gtqlxvvjdz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.ywan-chungtsiang.top/gtpugbyyww.html

PHP:  // 手写递归函数
来源：http://hz.vqdsnc.cn/gtlesnwzpu.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jinqigfzy.top/gtdbarihrk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jiagoushi.top/gtysvmdxuf.html

Java: // 手写递归
来源：http://hz.zycfv.cn/gtcrasddrq.html

Go:   // 手写递归
来源：http://hz.pycfn.com/gtciwnoydc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.zdqjudy.top/gtgmduttlh.html

C#:   // 手写递归
来源：http://hz.jianghu66.top/gtvepnwozq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.jqgfzy.top/gtolqxmijs.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.tianlin.xyz/gterliwslg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.cdnleiting.top/gtqkzdihii.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cqqwz.cn/gtvcldcqvr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yj20258888.top/gtjwbdbzlb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yangfankeji.com/gtccfubzqw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.316326.xyz/gtrjrkruuz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.hysaishi.cn/gtmgabdelq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.andypj.xyz/gtaaccmors.html

================================================================================
来源：http://hz.andypj.xyz/gttibhhpqf.html

O. 并发与异步
来源：http://hz.guowangkeji.top/gtgfrtuybr.html

================================================================================
来源：http://hz.nanxinkj.top/gtrzmenrtt.html

[O01] 启动一个线程
来源：http://hz.vqdsnc.cn/gtbxpyuffl.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.feifeiyinyue.top/gtvlspfasv.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.aibaodan.cn/gtqrziiroh.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.cucudq.cn/gtewsxfipb.html

TS:   // 同 JS
来源：http://hz.havefunace.top/gtskxibsma.html

Java: new Thread(() -> f()).start()
来源：http://hz.gotoacloud.top/gtrjiesckc.html

Go:   go f()
来源：http://hz.redwolf501.top/gtseutlqqk.html

Ruby: Thread.new { f }
来源：http://hz.bjfxy.top/gtifkgohta.html

C#:   Task.Run(() => F());
来源：http://hz.chenlongwang.top/gtmrwcezen.html

[O02] 使用线程池
来源：http://hz.ivvv.top/gtxeinjbrh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.wangshuangyany.cn/gtwxoisfnk.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.gzhubu.top/gtdqoiuoyd.html

JS:   // worker_threads 线程池
来源：http://hz.hnqzz.top/gtavjxdqhb.html

TS:   // worker_threads 线程池
来源：http://hz.redwolf501.top/gtgwtpibfn.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yvedp.cn/gticakycai.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.havefunace.top/gtyaznaclc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.gogol.net.cn/gtpzbkumju.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.hammf.cn/gtbovqhcdi.html

[O03] 加锁保护共享数据
来源：http://hz.xingfuxueyuan.xyz/gtlmppfyel.html

Py:   with lock: shared += 1
来源：http://hz.zhoulong.xyz/gtypvasovh.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.cashguo.top/gtmyhtsacg.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.zhongyouzk.top/gtahkqzyrd.html

TS:   // 同 JS
来源：http://hz.xziqi.cn/gtbysqchhw.html

Java: synchronized (this) { shared++; }
来源：http://hz.tanke756.top/gtuooyvxpm.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.kuanghao11.cn/gtvkwlytyc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.0kj1m.cn/gtyigpdxrq.html

C#:   lock (gate) { shared++; }
来源：http://hz.redwolf501.top/gtkwwngjcv.html

[O04] 定义异步函数并等待
来源：http://hz.mhx1999.top/gtrtfamlbx.html

Py:   async def f():⏎    await g()
来源：http://hz.fengsongda.top/gtugxvkjlo.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.snrcjt.cn/gtitnpullp.html

JS:   async function f() { await g(); }
来源：http://hz.yj202588.top/gtkzumfbkk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.aizwys.cn/gtzvqqwyrk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.daria6918.cn/gtudsibukq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.ydjk.org.cn/gtiwkpfhor.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.jqgufenzy.top/gtgdjvltqh.html

C#:   async Task F() { await G(); }
来源：http://hz.jinghuilouyu.cn/gtwjnuyiss.html

[O05] 并发执行并等待全部完成
来源：http://hz.sysykeji.top/gtlrnbwspz.html

Py:   asyncio.gather(*tasks)
来源：http://hz.shzxlz.cn/gtllmrbter.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.gaohongyu789.top/gtxyvdjkel.html

JS:   await Promise.all(tasks)
来源：http://hz.dashuyun.cn/gtxenealnp.html

TS:   await Promise.all(tasks)
来源：http://hz.52xcode.cn/gtptarvnks.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.xuanzx.com/gtplsnbbzw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.nanxinkj.top/gtbfegsiju.html

Ruby: threads.map(&:join)
来源：http://hz.jyoumei.cn/gtzcmdpehf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.ydjk.org.cn/gtojzjibod.html

[O06] 使用进程池
来源：http://hz.ydzc1.top/gtfttfohgz.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.snrcjt.cn/gtqrnnwruj.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.fzhhl.top/gtyvszyjee.html

JS:   // child_process / cluster 模块
来源：http://hz.jiagoushi.top/gthxrromrm.html

TS:   // child_process / cluster 模块
来源：http://hz.ehwqpu.com/gtmtnlhxei.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.guowangkeji.top/gtwidtzhez.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.fengsongda.top/gtugfprvem.html

Ruby: // fork 块
来源：http://hz.sxryk.cn/gtvlkyrxoa.html

C#:   Parallel.For
来源：http://hz.bjfxy.top/gtbgxguipd.html

================================================================================
来源：http://hz.52xcode.cn/gtldetobgb.html

P. 常用工具函数
来源：http://hz.guannengcc.top/gtltiwawqy.html

================================================================================
来源：http://hz.c1oappe.top/gtkcmesahq.html

[P01] 生成 UUID
来源：http://hz.tian-w.cn/gttfanazln.html

Py:   str(uuid.uuid4())
来源：http://hz.nanxinkj.top/gtaztmfdep.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.gotoacloud.top/gttbqqkxic.html

JS:   crypto.randomUUID()
来源：http://hz.yj20258.top/gtmdrwyxix.html

TS:   crypto.randomUUID()
来源：http://hz.shangyingyoupin.top/gtuaqdljkd.html

Java: UUID.randomUUID().toString()
来源：http://hz.gotoacloud.top/gtpgspfouc.html

Go:   // 用 github.com/google/uuid
来源：http://hz.cheryme.top/gtspyqqzsa.html

Ruby: SecureRandom.uuid
来源：http://hz.chenzaomai.com/gtlbarfphr.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.9152youxi.cn/gtupwatvet.html

[P02] MD5 / SHA256 摘要
来源：http://hz.zhixingplan.top/gtwmcbldgx.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.fengsongda.top/gtyrkhcude.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.chenjidiqi.icu/gtifndufzd.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.shangyingyoupin.top/gtsdithbcm.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.zhoulong.xyz/gtpnsfajrg.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.gaohongyu789.top/gtvtovchuh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.xylfe.cn/gtlhhmtuel.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.hywenlv.cn/gtqmuowvxj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.daria6918.cn/gttyrbtmdt.html

[P03] 生成短随机字符串
来源：http://hz.birdmap.top/gtuzaqoaaa.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.pycfn.com/gtcevjcjmg.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.jinqigfzy.top/gtslpxvvdk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhoulong.xyz/gtjqoljhsz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jqgfzy.top/gtcrzcsefl.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.nanxuanxn.top/gtfqvxzfrk.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.chenzaomai.com/gtqomhzigt.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.fengsongda.top/gtxehdzmzi.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.tanke756.top/gtezicidtz.html

[P04] 求长度
来源：http://hz.pycfn.com/gtaolipucw.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.yvedp.cn/gtpqbpctxl.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.haohaochexian.top/gtpbketxnf.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.snrcjt.cn/gtcnsmyuis.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.shanyushiyangkeji.top/gtjlwgudgl.html

Java: list.size();  map.size();  s.length()
来源：http://hz.sweek.top/gtdstayszs.html

Go:   len(arr);  len(m)
来源：http://hz.aizwys.cn/gtbcrpzqke.html

Ruby: x.length;  x.size
来源：http://hz.yanxiufei.cn/gtpyqrwytf.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.gaohongyu789.top/gtzqazuaho.html

[P05] 判断两个对象内容是否相等
来源：http://hz.ybcxt.top/gtdhegxmrc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.jyoumei.cn/gteuokpcph.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.zhiwuduotai.top/gtpuzfcdgz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.iojbl.cn/gtjhbxdhnp.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yuanzhike.top/gtrqcwgync.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.xuanzx.com/gtpgaetfgi.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.haohaochexian.top/gtygxpvshh.html

Ruby: a == b
来源：http://hz.zhiwuduotai.top/gtkxpsvaix.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.bjfxy.top/gtnhesulob.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.yuxming.cn/gtrnkodpqr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.smart0.xyz/gtmpdnnogz.html

PHP:  if (empty($x)) {}
来源：http://hz.dianchejie.cn/gtldqbjyse.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.shuidangran.top/gtxptsxhmf.html

TS:   if (x == null) {}
来源：http://hz.smart0.xyz/gttzgesvgz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.tanke756.top/gtweyzvhzw.html

Go:   if x == nil {}
来源：http://hz.cucudq.cn/gtbicyejph.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.yuxming.cn/gtpklovost.html

C#:   if (x is null) {}
来源：http://hz.ppjwa.cn/gtdscthsjv.html

[P07] 防抖与节流
来源：http://hz.birdmap.top/gtkqqzcoca.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.gogol.net.cn/gtrbtsahhr.html

PHP:  // 手写时间戳比较
来源：http://hz.9152youxi.cn/gtxzrbecfq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jinyuanbaomall.cn/gtkhrdgoav.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.chenzaomai.com/gtgdhdgcms.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.cucudq.cn/gtplsujfnv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.tanke756.top/gtyegivews.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.sxryk.cn/gtuvntqvcg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.wangshuangyany.cn/gtansvjhit.html

[P08] 处理浮点精度问题
来源：http://hz.gotoacloud.top/gtaubtelrh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.fzhhl.top/gtbynizjdt.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.jyoumei.cn/gtvjrcrhci.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.wangshuangyany.cn/gtmhsmmgqd.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.yj20258.top/gtcohzjvsb.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yongpay.top/gtvfbgowen.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.shuidangran.top/gtnetmvshk.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.jinyuanbaomall.cn/gtzeujaebd.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.chenjidiqi.icu/gtiuwfxvay.html

================================================================================
来源：http://hz.pycfn.com/gtibcdixjk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yanxiufei.cn/gtjzsycxlk.html

================================================================================
来源：http://hz.xylfe.cn/gtjvbdqyph.html

[Q01] 创建表
来源：http://hz.snrcjt.cn/gtufldqlkq.html

CREATE TABLE users (
来源：http://hz.jlsjyb.cn/gtuerfrewa.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.daria6918.cn/gtvlesrgyy.html

name VARCHAR(50) NOT NULL,
来源：http://hz.jinyuanbaomall.cn/gtpzwbaykp.html

email VARCHAR(100) UNIQUE,
来源：http://hz.zhengqikj.top/gttjtovhhq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.zycfv.cn/gtvsffckym.html

);
来源：http://hz.guowangkeji.top/gttwhnptve.html

[Q02] 创建带外键的表
来源：http://hz.zhongyouzk.top/gtuvoeaaxu.html

CREATE TABLE orders (
来源：http://hz.yanxiufei.cn/gtuumkwnlx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.quarkkingdee.top/gtrwdfgmax.html

user_id INT NOT NULL,
来源：http://hz.cheryme.top/gtyagbevqq.html

amount DECIMAL(10, 2),
来源：http://hz.zhengqikj.top/gtilddsvmx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.redwolf501.top/gtnokxoipr.html

);
来源：http://hz.jyoumei.cn/gtvpvschzi.html

[Q03] 增加列
来源：http://hz.0kj1m.cn/gtyvasedrx.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.jiagoushi.top/gtmfmatnol.html

[Q04] 修改列类型
来源：http://hz.yonumen.top/gthtphqifh.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.ybcxt.top/gtrhobdcft.html

[Q05] 重命名列
来源：http://hz.yj20258.top/gtjuvhtgpl.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.nanxuanxn.top/gtvqtyrsfl.html

[Q06] 删除列
来源：http://hz.sysykeji.top/gtoupissay.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.aibaodan.cn/gttjcfaoiz.html

[Q07] 删除表
来源：http://hz.yj20258888.top/gtsptvwgcz.html

DROP TABLE IF EXISTS orders;
来源：http://hz.tian-w.cn/gtzedlsjpf.html

[Q08] 创建普通索引
来源：http://hz.tianlin.xyz/gtcuqsawxa.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.snrcjt.cn/gtmxsmzbvt.html

[Q09] 创建唯一索引
来源：http://hz.bjfxy.top/gtetjbdvjd.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.kuanghao11.cn/gtkkksphja.html

[Q10] 插入单行
来源：http://hz.jinqigfzy.top/gttmwgzscs.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.ydzc1.top/gtlohmtgwx.html

[Q11] 一次插入多行
来源：http://hz.ivvv.top/gtifmjwqtw.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yuxming.cn/gtmaicxoqk.html

[Q12] 插入后取自增 ID
来源：http://hz.hywenlv.cn/gtqpitskjw.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yonumen.top/gtbxsgareb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.hnqzz.top/gtzzbwjgbk.html

[Q13] 忽略重复插入
来源：http://hz.quarkkingdee.top/gtwozaajsu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.pycfn.com/gtufoobgzz.html

[Q14] 存在则更新（upsert）
来源：http://hz.xinyue.icu/gtagrgnwem.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.c1oappe.top/gtojyafqpj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.zhongyouzk.top/gtduxonhmb.html

[Q15] 查询全部
来源：http://hz.havefunace.top/gtdobohdlk.html

SELECT * FROM users;
来源：http://hz.cqqwz.cn/gtbgnnimoj.html

[Q16] 查询指定列
来源：http://hz.yueranfly.top/gttbynxzpv.html

SELECT id, name FROM users;
来源：http://hz.aizwys.cn/gtcsgqfkot.html

[Q17] 条件查询
来源：http://hz.meibo888.top/gtaldwyyod.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.c1oappe.top/gtkekbduuv.html

[Q18] 模糊匹配
来源：http://hz.cashguo.top/gtahrsirfv.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yj20258888.top/gtwmzratsi.html

[Q19] 范围查询
来源：http://hz.zycfv.cn/gtqvgkdpnf.html


<!-- 参考信息 -->