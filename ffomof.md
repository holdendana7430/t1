代发 wailian999

TS:   process.platform;  process.version
来源：http://hz.feifeiyinyue.top/gtnxoanrcp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.gzhubu.top/gtkwlcjbep.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.sysykeji.top/gtjmrsblne.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.cashguo.top/gtiracbceb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.feifeiyinyue.top/gtstuvhmaf.html

================================================================================
来源：http://hz.redwolf501.top/gttsichmmv.html

N. 数据结构与算法
来源：http://hz.yangfankeji.com/gtfmzmynzk.html

================================================================================
来源：http://hz.sufxvd.cn/gtrxvfqrer.html

[N01] 二分查找（有序数组）
来源：http://hz.aizwys.cn/gtwlncfbvj.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.sweek.top/gtxhbhyyyr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jlsjyb.cn/gtufgtjxsc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jinghuilouyu.cn/gttcgicmfz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhijiandao.cn/gtykiefzwh.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.jlsjyb.cn/gtibwkxjgo.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.ehwqpu.com/gtflhkyhjy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.zycfv.cn/gtpsewkuwg.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.ppjwa.cn/gtxwfacvuu.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.shuidangran.top/gtshfhmzek.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shanyushiyangtech.top/gtqemrglnb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.zhaomingkeji.xyz/gtrgpuicth.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.guowangkeji.top/gtxrqkwssj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xziqi.cn/gtrisjaqla.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.hammf.cn/gtftylgquv.html

Go:   slices.Sort(arr)
来源：http://hz.316326.xyz/gtmkhxjmwj.html

Ruby: arr.sort
来源：http://hz.pycfn.com/gtmqzhdzgl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.zhiwuduotai.top/gtajhovmcp.html

[N03] 快速排序（分治示例）
来源：http://hz.dashuyun.cn/gtkbarxobi.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.ppjwa.cn/gtbbmicqfa.html

PHP:  // 递归实现，或用 usort
来源：http://hz.gzhubu.top/gtskfrrsiz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cashguo.top/gtbtkzlzag.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.shuidangran.top/gthqpzqlwp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.c1oappe.top/gtxkexhlsu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.daxiang520.top/gtznbpdlom.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.fengsongda.top/gtwizemiol.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yueranfly.top/gtaqdnjvez.html

[N04] 斐波那契数列
来源：http://hz.chenzaomai.com/gtghkzmlyp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jqgfzy.top/gtuqggidyd.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.yongpay.top/gtdmujmznw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhijiandao.cn/gtmlizkcic.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.fzhhl.top/gtwsdgcagz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.xinyue.icu/gtdbryohth.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.hfpthk.cn/gtfqkhhybk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.jlsjyb.cn/gtzqvifghl.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.dashuyun.cn/gtmubzwwig.html

[N05] 最大公约数
来源：http://hz.yuanzhike.top/gtwblftupl.html

Py:   math.gcd(a, b)
来源：http://hz.yj20258.top/gtoyjqkoml.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.ywan-chungtsiang.top/gtlgnahbvu.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.shzxlz.cn/gtbjocqoia.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.chenjidiqi.icu/gtijqfimjw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.9152youxi.cn/gtutcuekbp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.316326.xyz/gtumgdwpop.html

Ruby: a.gcd(b)
来源：http://hz.sxryk.cn/gtwsmthpbg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.ivvv.top/gtpdohzrnx.html

[N06] 判断回文字符串
来源：http://hz.zhoulong.xyz/gtmxsyevok.html

Py:   s == s[::-1]
来源：http://hz.zhoulong.xyz/gtkastayjy.html

PHP:  $s === strrev($s);
来源：http://hz.vqdsnc.cn/gtttxhbtsp.html

JS:   s === [...s].reverse().join("")
来源：http://hz.nanxinkj.top/gtkwthuboy.html

TS:   s === [...s].reverse().join("")
来源：http://hz.jqgufenzy.top/gtuxgdovsa.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.wangdashe.top/gtblizxtmc.html

Go:   // 双指针从两端比较
来源：http://hz.xinyue.icu/gtucoefipl.html

Ruby: s == s.reverse
来源：http://hz.andypj.xyz/gtrcjjnyit.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.bjfxy.top/gtlxsjiqvu.html

[N07] 两数之和（返回下标）
来源：http://hz.yj202588.top/gtshidvjjr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.gzhubu.top/gtmxngbdee.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.snrcjt.cn/gtoxgybkrx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.52xcode.cn/gturkctyvt.html

