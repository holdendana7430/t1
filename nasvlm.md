代发 wailian999

[M08] 获取系统与运行时信息
来源：http://hz.wangshuangyany.cn/gtwjgkxwlq.html

Py:   platform.system();  platform.python_version()
来源：http://hz.sysykeji.top/gtshesndly.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.316326.xyz/gtvjjwcxlc.html

JS:   process.platform;  process.version
来源：http://hz.daria6918.cn/gtoeolqodx.html

TS:   process.platform;  process.version
来源：http://hz.aizwys.cn/gteastpkhw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.zycfv.cn/gtheavakxg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.smart0.xyz/gtoiqrzurk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.snrcjt.cn/gtsdsavois.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.jinqigfzy.top/gtwogaegwy.html

================================================================================
来源：http://hz.jinqigufen.top/gtqayesywi.html

N. 数据结构与算法
来源：http://hz.xziqi.cn/gtppmyltol.html

================================================================================
来源：http://hz.gotoacloud.top/gtxrxbjkya.html

[N01] 二分查找（有序数组）
来源：http://hz.0kj1m.cn/gtauyykamt.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.316326.xyz/gtzsdlqmgk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.feifeiyinyue.top/gtahtlsxfo.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.gogol.net.cn/gtevwjsamp.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.bjfxy.top/gtznfxiaez.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.jqgfzy.top/gtprkuujzd.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.meibo888.top/gtmzffvksi.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.hnqzz.top/gtnbhhtrvd.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.xuetiantiany.cn/gtxmahlmbe.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.zhiwuduotai.top/gtbywfcklo.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.tianlin.xyz/gtavtpaijx.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.ppjwa.cn/gtxsfyohqz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhoulong.xyz/gtiwzrqnvs.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.havefunace.top/gtbpfhsgcv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.iojbl.cn/gtseubncke.html

Go:   slices.Sort(arr)
来源：http://hz.jinghuilouyu.cn/gtlqmqalxe.html

Ruby: arr.sort
来源：http://hz.fengsongda.top/gtbiybyqmo.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.zhengqikj.top/gtpzzbsruh.html

[N03] 快速排序（分治示例）
来源：http://hz.ppjwa.cn/gttmlweitf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.bjfxy.top/gtmqgyzwsx.html

PHP:  // 递归实现，或用 usort
来源：http://hz.ppjwa.cn/gtnlpqhexf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.tian-w.cn/gtapvdrdvd.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.gaohongyu789.top/gthlxrlekk.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.cdnleiting.top/gthwrjfytz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.havefunace.top/gtngtfnran.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.jiagoushi.top/gtcgduutwl.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.hfpthk.cn/gthzcrcwhc.html

[N04] 斐波那契数列
来源：http://hz.hywenlv.cn/gtvhrbdmos.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.cucudq.cn/gtnzgqdjlp.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.daxiang520.top/gtklmpcozh.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jinyuanbaomall.cn/gtsbjnthzd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.nanxuanxn.top/gtnrlgubya.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.pycfn.com/gttpeeokmn.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jinqigufen.top/gttqnuxnmc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.vqdsnc.cn/gtxqiokiif.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yonumen.top/gthllhukoi.html

[N05] 最大公约数
来源：http://hz.yangfankeji.com/gtuormvrwp.html

Py:   math.gcd(a, b)
来源：http://hz.xuanzx.com/gtsfljfbpf.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.tian-w.cn/gtvpbutgaq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhengqikj.top/gtbhtgrnjn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hnqzz.top/gtwkwqjpgm.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.zdqjudy.top/gtgiiitplh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.zhongyouzk.top/gtagqocjdi.html

Ruby: a.gcd(b)
来源：http://hz.meibo888.top/gtmowsngum.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.0kj1m.cn/gtyucfnsax.html

[N06] 判断回文字符串
来源：http://hz.jianghu66.top/gtplkdtpga.html

Py:   s == s[::-1]
来源：http://hz.yj202588.top/gtkgsunpje.html

PHP:  $s === strrev($s);
来源：http://hz.ydzc1.top/gtqkqiwrlg.html

JS:   s === [...s].reverse().join("")
来源：http://hz.tianlin.xyz/gtwztldxhz.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yongpay.top/gtlglazkmx.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.yueranfly.top/gtpwmspftt.html

Go:   // 双指针从两端比较
来源：http://hz.jyoumei.cn/gtpxuvxpeo.html

