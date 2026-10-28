代发 wailian999

TS:   process.platform;  process.version
来源：http://hz.cheryme.top/gtxcrvwwxk.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.feifeiyinyue.top/gtzvtvyopx.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.hammf.cn/gtbjmifjgd.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.sweek.top/gtawgxjpbd.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.wangshuangyany.cn/gtywdlxopv.html

================================================================================
来源：http://hz.316326.xyz/gttiuxwabs.html

N. 数据结构与算法
来源：http://hz.daxiang520.top/gtpocnlmiz.html

================================================================================
来源：http://hz.tian-w.cn/gtrdpbcmwa.html

[N01] 二分查找（有序数组）
来源：http://hz.tianlin.xyz/gtzrbhthfo.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.fengsongda.top/gtvazraqiq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.zhoulong.xyz/gtenkiravq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.mhx1999.top/gtpowlxtxw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.daxiang520.top/gtawfyfcda.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.zhoulong.xyz/gtciqqitvq.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jinqigufen.top/gttqdugnfo.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.shanyushiyangtech.top/gtrfgegzwa.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.cucudq.cn/gtkinyaubq.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.wangdashe.top/gtrskshvjm.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhoulong.xyz/gtmvcreqky.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.cashguo.top/gtxzbzlhkh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xziqi.cn/gtycfhikwq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jinghuilouyu.cn/gtxoqsqook.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.jqgfzy.top/gtegkyaazg.html

Go:   slices.Sort(arr)
来源：http://hz.xuanzx.com/gtkkvztyii.html

Ruby: arr.sort
来源：http://hz.jianghu66.top/gtieyiiqey.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.jyoumei.cn/gtwrkvhfwv.html

[N03] 快速排序（分治示例）
来源：http://hz.aibaodan.cn/gtrdnkvjtw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.ywan-chungtsiang.top/gtbqgzdyud.html

PHP:  // 递归实现，或用 usort
来源：http://hz.tanke756.top/gtqvaftwvl.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.bjfxy.top/gtdeqdpdxw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jinqigufen.top/gtyptntjua.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.zhaomingkeji.xyz/gtryhnuqvu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.nwbrower.top/gtzduvwsqe.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yongpay.top/gtfygwyemv.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.ppjwa.cn/gtrrvwhfut.html

[N04] 斐波那契数列
来源：http://hz.316326.xyz/gtvjghcvbb.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.xuanzx.com/gtlabzcyix.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.aizwys.cn/gttgkqpzle.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.daria6918.cn/gtzbpdxphm.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhongyouzk.top/gtbcrupgub.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yj202588.top/gtnwjgpsrp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.fengsongda.top/gtznraoahb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.zdqjudy.top/gtpptizwhl.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.xuanzx.com/gtqgzciyni.html

[N05] 最大公约数
来源：http://hz.gaohongyu789.top/gthzxawevz.html

Py:   math.gcd(a, b)
来源：http://hz.hywenlv.cn/gtmlnqkclw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.sweek.top/gtbhapiabv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yongpay.top/gtqklvptoc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yvedp.cn/gtrirhoqid.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.ppjwa.cn/gtmnpdacmv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.hysaishi.cn/gttmoafayn.html

Ruby: a.gcd(b)
来源：http://hz.zhongyouzk.top/gtgjqjecfp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.svipenyu.cn/gtfnecuncg.html

[N06] 判断回文字符串
来源：http://hz.fengsongda.top/gtwucrxuad.html

Py:   s == s[::-1]
来源：http://hz.sweek.top/gtzucfzfoi.html

PHP:  $s === strrev($s);
来源：http://hz.mhx1999.top/gtauvrvzte.html

JS:   s === [...s].reverse().join("")
来源：http://hz.xinyue.icu/gtghjnlfrh.html

TS:   s === [...s].reverse().join("")
来源：http://hz.birdmap.top/gtstltooic.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.gaohongyu789.top/gtirvfrgch.html

Go:   // 双指针从两端比较
来源：http://hz.xziqi.cn/gttmbeakdl.html

Ruby: s == s.reverse
来源：http://hz.jinghuilouyu.cn/gtuvpoxgeu.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.cucudq.cn/gtbekxmdyh.html

[N07] 两数之和（返回下标）
来源：http://hz.zdqjudy.top/gtnhxbmifk.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.yvedp.cn/gtjinofidg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.gotoacloud.top/gtenuinylx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.jianghu66.top/gthyswyftz.html