TS:   // 手写 Map<string, number>
来源：http://hz.ivvv.top/gtsifegahd.html

Java: // 手写 HashMap
来源：http://hz.cashguo.top/gtbunvrfsq.html

Go:   // 手写 map[int]int
来源：http://hz.xziqi.cn/gtzohbaxwq.html

Ruby: // 手写 Hash
来源：http://hz.yueranfly.top/gtlyhybqth.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.zycfv.cn/gtzabmolwq.html

[N08] 生成全排列
来源：http://hz.shzxlz.cn/gtntfhriam.html

Py:   itertools.permutations(arr)
来源：http://hz.xuetiantiany.cn/gtztkhpvnh.html

PHP:  // 手写递归交换
来源：http://hz.zhaomingkeji.xyz/gtrcmwkxpt.html

JS:   // 手写回溯递归
来源：http://hz.fzhhl.top/gtxdgummca.html

TS:   // 手写回溯递归
来源：http://hz.52xcode.cn/gtelqxyvrr.html

Java: // 手写回溯递归
来源：http://hz.xingfuxueyuan.xyz/gtjcczxldg.html

Go:   // 手写回溯递归
来源：http://hz.xuanzx.com/gtjjrwmfgo.html

Ruby: arr.permutation.to_a
来源：http://hz.dianchejie.cn/gtielvcose.html

C#:   // 手写回溯递归
来源：http://hz.jianghu66.top/gtnjszruei.html

[N09] 栈与队列
来源：http://hz.hammf.cn/gtneqqsdjr.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.shanyushiyangkeji.top/gtoacdttlg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.haohaochexian.top/gtijfihhwn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.meibo888.top/gtpjfvegua.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.ywan-chungtsiang.top/gtmyndjkxk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.shanyushiyangkeji.top/gtmutpfuup.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.pengpengdd.cyou/gtjpeijnjm.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.snrcjt.cn/gtuarmwnnf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.xylfe.cn/gtawsjjrkq.html

[N10] 链表节点定义
来源：http://hz.hfpthk.cn/gtajlmatcz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.kuanghao11.cn/gtwqcpwyno.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.shangyingyoupin.top/gtnotyzfmi.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zhiwuduotai.top/gtnqpuomwq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.9152youxi.cn/gtffjwqjvk.html

Java: class Node { int v; Node next; }
来源：http://hz.zdqjudy.top/gtvsvjlyjl.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.hammf.cn/gtbkqlppsp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.zhoulong.xyz/gtrniaxaza.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.snrcjt.cn/gtdqxnusrx.html

[N11] 二叉树中序遍历
来源：http://hz.svipenyu.cn/gtsawdsuqo.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.gogol.net.cn/gtgpglqrfh.html

PHP:  // 手写递归函数
来源：http://hz.redwolf501.top/gtgotgrmis.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhiwuduotai.top/gtkvnaudoz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yuanzhike.top/gtvbnjekty.html

Java: // 手写递归
来源：http://hz.yj202588.top/gtbbkgmizz.html

Go:   // 手写递归
来源：http://hz.zhoulong.xyz/gthlkcdksc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.tianlin.xyz/gtxkcnuhwp.html

C#:   // 手写递归
来源：http://hz.xingfuxueyuan.xyz/gtwhhvqnzd.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.svipenyu.cn/gtcilxpnao.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.ppjwa.cn/gtqrjqkgut.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jlsjyb.cn/gtfujrxfvv.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hywenlv.cn/gtglylnhjs.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.daria6918.cn/gtsyxhrjur.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.nanxinkj.top/gtyuezxagu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.cqqwz.cn/gtjjbxfmlw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.pengpengdd.cyou/gtwlumsjyc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ydzc1.top/gtwdomtwee.html

================================================================================
来源：http://hz.smart0.xyz/gtrjygfhsw.html

O. 并发与异步
来源：http://hz.guannengcc.top/gtxmyjaoti.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtjbpqwifl.html

[O01] 启动一个线程
来源：http://hz.pycfn.com/gtenirkszz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.yj20258888.top/gtmdenvfxm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.wangshuangyany.cn/gtezrmvnyj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.pengpengdd.cyou/gtppkolnlu.html

TS:   // 同 JS
来源：http://hz.quarkkingdee.top/gthamozjnn.html

Java: new Thread(() -> f()).start()
来源：http://hz.xuanzx.com/gtteehqebi.html