Ruby: s == s.reverse
来源：http://hz.shanyushiyangkeji.top/gtrrmevowf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yueranfly.top/gtelkmlluy.html

[N07] 两数之和（返回下标）
来源：http://hz.ppjwa.cn/gtpzdwckdz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.0kj1m.cn/gtlaiwswxl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yvedp.cn/gtqwomsibj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.hnxiangtu.top/gtowtdvvxt.html

TS:   // 手写 Map<string, number>
来源：http://hz.c1oappe.top/gtxeygviek.html

Java: // 手写 HashMap
来源：http://hz.kuanghao11.cn/gthslzxnbw.html

Go:   // 手写 map[int]int
来源：http://hz.shzxlz.cn/gtrzxkwtmm.html

Ruby: // 手写 Hash
来源：http://hz.sysykeji.top/gtphgnnffo.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.shanyushiyangkeji.top/gtdbjexomf.html

[N08] 生成全排列
来源：http://hz.daria6918.cn/gthvioumgy.html

Py:   itertools.permutations(arr)
来源：http://hz.cheryme.top/gtpfvtknpr.html

PHP:  // 手写递归交换
来源：http://hz.ivvv.top/gtdgexhqbt.html

JS:   // 手写回溯递归
来源：http://hz.zhaomingkeji.xyz/gtvzhaeyur.html

TS:   // 手写回溯递归
来源：http://hz.cqqwz.cn/gthfslnkgl.html

Java: // 手写回溯递归
来源：http://hz.zhiwuduotai.top/gtepksonow.html

Go:   // 手写回溯递归
来源：http://hz.ivvv.top/gtqpywvmvh.html

Ruby: arr.permutation.to_a
来源：http://hz.zhijiandao.cn/gtfkfugvle.html

C#:   // 手写回溯递归
来源：http://hz.chenjidiqi.icu/gtfkohrwpi.html

[N09] 栈与队列
来源：http://hz.gzhubu.top/gtbbjissmx.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.ppjwa.cn/gtyonlrqcd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.cdnleiting.top/gtmfgnvoir.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.xziqi.cn/gttuvqweki.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.sxryk.cn/gthewjkauh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.gzhubu.top/gteflcyubw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.birdmap.top/gtiwocrqyr.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.zhijiandao.cn/gtgpxtbjpw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.zhijiandao.cn/gtcpjkajgr.html

[N10] 链表节点定义
来源：http://hz.fengsongda.top/gtqcblghkz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.haohaochexian.top/gtxhqdrthx.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.sxryk.cn/gtlihybvre.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.aizwys.cn/gtypbgokij.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.cashguo.top/gtvemsmpso.html

Java: class Node { int v; Node next; }
来源：http://hz.hfpthk.cn/gttmsemnxp.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.jinyuanbaomall.cn/gttiusplzk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.yuxming.cn/gtyimegryr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.feifeiyinyue.top/gtsmkfkkrr.html

[N11] 二叉树中序遍历
来源：http://hz.xuanzx.com/gtsvysiczt.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.nanxinkj.top/gtqbvvlbyw.html

PHP:  // 手写递归函数
来源：http://hz.hongshengwenyu.top/gtkfngzzmq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.birdmap.top/gtsqkkwtek.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhijiandao.cn/gtfnnnrbhl.html

Java: // 手写递归
来源：http://hz.sxryk.cn/gtkzdglgkf.html

Go:   // 手写递归
来源：http://hz.dianchejie.cn/gtvvaxxjby.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.ehwqpu.com/gtooyrzwbk.html

C#:   // 手写递归
来源：http://hz.cashguo.top/gtaunmojsk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.sufxvd.cn/gtswlpruna.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.gotoacloud.top/gtudedklok.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.chenzaomai.com/gtwixrtypq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yuanzhike.top/gtbucbnumx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.gzhubu.top/gtlnvxbedo.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.gzhubu.top/gtxymrldix.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.xingfuxueyuan.xyz/gtclpdeper.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.hnxiangtu.top/gtcqdavglg.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.gzhubu.top/gteurqjfzr.html

================================================================================
来源：http://hz.andypj.xyz/gtlkfypuas.html

O. 并发与异步
来源：http://hz.ybcxt.top/gtfinnltkc.html

================================================================================
来源：http://hz.daxiang520.top/gtmccftejz.html