TS:   // 手写 Map<string, number>
来源：http://hz.jinghuilouyu.cn/gtijzspsmu.html

Java: // 手写 HashMap
来源：http://hz.shuidangran.top/gtthsyimyv.html

Go:   // 手写 map[int]int
来源：http://hz.redwolf501.top/gtqsryvsou.html

Ruby: // 手写 Hash
来源：http://hz.fzhhl.top/gtzfxtoajw.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.xingfuxueyuan.xyz/gtburgeysn.html

[N08] 生成全排列
来源：http://hz.vqdsnc.cn/gtgmdgymyl.html

Py:   itertools.permutations(arr)
来源：http://hz.shangyingyoupin.top/gtxboztjbr.html

PHP:  // 手写递归交换
来源：http://hz.jyoumei.cn/gtpadkyyiw.html

JS:   // 手写回溯递归
来源：http://hz.tian-w.cn/gtfaaykuwu.html

TS:   // 手写回溯递归
来源：http://hz.svipenyu.cn/gtfkpuesrm.html

Java: // 手写回溯递归
来源：http://hz.hammf.cn/gtapfhrspn.html

Go:   // 手写回溯递归
来源：http://hz.jlsjyb.cn/gtymhxzwmr.html

Ruby: arr.permutation.to_a
来源：http://hz.birdmap.top/gtqjztmdsg.html

C#:   // 手写回溯递归
来源：http://hz.redwolf501.top/gtzupmvdvm.html

[N09] 栈与队列
来源：http://hz.shanyushiyangkeji.top/gthukpkevv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.tian-w.cn/gtsoysusgp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.gogol.net.cn/gtndjaokmm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.wangshuangyany.cn/gtduylhpre.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.wangshuangyany.cn/gtswsxsrne.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.gogol.net.cn/gtwerkrhye.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.havefunace.top/gtncqzygpm.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yangfankeji.com/gtrgxhlexo.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.316326.xyz/gtpzrpjgaf.html

[N10] 链表节点定义
来源：http://hz.zhoulong.xyz/gtwuspuasn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.jinyuanbaomall.cn/gtmlvxwoip.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.tanke756.top/gtsrghxeff.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.c1oappe.top/gtgrmnxaer.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.nanxinkj.top/gtrocqgrrb.html

Java: class Node { int v; Node next; }
来源：http://hz.yueranfly.top/gtqapqaukm.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.gzhubu.top/gtqlvmvmcc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.jinghuilouyu.cn/gtzuswtose.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.xziqi.cn/gtvaiwisqs.html

[N11] 二叉树中序遍历
来源：http://hz.jiagoushi.top/gtpbnizfsu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.hongshengwenyu.top/gtbufafrtd.html

PHP:  // 手写递归函数
来源：http://hz.sweek.top/gtfrjhqram.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jinghuilouyu.cn/gtdhjbetgb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.tianlin.xyz/gtpyhuxnxq.html

Java: // 手写递归
来源：http://hz.haohaochexian.top/gtwbmcfuli.html

Go:   // 手写递归
来源：http://hz.shanyushiyangkeji.top/gtrlsnepgz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.cucudq.cn/gtwdljqedu.html

C#:   // 手写递归
来源：http://hz.sweek.top/gtvovtcluo.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.vqdsnc.cn/gttvxkfzbm.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.snrcjt.cn/gtfmkbhhan.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.zhiwuduotai.top/gtvuoetiob.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yj20258888.top/gtfxbssidf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xuetiantiany.cn/gtxjxmwwfb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jqgfzy.top/gtwwitxdae.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.wangshuangyany.cn/gtmqnvgrir.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.xylfe.cn/gtllojdvec.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.snrcjt.cn/gtmltcqncf.html

================================================================================
来源：http://hz.daria6918.cn/gtkuiufujf.html

O. 并发与异步
来源：http://hz.xylfe.cn/gtichlmslp.html

================================================================================
来源：http://hz.yonumen.top/gtuzrmrres.html

[O01] 启动一个线程
来源：http://hz.zhijiandao.cn/gtxaueepnj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.zhijiandao.cn/gtdtmrvzkq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.meibo888.top/gtnxcoatjh.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.yj20258888.top/gtpttustag.html

TS:   // 同 JS
来源：http://hz.ydzc1.top/gtesttqdff.html

Java: new Thread(() -> f()).start()
来源：http://hz.hnxiangtu.top/gtgfqorepb.html