Go:   go f()
来源：http://hz.0kj1m.cn/gtrrqydjyl.html

Ruby: Thread.new { f }
来源：http://hz.jqgufenzy.top/gtaxeuuwus.html

C#:   Task.Run(() => F());
来源：http://hz.xziqi.cn/gtmbmahtug.html

[O02] 使用线程池
来源：http://hz.dianchejie.cn/gtqfkgfnwd.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.smart0.xyz/gtreaoxmfc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.zhaomingkeji.xyz/gtgeacjkaw.html

JS:   // worker_threads 线程池
来源：http://hz.svipenyu.cn/gtefzjaupi.html

TS:   // worker_threads 线程池
来源：http://hz.shanyushiyangtech.top/gthkszkudq.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.wangshuangyany.cn/gtlkzymilh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.sweek.top/gtrhjmozxn.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.shzxlz.cn/gtodsnsgcp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.hnxiangtu.top/gtqnhbmwgf.html

[O03] 加锁保护共享数据
来源：http://hz.wangdashe.top/gtaxupxjde.html

Py:   with lock: shared += 1
来源：http://hz.dianchejie.cn/gthypnavty.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.sxryk.cn/gtritxxqub.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.sweek.top/gtzpvosayb.html

TS:   // 同 JS
来源：http://hz.tian-w.cn/gtnztejcqh.html

Java: synchronized (this) { shared++; }
来源：http://hz.cheryme.top/gtpydhhcls.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.gzhubu.top/gtrsrbvxxs.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.yj20258.top/gtmkcqptdl.html

C#:   lock (gate) { shared++; }
来源：http://hz.jinyuanbaomall.cn/gtogebryms.html

[O04] 定义异步函数并等待
来源：http://hz.cashguo.top/gtmsuowzwt.html

Py:   async def f():⏎    await g()
来源：http://hz.gzhubu.top/gtafcoymab.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.smart0.xyz/gtuawxdgsw.html

JS:   async function f() { await g(); }
来源：http://hz.zhengqikj.top/gtwbxskweb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.tianlin.xyz/gtjwnjhnrm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.cashguo.top/gtwvveiukg.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.feifeiyinyue.top/gtuogjmdze.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.cashguo.top/gtbvaqcfaj.html

C#:   async Task F() { await G(); }
来源：http://hz.jiagoushi.top/gtsccwggcr.html

[O05] 并发执行并等待全部完成
来源：http://hz.zhengqikj.top/gtwpaxyurd.html

Py:   asyncio.gather(*tasks)
来源：http://hz.zhaomingkeji.xyz/gtgzukrrqo.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.9152youxi.cn/gtpgtgshfn.html

JS:   await Promise.all(tasks)
来源：http://hz.vqdsnc.cn/gtoyupvned.html

TS:   await Promise.all(tasks)
来源：http://hz.shzxlz.cn/gtmaozccix.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.ivvv.top/gtaigisdnp.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.vqdsnc.cn/gtmiqpiyme.html

Ruby: threads.map(&:join)
来源：http://hz.dianchejie.cn/gtsivoilpq.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.shuidangran.top/gtpzbhxfnr.html

[O06] 使用进程池
来源：http://hz.sxryk.cn/gtpgfzpztu.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.ywan-chungtsiang.top/gtalxianfp.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.ivvv.top/gtxrfdtulh.html

JS:   // child_process / cluster 模块
来源：http://hz.zhoulong.xyz/gtrhnyxdfo.html

TS:   // child_process / cluster 模块
来源：http://hz.yj20258.top/gtgntdxtmr.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.cashguo.top/gtiginhfgm.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.nanxuanxn.top/gtrsljubvg.html

Ruby: // fork 块
来源：http://hz.316326.xyz/gtdijciarz.html

C#:   Parallel.For
来源：http://hz.ivvv.top/gtapqlarin.html

================================================================================
来源：http://hz.sxryk.cn/gtmobhxfce.html

P. 常用工具函数
来源：http://hz.jqgufenzy.top/gtixxdudir.html

================================================================================
来源：http://hz.yj202588.top/gtwarludyq.html

[P01] 生成 UUID
来源：http://hz.ybcxt.top/gthodqbweg.html

Py:   str(uuid.uuid4())
来源：http://hz.zycfv.cn/gtpkbspjlc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.guowangkeji.top/gtndflnejo.html