[O01] 启动一个线程
来源：http://hz.havefunace.top/gtxvsrcmsy.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.pengpengdd.cyou/gtcmgivlbg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.jyoumei.cn/gtahnfxtsb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.yj20258.top/gtylxaaohv.html

TS:   // 同 JS
来源：http://hz.jianghu66.top/gtwtxwvsca.html

Java: new Thread(() -> f()).start()
来源：http://hz.daxiang520.top/gtnyzceicm.html

Go:   go f()
来源：http://hz.andypj.xyz/gtoycpqohl.html

Ruby: Thread.new { f }
来源：http://hz.yonumen.top/gtfqlvcshl.html

C#:   Task.Run(() => F());
来源：http://hz.feifeiyinyue.top/gtcvjncdgb.html

[O02] 使用线程池
来源：http://hz.dianchejie.cn/gtjgjebkxy.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yangfankeji.com/gtckytbikf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.ydjk.org.cn/gtqivelols.html

JS:   // worker_threads 线程池
来源：http://hz.hfpthk.cn/gtfhtvgiio.html

TS:   // worker_threads 线程池
来源：http://hz.jqgufenzy.top/gtvrqvsbrf.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.shanyushiyangtech.top/gtktcocchy.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.dianchejie.cn/gtoctocdga.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.mhx1999.top/gtmxhonyeo.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.iojbl.cn/gtgfizsmhw.html

[O03] 加锁保护共享数据
来源：http://hz.316326.xyz/gtwswcbrfo.html

Py:   with lock: shared += 1
来源：http://hz.wangdashe.top/gtbmicxdcd.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.yonumen.top/gtzueqafth.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.tian-w.cn/gtmvkekzmp.html

TS:   // 同 JS
来源：http://hz.meibo888.top/gtwpwgabyt.html

Java: synchronized (this) { shared++; }
来源：http://hz.shanyushiyangtech.top/gtxbjrdqol.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.fzhhl.top/gttxktnopm.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.andypj.xyz/gtuegpwvfd.html

C#:   lock (gate) { shared++; }
来源：http://hz.gotoacloud.top/gtavsclhjf.html

[O04] 定义异步函数并等待
来源：http://hz.hfpthk.cn/gtnghqwibo.html

Py:   async def f():⏎    await g()
来源：http://hz.ydzc1.top/gtptxduagy.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.fengsongda.top/gtjsqwgwld.html

JS:   async function f() { await g(); }
来源：http://hz.iojbl.cn/gtmmoatdhw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.zhongyouzk.top/gtfltgvnmk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.dianchejie.cn/gtrkpymauy.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.dashuyun.cn/gtbsddkrsc.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.shzxlz.cn/gtbytzmmds.html

C#:   async Task F() { await G(); }
来源：http://hz.cqqwz.cn/gthzevkomy.html

[O05] 并发执行并等待全部完成
来源：http://hz.daria6918.cn/gtsedhdnrh.html

Py:   asyncio.gather(*tasks)
来源：http://hz.zhongyouzk.top/gtvtjscxsl.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.nanxuanxn.top/gtwgokahsj.html

JS:   await Promise.all(tasks)
来源：http://hz.yuanzhike.top/gtemchfpzk.html

TS:   await Promise.all(tasks)
来源：http://hz.yj202588.top/gtfogzwids.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.yongpay.top/gtmmyutypw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.dianchejie.cn/gtrwprftjr.html

Ruby: threads.map(&:join)
来源：http://hz.gzhubu.top/gtzrmuyodc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.chenzaomai.com/gtlkfwncrk.html

[O06] 使用进程池
来源：http://hz.dashuyun.cn/gtenechbhv.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.jyoumei.cn/gtlvwprrwg.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.kuanghao11.cn/gtngnsgxoz.html

JS:   // child_process / cluster 模块
来源：http://hz.jinqigufen.top/gtjkbtzggo.html

TS:   // child_process / cluster 模块
来源：http://hz.gogol.net.cn/gtczcysfac.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.cashguo.top/gtzylbhfdz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.vqdsnc.cn/gtxqhbgbpa.html

Ruby: // fork 块
来源：http://hz.pycfn.com/gtfcgyfmfm.html

C#:   Parallel.For
来源：http://hz.hywenlv.cn/gtxivfweap.html

================================================================================
来源：http://hz.aizwys.cn/gtwwcpklmd.html

P. 常用工具函数
来源：http://hz.316326.xyz/gtqxfkpiap.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtfrffspdu.html