Go:   go f()
来源：http://hz.gzhubu.top/gtfrqsnnmk.html

Ruby: Thread.new { f }
来源：http://hz.jlsjyb.cn/gtjlfqwxxo.html

C#:   Task.Run(() => F());
来源：http://hz.yj20258888.top/gtkrfblrdl.html

[O02] 使用线程池
来源：http://hz.mhx1999.top/gtraiftzyy.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yongpay.top/gtgusbmshb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.jyoumei.cn/gtgdakssvk.html

JS:   // worker_threads 线程池
来源：http://hz.ppjwa.cn/gtqjpiwqyk.html

TS:   // worker_threads 线程池
来源：http://hz.yongpay.top/gtljofcpcw.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.tian-w.cn/gtxvcvgoyb.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.birdmap.top/gtvvxznptx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.gogol.net.cn/gtfdhqbxng.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.ivvv.top/gtbllavumc.html

[O03] 加锁保护共享数据
来源：http://hz.shanyushiyangkeji.top/gthcfzefdh.html

Py:   with lock: shared += 1
来源：http://hz.sufxvd.cn/gtulzvnskm.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.jlsjyb.cn/gtszmketxx.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.guannengcc.top/gtwjrmfwym.html

TS:   // 同 JS
来源：http://hz.jinqigfzy.top/gtwmoevowb.html

Java: synchronized (this) { shared++; }
来源：http://hz.yj20258.top/gtcpfrebch.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.pycfn.com/gtyehqsylk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.smart0.xyz/gtnrobvopa.html

C#:   lock (gate) { shared++; }
来源：http://hz.shuidangran.top/gtsbjpzwhh.html

[O04] 定义异步函数并等待
来源：http://hz.yuanzhike.top/gtrykzfuyg.html

Py:   async def f():⏎    await g()
来源：http://hz.zhijiandao.cn/gtywhopqai.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.snrcjt.cn/gtbyifnrne.html

JS:   async function f() { await g(); }
来源：http://hz.hysaishi.cn/gtrpaveskq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.jlsjyb.cn/gtpboppsim.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.ivvv.top/gtybdwvgqb.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.jqgfzy.top/gtizdpqxub.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.zhixingplan.top/gtpyhydnjb.html

C#:   async Task F() { await G(); }
来源：http://hz.nwbrower.top/gtvhzbzmcp.html

[O05] 并发执行并等待全部完成
来源：http://hz.sweek.top/gtfzlcnexu.html

Py:   asyncio.gather(*tasks)
来源：http://hz.hnqzz.top/gtcufvszra.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.bjfxy.top/gtfsotmobh.html

JS:   await Promise.all(tasks)
来源：http://hz.yj20258.top/gtzbeylsgo.html

TS:   await Promise.all(tasks)
来源：http://hz.feifeiyinyue.top/gtigjtengj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.nanxuanxn.top/gtdeekkgqr.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.hysaishi.cn/gtdilkxjha.html

Ruby: threads.map(&:join)
来源：http://hz.sysykeji.top/gtsrvxwmai.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.zycfv.cn/gtxqngantv.html

[O06] 使用进程池
来源：http://hz.havefunace.top/gtgiqucgah.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.chenlongwang.top/gtfijjkncg.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.sufxvd.cn/gtxkysefzz.html

JS:   // child_process / cluster 模块
来源：http://hz.chenzaomai.com/gtgdztpjee.html

TS:   // child_process / cluster 模块
来源：http://hz.kuanghao11.cn/gtavbfpotc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.9152youxi.cn/gtxbmjodis.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.chenzaomai.com/gtenmxgnzn.html

Ruby: // fork 块
来源：http://hz.dashuyun.cn/gtzryuqbvn.html

C#:   Parallel.For
来源：http://hz.xuanzx.com/gtcnfjcduo.html

================================================================================
来源：http://hz.ehwqpu.com/gtfbouxhdd.html

P. 常用工具函数
来源：http://hz.0kj1m.cn/gtkjrujlyk.html

================================================================================
来源：http://hz.snrcjt.cn/gtaaaornyn.html

[P01] 生成 UUID
来源：http://hz.wangshuangyany.cn/gtnpprhzes.html

Py:   str(uuid.uuid4())
来源：http://hz.cdnleiting.top/gtrueprpam.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.ydzc1.top/gtitefgmnw.html

JS:   crypto.randomUUID()
来源：http://hz.snrcjt.cn/gtwlbhfhxd.html