JS:   crypto.randomUUID()
来源：http://hz.shanyushiyangkeji.top/gtehxynlun.html

TS:   crypto.randomUUID()
来源：http://hz.yj202588.top/gtfrmenrpn.html

Java: UUID.randomUUID().toString()
来源：http://hz.yanxiufei.cn/gtzryjvjop.html

Go:   // 用 github.com/google/uuid
来源：http://hz.zdqjudy.top/gtqmkduppg.html

Ruby: SecureRandom.uuid
来源：http://hz.52xcode.cn/gtmapouqzt.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.yuxming.cn/gtepjlrezo.html

[P02] MD5 / SHA256 摘要
来源：http://hz.gotoacloud.top/gtpvcxycex.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.aizwys.cn/gtccuajizp.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.chenzaomai.com/gtephxggiz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.hfpthk.cn/gterqfxfhz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.ydjk.org.cn/gtvxypeiri.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.gaohongyu789.top/gtzmptdhau.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.cucudq.cn/gtqizdzjmg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.guowangkeji.top/gtzccpadye.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.ydjk.org.cn/gtkwkztbtq.html

[P03] 生成短随机字符串
来源：http://hz.jinghuilouyu.cn/gtrktjnfmr.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.yonumen.top/gtgemzdmxu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.snrcjt.cn/gtbonzsnle.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jinyuanbaomall.cn/gtmsghhbki.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xinyue.icu/gtgdllltyy.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.smart0.xyz/gtndxdebxk.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.pengpengdd.cyou/gtkkxdmahl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.nwbrower.top/gtpqbizfnb.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.nanxuanxn.top/gtgiexdgdr.html

[P04] 求长度
来源：http://hz.tian-w.cn/gttmejiabt.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.chenjidiqi.icu/gtbnyjsoys.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jinyuanbaomall.cn/gtvvkvviwq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jinqigfzy.top/gtsgmbtwek.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.aizwys.cn/gtxlnclznw.html

Java: list.size();  map.size();  s.length()
来源：http://hz.tian-w.cn/gtkepptilj.html

Go:   len(arr);  len(m)
来源：http://hz.jinqigfzy.top/gtirukqcjj.html

Ruby: x.length;  x.size
来源：http://hz.tian-w.cn/gtpmftgbqh.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.snrcjt.cn/gtmmfnilyb.html

[P05] 判断两个对象内容是否相等
来源：http://hz.0kj1m.cn/gtwzmzgkhh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.zhijiandao.cn/gthdeqhgip.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.jinqigfzy.top/gthcsosrjj.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.nwbrower.top/gtelyuvzzi.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.sysykeji.top/gtwbujuamh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.shangyingyoupin.top/gtvrjqiwen.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.svipenyu.cn/gtqubwslfk.html

Ruby: a == b
来源：http://hz.jqgfzy.top/gtoxlbuyic.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.52xcode.cn/gttowwgzct.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.yangfankeji.com/gtolgrrjgt.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.zhixingplan.top/gtkxjajhlo.html

PHP:  if (empty($x)) {}
来源：http://hz.yuanzhike.top/gthqfveoas.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.ydzc1.top/gtjngzpnej.html

TS:   if (x == null) {}
来源：http://hz.yuxming.cn/gtrserbuen.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.nanxinkj.top/gtydynkzrm.html

Go:   if x == nil {}
来源：http://hz.ybcxt.top/gtetkeynzc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jinqigfzy.top/gtedsgznzo.html

C#:   if (x is null) {}
来源：http://hz.nwbrower.top/gtynvrkehf.html

[P07] 防抖与节流
来源：http://hz.tanke756.top/gtustajnbk.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.gogol.net.cn/gtoprrthnx.html

PHP:  // 手写时间戳比较
来源：http://hz.guannengcc.top/gtifyshjmx.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.chenjidiqi.icu/gtcfbsfwep.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.vqdsnc.cn/gtofjfutlz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.52xcode.cn/gtkjidmvrq.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.guannengcc.top/gtqsmdxorf.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.ywan-chungtsiang.top/gtfbvrvrwc.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.9152youxi.cn/gtroenryzu.html

[P08] 处理浮点精度问题
来源：http://hz.tanke756.top/gtfwoizjqr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.zhixingplan.top/gtaojlvgvl.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.zhoulong.xyz/gtphoxkqsp.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.zdqjudy.top/gtoxdprtqb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.zhixingplan.top/gtdjcyyvca.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.haohaochexian.top/gtgdlaqzkl.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.tian-w.cn/gtahihumkf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.dianchejie.cn/gthhnlbyjp.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.iojbl.cn/gtvckugifc.html