[P01] 生成 UUID
来源：http://hz.xuanzx.com/gtxocklsnd.html

Py:   str(uuid.uuid4())
来源：http://hz.9152youxi.cn/gtgixydqck.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.smart0.xyz/gttockytae.html

JS:   crypto.randomUUID()
来源：http://hz.zhengqikj.top/gtewmjzefj.html

TS:   crypto.randomUUID()
来源：http://hz.sweek.top/gtkdpzrhsn.html

Java: UUID.randomUUID().toString()
来源：http://hz.bjfxy.top/gtcojiealx.html

Go:   // 用 github.com/google/uuid
来源：http://hz.xuanzx.com/gtytibspzd.html

Ruby: SecureRandom.uuid
来源：http://hz.jlsjyb.cn/gtsuprgzfl.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.feifeiyinyue.top/gtahwlxmpt.html

[P02] MD5 / SHA256 摘要
来源：http://hz.hysaishi.cn/gtxquucbwk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.xziqi.cn/gtfafccbcm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.yanxiufei.cn/gtckcxmqbs.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.xuanzx.com/gtgelcxral.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.tian-w.cn/gtlyqajttq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.shanyushiyangtech.top/gtcwcttvth.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.yonumen.top/gtuhyiwicd.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.zhiwuduotai.top/gthezyvfkr.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.0kj1m.cn/gtlquyritc.html

[P03] 生成短随机字符串
来源：http://hz.yonumen.top/gtmivheije.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.yvedp.cn/gteemkebdo.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.hnxiangtu.top/gtwjheahrc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ppjwa.cn/gtiowrgiib.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ivvv.top/gtmvxgyoyg.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yanxiufei.cn/gtrmkduvno.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.nwbrower.top/gtvhnordht.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jinghuilouyu.cn/gtciprdcyi.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jinqigfzy.top/gtygeuehwt.html

[P04] 求长度
来源：http://hz.aibaodan.cn/gtugaghrlv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.jlsjyb.cn/gtxbgwkmwe.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.snrcjt.cn/gthukjjurb.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ivvv.top/gtnjnntvwq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ydjk.org.cn/gtnyjahpka.html

Java: list.size();  map.size();  s.length()
来源：http://hz.dashuyun.cn/gtccexgegj.html

Go:   len(arr);  len(m)
来源：http://hz.haohaochexian.top/gtmedidckc.html

Ruby: x.length;  x.size
来源：http://hz.zdqjudy.top/gtjrxlcaqw.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.yuxming.cn/gtidvzvjqv.html

[P05] 判断两个对象内容是否相等
来源：http://hz.jinyuanbaomall.cn/gtfkarqtof.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.hammf.cn/gtfyfeuxwy.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.pengpengdd.cyou/gtszasfamf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.shanyushiyangtech.top/gtvewhjcwk.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zhaomingkeji.xyz/gtyftoubzc.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.fengsongda.top/gtxhzmjmfo.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.ehwqpu.com/gtnyxetxgb.html

Ruby: a == b
来源：http://hz.cashguo.top/gtaxptbfzc.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.jianghu66.top/gtbnzokphx.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.tanke756.top/gtpabsikcq.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.gaohongyu789.top/gtiyplqkgr.html

PHP:  if (empty($x)) {}
来源：http://hz.daxiang520.top/gtcvfohvhm.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.yongpay.top/gtoqaotjjy.html

TS:   if (x == null) {}
来源：http://hz.cucudq.cn/gtmbahqccu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.sysykeji.top/gtrxjomnxh.html

Go:   if x == nil {}
来源：http://hz.shzxlz.cn/gtiuzqmvty.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.ydjk.org.cn/gtcivuziuy.html

C#:   if (x is null) {}
来源：http://hz.shangyingyoupin.top/gtuhbxijpw.html

[P07] 防抖与节流
来源：http://hz.dianchejie.cn/gtwkqpyzxo.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.ppjwa.cn/gtqvlqtkdx.html

PHP:  // 手写时间戳比较
来源：http://hz.kuanghao11.cn/gteqznbjai.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cheryme.top/gtqmkmqmzv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xinyue.icu/gtdwschxjt.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.guowangkeji.top/gtkgpqrxnz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.nanxinkj.top/gtauoyikel.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.meibo888.top/gtkutvrzun.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.yangfankeji.com/gtmicqzgdv.html