TS:   crypto.randomUUID()
来源：http://hz.cheryme.top/gtcehrkcol.html

Java: UUID.randomUUID().toString()
来源：http://hz.daxiang520.top/gttuvugezi.html

Go:   // 用 github.com/google/uuid
来源：http://hz.9152youxi.cn/gtwwexecpq.html

Ruby: SecureRandom.uuid
来源：http://hz.nanxuanxn.top/gtoenpikqb.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.hfpthk.cn/gtagdgjsug.html

[P02] MD5 / SHA256 摘要
来源：http://hz.fzhhl.top/gttdotbmtf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.haohaochexian.top/gtlgtudlul.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.wangdashe.top/gtybqpbpit.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.nanxinkj.top/gtkrrcutsx.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.hongshengwenyu.top/gtljabsbdw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.ehwqpu.com/gtgrweqrwc.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.xuetiantiany.cn/gtfcbckvms.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.zycfv.cn/gtmonjsryl.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yuanzhike.top/gtivwuzzwy.html

[P03] 生成短随机字符串
来源：http://hz.jyoumei.cn/gtztwznmwo.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.cqqwz.cn/gtjipconvk.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.kuanghao11.cn/gtapybibtv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.shangyingyoupin.top/gttxwvhoch.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.pycfn.com/gtbnqwnhoy.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.zhixingplan.top/gtkpkxkswr.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.jinghuilouyu.cn/gtccpwtlsu.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.chenjidiqi.icu/gtdgioiuac.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.gzhubu.top/gtrgmrbszv.html

[P04] 求长度
来源：http://hz.havefunace.top/gttayzvqav.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.ywan-chungtsiang.top/gtvrgjzdte.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xuanzx.com/gttugrqiqx.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.cucudq.cn/gtxjtznpbh.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xinyue.icu/gtfqnlusgz.html

Java: list.size();  map.size();  s.length()
来源：http://hz.xylfe.cn/gtopxjaydc.html

Go:   len(arr);  len(m)
来源：http://hz.sxryk.cn/gtyirvcrcw.html

Ruby: x.length;  x.size
来源：http://hz.chenjidiqi.icu/gtmroxaxmc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.shanyushiyangkeji.top/gtixmrimwf.html

[P05] 判断两个对象内容是否相等
来源：http://hz.9152youxi.cn/gtgtaowwzi.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.hammf.cn/gtwfnuoizc.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.jinqigfzy.top/gtegifxbsc.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.birdmap.top/gtyjnienrd.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zhongyouzk.top/gtbshoywvv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.shanyushiyangkeji.top/gtlfqtwyle.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.316326.xyz/gtcpynkwor.html

Ruby: a == b
来源：http://hz.shuidangran.top/gtqfaynagb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.52xcode.cn/gtvtlwphiv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.snrcjt.cn/gtrcdluvqe.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.haohaochexian.top/gtjeebhima.html

PHP:  if (empty($x)) {}
来源：http://hz.zhijiandao.cn/gtifoiazfm.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jqgufenzy.top/gtoatdeuik.html

TS:   if (x == null) {}
来源：http://hz.sysykeji.top/gtdtyjjxwi.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.xingfuxueyuan.xyz/gtrwthsesa.html

Go:   if x == nil {}
来源：http://hz.wangshuangyany.cn/gttfojypgy.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.hongshengwenyu.top/gtkoyxhovc.html

C#:   if (x is null) {}
来源：http://hz.9152youxi.cn/gtycfpfoaj.html

[P07] 防抖与节流
来源：http://hz.ywan-chungtsiang.top/gthoihgqbh.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.ppjwa.cn/gtpbwqlpbo.html

PHP:  // 手写时间戳比较
来源：http://hz.jinqigufen.top/gtbipqbvbr.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zdqjudy.top/gtfrxxoadf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.c1oappe.top/gtpkjbbzwc.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.andypj.xyz/gtahimeghf.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.jiagoushi.top/gtjmeznybh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.hnqzz.top/gtscrkbmmm.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.jianghu66.top/gtjqinekcx.html

[P08] 处理浮点精度问题
来源：http://hz.xinyue.icu/gtezwozbix.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jinyuanbaomall.cn/gtiqvlplfe.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.jianghu66.top/gtdkzheoym.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.jinqigfzy.top/gtvrdzcfbd.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.yj20258888.top/gtdngnvmnz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.gzhubu.top/gtpdwnlfgu.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.cqqwz.cn/gtxvretfke.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.xuanzx.com/gtewlldsux.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.shuidangran.top/gtjrxirdup.html