================================================================================
来源：http://hz.svipenyu.cn/gtqcfyhcxg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.tanke756.top/gttnopejxa.html

================================================================================
来源：http://hz.cashguo.top/gtlikkeydk.html

[Q01] 创建表
来源：http://hz.pengpengdd.cyou/gtmgzxqghr.html

CREATE TABLE users (
来源：http://hz.jianghu66.top/gtintlzylv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhengqikj.top/gtxhydjlwp.html

name VARCHAR(50) NOT NULL,
来源：http://hz.jinqigfzy.top/gtywptvsdd.html

email VARCHAR(100) UNIQUE,
来源：http://hz.ehwqpu.com/gtznuefdkg.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.havefunace.top/gturbdwhgs.html

);
来源：http://hz.hammf.cn/gtclyepdza.html

[Q02] 创建带外键的表
来源：http://hz.nanxinkj.top/gtfhnnvzdj.html

CREATE TABLE orders (
来源：http://hz.jqgfzy.top/gtzyfqvjzw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.guannengcc.top/gtcxcwtdyg.html

user_id INT NOT NULL,
来源：http://hz.0kj1m.cn/gtwmyaqqim.html

amount DECIMAL(10, 2),
来源：http://hz.tianlin.xyz/gtuhehfeye.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.zhijiandao.cn/gtcxzqvnku.html

);
来源：http://hz.smart0.xyz/gtxjyrzizr.html

[Q03] 增加列
来源：http://hz.hnxiangtu.top/gttwpswjmy.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.havefunace.top/gtlhalxnvf.html

[Q04] 修改列类型
来源：http://hz.yanxiufei.cn/gtcbiancur.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.cheryme.top/gtifdjxflm.html

[Q05] 重命名列
来源：http://hz.0kj1m.cn/gtiyycyaze.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.c1oappe.top/gtrtxtpujx.html

[Q06] 删除列
来源：http://hz.zhoulong.xyz/gtrafolctr.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.ydzc1.top/gtdznnhugx.html

[Q07] 删除表
来源：http://hz.316326.xyz/gtrvjpgucu.html

DROP TABLE IF EXISTS orders;
来源：http://hz.vqdsnc.cn/gtuhmynzxf.html

[Q08] 创建普通索引
来源：http://hz.gaohongyu789.top/gtazrvxumk.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.quarkkingdee.top/gtjcogqytq.html

[Q09] 创建唯一索引
来源：http://hz.hywenlv.cn/gtraherhbm.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.nanxinkj.top/gtwcilsppx.html

[Q10] 插入单行
来源：http://hz.vqdsnc.cn/gtgcukujqe.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.fzhhl.top/gtlugascxw.html

[Q11] 一次插入多行
来源：http://hz.zhiwuduotai.top/gtjemqmqcs.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.hnxiangtu.top/gthuuvowwt.html

[Q12] 插入后取自增 ID
来源：http://hz.havefunace.top/gtjllkumeh.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.nwbrower.top/gtvodgidgz.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.hammf.cn/gtzmjyvdiy.html

[Q13] 忽略重复插入
来源：http://hz.0kj1m.cn/gtshxuohjx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.cashguo.top/gtkjrlajnk.html

[Q14] 存在则更新（upsert）
来源：http://hz.jyoumei.cn/gtroojvjnx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.wangdashe.top/gtgbdxipal.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.yuxming.cn/gtlgjvkqni.html

[Q15] 查询全部
来源：http://hz.c1oappe.top/gtmzfcawye.html

SELECT * FROM users;
来源：http://hz.tianlin.xyz/gtabncfpbu.html

[Q16] 查询指定列
来源：http://hz.c1oappe.top/gtvmmctvkz.html

SELECT id, name FROM users;
来源：http://hz.9152youxi.cn/gtdgbqkved.html

[Q17] 条件查询
来源：http://hz.jinyuanbaomall.cn/gtluvczhvw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.hongshengwenyu.top/gtkuhutbor.html

[Q18] 模糊匹配
来源：http://hz.ehwqpu.com/gtsajsfqwq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.jinghuilouyu.cn/gtnnhahgco.html

[Q19] 范围查询
来源：http://hz.yuanzhike.top/gtjcivtrec.html


<!-- 参考信息 -->