[P08] 处理浮点精度问题
来源：http://hz.sweek.top/gthmsrabvc.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.xuetiantiany.cn/gtweeomloq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.ppjwa.cn/gtdazrmqhf.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.9152youxi.cn/gtneskegmk.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.c1oappe.top/gtlkuylqxe.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.zdqjudy.top/gtecppagnv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.jinghuilouyu.cn/gtrrhqcwzk.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.nanxuanxn.top/gtkwortwxi.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.c1oappe.top/gtogwbynip.html

================================================================================
来源：http://hz.guowangkeji.top/gtpinhfgji.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.vqdsnc.cn/gtuegkvseg.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtbzwyiyhe.html

[Q01] 创建表
来源：http://hz.yangfankeji.com/gtmtbbiytc.html

CREATE TABLE users (
来源：http://hz.yongpay.top/gtdfylxcnu.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.fzhhl.top/gtgvyhlpsl.html

name VARCHAR(50) NOT NULL,
来源：http://hz.wangshuangyany.cn/gtzdcnvofa.html

email VARCHAR(100) UNIQUE,
来源：http://hz.sufxvd.cn/gtaqwshcuc.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.meibo888.top/gtjxqpjdaz.html

);
来源：http://hz.cucudq.cn/gtqolkjkxz.html

[Q02] 创建带外键的表
来源：http://hz.xylfe.cn/gthabrezok.html

CREATE TABLE orders (
来源：http://hz.haohaochexian.top/gtqwrdgvke.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ivvv.top/gtsjlxqoih.html

user_id INT NOT NULL,
来源：http://hz.fengsongda.top/gtoubpgucj.html

amount DECIMAL(10, 2),
来源：http://hz.bjfxy.top/gtkzphamrm.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.nanxuanxn.top/gtruxtktnw.html

);
来源：http://hz.ehwqpu.com/gtveseogsp.html

[Q03] 增加列
来源：http://hz.redwolf501.top/gtjyfsmjci.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.sufxvd.cn/gtnokpddza.html

[Q04] 修改列类型
来源：http://hz.jqgfzy.top/gtffuyyegb.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.andypj.xyz/gtgsfmjwgb.html

[Q05] 重命名列
来源：http://hz.gaohongyu789.top/gtfrpqevnq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.shzxlz.cn/gtdtxfixso.html

[Q06] 删除列
来源：http://hz.birdmap.top/gtcvgyasta.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.ybcxt.top/gthbaxudli.html

[Q07] 删除表
来源：http://hz.ppjwa.cn/gtkdtzpixi.html

DROP TABLE IF EXISTS orders;
来源：http://hz.redwolf501.top/gtgtrhfzuc.html

[Q08] 创建普通索引
来源：http://hz.hfpthk.cn/gthpztnrpn.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.chenzaomai.com/gtzdwfglvr.html

[Q09] 创建唯一索引
来源：http://hz.bjfxy.top/gtojkozrat.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.shuidangran.top/gtawgsnonf.html

[Q10] 插入单行
来源：http://hz.yvedp.cn/gtwenmhdkx.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.yuxming.cn/gtmfgsmwex.html

[Q11] 一次插入多行
来源：http://hz.jinqigfzy.top/gtllsdqmlc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.shzxlz.cn/gtijcpqoja.html

[Q12] 插入后取自增 ID
来源：http://hz.cdnleiting.top/gtkdmtyqzv.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.chenjidiqi.icu/gtsixgaknu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.316326.xyz/gtbwchotye.html

[Q13] 忽略重复插入
来源：http://hz.xuanzx.com/gtqjrdswsf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.hywenlv.cn/gtdpxznldh.html

[Q14] 存在则更新（upsert）
来源：http://hz.yonumen.top/gtrtjtkqtq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.cucudq.cn/gtwqudkrmp.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.yanxiufei.cn/gtngdelxae.html

[Q15] 查询全部
来源：http://hz.hnxiangtu.top/gttkgvytbb.html

SELECT * FROM users;
来源：http://hz.316326.xyz/gtuyvuskfs.html

[Q16] 查询指定列
来源：http://hz.birdmap.top/gtvoardawp.html

SELECT id, name FROM users;
来源：http://hz.daxiang520.top/gtddtvbnon.html

[Q17] 条件查询
来源：http://hz.zhaomingkeji.xyz/gtiqfbcxuy.html


<!-- 参考信息 -->