================================================================================
来源：http://hz.smart0.xyz/gtowaakril.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yuanzhike.top/gtqxjdhajh.html

================================================================================
来源：http://hz.zhengqikj.top/gtnhubdddb.html

[Q01] 创建表
来源：http://hz.ydzc1.top/gthxwwnnvz.html

CREATE TABLE users (
来源：http://hz.kuanghao11.cn/gtlysvmhjr.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.cashguo.top/gtpuymghmh.html

name VARCHAR(50) NOT NULL,
来源：http://hz.hnxiangtu.top/gtoymkblio.html

email VARCHAR(100) UNIQUE,
来源：http://hz.xinyue.icu/gtfrkjuxhg.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.9152youxi.cn/gtavijhasd.html

);
来源：http://hz.nanxuanxn.top/gtgbhnutqg.html

[Q02] 创建带外键的表
来源：http://hz.sxryk.cn/gtxosrcnpx.html

CREATE TABLE orders (
来源：http://hz.ybcxt.top/gtrbbadyft.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhoulong.xyz/gttfqzxide.html

user_id INT NOT NULL,
来源：http://hz.hnqzz.top/gtfldyyqdz.html

amount DECIMAL(10, 2),
来源：http://hz.sufxvd.cn/gtnajbedrh.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.yvedp.cn/gteycfhcqb.html

);
来源：http://hz.nanxuanxn.top/gtoqshqvmb.html

[Q03] 增加列
来源：http://hz.zhoulong.xyz/gtphudylcq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.vqdsnc.cn/gtwriwukel.html

[Q04] 修改列类型
来源：http://hz.zhengqikj.top/gtkmrouhts.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.redwolf501.top/gtrqewqtfv.html

[Q05] 重命名列
来源：http://hz.gzhubu.top/gtkvhjjtwz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.c1oappe.top/gtifqgamxf.html

[Q06] 删除列
来源：http://hz.guannengcc.top/gtosgzlazk.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.yj20258888.top/gtfulxwfyy.html

[Q07] 删除表
来源：http://hz.tian-w.cn/gtqbfekbwh.html

DROP TABLE IF EXISTS orders;
来源：http://hz.ehwqpu.com/gtmhlwrpmd.html

[Q08] 创建普通索引
来源：http://hz.hywenlv.cn/gtutbfgccm.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.ybcxt.top/gtjgnqfbof.html

[Q09] 创建唯一索引
来源：http://hz.chenjidiqi.icu/gtkygxdnxv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.yj20258.top/gtwwopklyf.html

[Q10] 插入单行
来源：http://hz.aibaodan.cn/gtgbnssgte.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.xingfuxueyuan.xyz/gtntdnjozq.html

[Q11] 一次插入多行
来源：http://hz.cucudq.cn/gthnrcfgyo.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yongpay.top/gtebaiuoef.html

[Q12] 插入后取自增 ID
来源：http://hz.zhiwuduotai.top/gtnzsjrnrz.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.sxryk.cn/gtsbnfgotx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.zhiwuduotai.top/gttaeqspqw.html

[Q13] 忽略重复插入
来源：http://hz.hnqzz.top/gtmepzpfkw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.ywan-chungtsiang.top/gtcztsboek.html

[Q14] 存在则更新（upsert）
来源：http://hz.cashguo.top/gtscrxekdb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.shanyushiyangtech.top/gtcqgnqlim.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.cucudq.cn/gtztzrshjb.html

[Q15] 查询全部
来源：http://hz.pengpengdd.cyou/gtutamjdqz.html

SELECT * FROM users;
来源：http://hz.kuanghao11.cn/gtlqlpmepp.html

[Q16] 查询指定列
来源：http://hz.tanke756.top/gtcyqupwpk.html

SELECT id, name FROM users;
来源：http://hz.jinqigfzy.top/gtcqtlhyii.html

[Q17] 条件查询
来源：http://hz.xinyue.icu/gtgpkpjide.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.nanxinkj.top/gtzvdpojsm.html

[Q18] 模糊匹配
来源：http://hz.zhijiandao.cn/gtbhhjihqu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.xinyue.icu/gtlxtekfjj.html

[Q19] 范围查询
来源：http://hz.hnxiangtu.top/gtkeepetiu.html


<!-- 参考信息 -->