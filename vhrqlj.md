代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.hnqzz.top/gtrhzhrtss.html

================================================================================
来源：http://hz.xylfe.cn/gtztcnuuvx.html

N. 数据结构与算法
来源：http://hz.wangshuangyany.cn/gtuioyyzyo.html

================================================================================
来源：http://hz.birdmap.top/gthncpeejh.html

[N01] 二分查找（有序数组）
来源：http://hz.dashuyun.cn/gtdsjrctne.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.aizwys.cn/gtgluvxvdm.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yanxiufei.cn/gtzwfinhhv.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.fengsongda.top/gtzlapkwqm.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.haohaochexian.top/gtkpyknylw.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.hywenlv.cn/gtjternomu.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.sxryk.cn/gtwcimpulg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.yj20258.top/gtpnpwjflr.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.havefunace.top/gtbbgbycnf.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.shzxlz.cn/gtquwruode.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.nanxuanxn.top/gtddzkbgyo.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.zycfv.cn/gtayvzbdos.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hammf.cn/gthvtppgng.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.iojbl.cn/gtzsjwjkmj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.andypj.xyz/gtrmcmzdwc.html

Go:   slices.Sort(arr)
来源：http://hz.ydzc1.top/gtfpisodbe.html

Ruby: arr.sort
来源：http://hz.ywan-chungtsiang.top/gtegwlvayf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.cashguo.top/gtviicchci.html

[N03] 快速排序（分治示例）
来源：http://hz.jyoumei.cn/gtyucwoqhk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.hongshengwenyu.top/gtibabvjqp.html

PHP:  // 递归实现，或用 usort
来源：http://hz.daria6918.cn/gtxrgpyxtp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cdnleiting.top/gtqbfrrtfz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.shanyushiyangtech.top/gthzbdpzos.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.feifeiyinyue.top/gttvqucfof.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.zhengqikj.top/gtiycsdhxl.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.chenlongwang.top/gtzgbwpsuq.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.chenlongwang.top/gteqvdsnsp.html

[N04] 斐波那契数列
来源：http://hz.bjfxy.top/gtexumsgjw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.0kj1m.cn/gtjzikerzx.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.ivvv.top/gtwzsuemzm.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.nanxinkj.top/gtemnjeaqz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.feifeiyinyue.top/gtbdescmdf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.9152youxi.cn/gtewjszlah.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.gotoacloud.top/gtomiqmnce.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.jinqigfzy.top/gtgsgzyinp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.havefunace.top/gtyvnppepi.html

[N05] 最大公约数
来源：http://hz.tian-w.cn/gtvmqjnjel.html

Py:   math.gcd(a, b)
来源：http://hz.zhijiandao.cn/gtbzuyxqsb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.xziqi.cn/gtawalszhj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xuanzx.com/gtxwgtqpxa.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.dianchejie.cn/gtglymmbld.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.daria6918.cn/gtebzqanwh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.sufxvd.cn/gtxvxryggc.html

Ruby: a.gcd(b)
来源：http://hz.52xcode.cn/gtezdpzahi.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.fengsongda.top/gtwoducjuw.html

[N06] 判断回文字符串
来源：http://hz.shanyushiyangkeji.top/gtujqemibb.html

Py:   s == s[::-1]
来源：http://hz.zhongyouzk.top/gtnuzzusju.html

PHP:  $s === strrev($s);
来源：http://hz.wangshuangyany.cn/gtbvelfsgt.html

JS:   s === [...s].reverse().join("")
来源：http://hz.quarkkingdee.top/gtdcjmfgdv.html

TS:   s === [...s].reverse().join("")
来源：http://hz.cdnleiting.top/gtqbvicnup.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.dianchejie.cn/gtnhofngrg.html

Go:   // 双指针从两端比较
来源：http://hz.zhijiandao.cn/gtsbltgldg.html

Ruby: s == s.reverse
来源：http://hz.hysaishi.cn/gtjakgdkte.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.gotoacloud.top/gtvtmhkvzg.html

[N07] 两数之和（返回下标）
来源：http://hz.jinqigfzy.top/gtmtphpqab.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.smart0.xyz/gtaqzvqwyr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.ppjwa.cn/gtpwhdmuzj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.birdmap.top/gttctwzfni.html

TS:   // 手写 Map<string, number>
来源：http://hz.yuanzhike.top/gtkmlgrtit.html

Java: // 手写 HashMap
来源：http://hz.zhaomingkeji.xyz/gtbvqqhvrq.html

Go:   // 手写 map[int]int
来源：http://hz.gaohongyu789.top/gtewuhzsre.html

Ruby: // 手写 Hash
来源：http://hz.yj20258888.top/gtpjizwykc.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yangfankeji.com/gtbebmzucl.html

[N08] 生成全排列
来源：http://hz.hysaishi.cn/gtplniblxj.html

Py:   itertools.permutations(arr)
来源：http://hz.shzxlz.cn/gtborjramg.html

PHP:  // 手写递归交换
来源：http://hz.ppjwa.cn/gtcxqygxdj.html

JS:   // 手写回溯递归
来源：http://hz.shzxlz.cn/gtimckxiwu.html

TS:   // 手写回溯递归
来源：http://hz.ydjk.org.cn/gtntvutlfw.html

Java: // 手写回溯递归
来源：http://hz.jinghuilouyu.cn/gtspywutud.html

Go:   // 手写回溯递归
来源：http://hz.wangshuangyany.cn/gtaxfhywqb.html

Ruby: arr.permutation.to_a
来源：http://hz.zhengqikj.top/gtgocfwzff.html

C#:   // 手写回溯递归
来源：http://hz.yonumen.top/gtfpjdikan.html

[N09] 栈与队列
来源：http://hz.svipenyu.cn/gtxjpcrqbx.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.cqqwz.cn/gtqcfkrkwo.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.iojbl.cn/gttskgnnnd.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.hongshengwenyu.top/gtzbwobkys.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.svipenyu.cn/gtlxgnzoyn.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.zhengqikj.top/gtugtwnuwl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.shuidangran.top/gtkcpdywuw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.ybcxt.top/gtdnvrchck.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.cucudq.cn/gtezpbyvto.html

[N10] 链表节点定义
来源：http://hz.hnxiangtu.top/gtuefuapot.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.smart0.xyz/gtdvzzxhna.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.hnxiangtu.top/gtblzzlonh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yuxming.cn/gtqhlhfjxq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.shanyushiyangtech.top/gtvjpmfgoy.html

Java: class Node { int v; Node next; }
来源：http://hz.cashguo.top/gttyxlxdva.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.yangfankeji.com/gtbwdivorh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.hongshengwenyu.top/gtbwyjjfmk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.jyoumei.cn/gteulqkofh.html

[N11] 二叉树中序遍历
来源：http://hz.316326.xyz/gtscttlywa.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.svipenyu.cn/gtdknpozby.html

PHP:  // 手写递归函数
来源：http://hz.nanxinkj.top/gtzlgmpxnd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.havefunace.top/gtidjvtdco.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.sweek.top/gteghaftbj.html

Java: // 手写递归
来源：http://hz.yonumen.top/gtbjuqqgpu.html

Go:   // 手写递归
来源：http://hz.pengpengdd.cyou/gtdzvpkrls.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.hfpthk.cn/gtfczuxpyo.html

C#:   // 手写递归
来源：http://hz.yanxiufei.cn/gtsenkxand.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.xuanzx.com/gtigkyzwfn.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.sweek.top/gtsrpsygfg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.shanyushiyangtech.top/gtctabqjqj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jqgfzy.top/gtrgnbgjig.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.birdmap.top/gtbsfekilf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.shuidangran.top/gtwzwcwkyh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.aibaodan.cn/gtycpivzlj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.chenzaomai.com/gtpscphsar.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.sufxvd.cn/gtqzcvindb.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtktaqjepc.html

O. 并发与异步
来源：http://hz.9152youxi.cn/gtjdwnykmv.html

================================================================================
来源：http://hz.aibaodan.cn/gtyvirhfus.html

[O01] 启动一个线程
来源：http://hz.jiagoushi.top/gtcuhyqmfv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.zycfv.cn/gtoqlkeofm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.chenlongwang.top/gtrplaacjp.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.dashuyun.cn/gtflalsfnh.html

TS:   // 同 JS
来源：http://hz.sufxvd.cn/gtmkcbmwen.html

Java: new Thread(() -> f()).start()
来源：http://hz.pycfn.com/gtqkljazor.html

Go:   go f()
来源：http://hz.tianlin.xyz/gtzqzvswyb.html

Ruby: Thread.new { f }
来源：http://hz.yvedp.cn/gtslexunuw.html

C#:   Task.Run(() => F());
来源：http://hz.guowangkeji.top/gtozhawded.html

[O02] 使用线程池
来源：http://hz.feifeiyinyue.top/gtbbokgrxe.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.pengpengdd.cyou/gtyxvxmrzs.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.smart0.xyz/gtnsyehczp.html

JS:   // worker_threads 线程池
来源：http://hz.xuanzx.com/gtynkojmge.html

TS:   // worker_threads 线程池
来源：http://hz.smart0.xyz/gtspyrxgqk.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.zhiwuduotai.top/gtkrujjrpb.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.chenlongwang.top/gtlunxwndj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.ybcxt.top/gtfdwfzipv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.xingfuxueyuan.xyz/gtomdpudny.html

[O03] 加锁保护共享数据
来源：http://hz.xylfe.cn/gtbgeyxydp.html

Py:   with lock: shared += 1
来源：http://hz.zhoulong.xyz/gtwlirarbt.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.xingfuxueyuan.xyz/gtbspcwmmn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.wangdashe.top/gteijxkbbs.html

TS:   // 同 JS
来源：http://hz.havefunace.top/gtuimlslml.html

Java: synchronized (this) { shared++; }
来源：http://hz.aibaodan.cn/gtgmtlzkyl.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.xylfe.cn/gtshxgutlp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.cqqwz.cn/gtitajulfb.html

C#:   lock (gate) { shared++; }
来源：http://hz.pengpengdd.cyou/gtgrrmzxks.html

[O04] 定义异步函数并等待
来源：http://hz.ivvv.top/gtprmvtxcx.html

Py:   async def f():⏎    await g()
来源：http://hz.chenzaomai.com/gtnqklnnrx.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.bjfxy.top/gtaalrvvsf.html

JS:   async function f() { await g(); }
来源：http://hz.shanyushiyangkeji.top/gteefmruaf.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.quarkkingdee.top/gtilkbgold.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.daria6918.cn/gtlsywjfpy.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.316326.xyz/gtnbzujase.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.zhoulong.xyz/gtaetcwxuu.html

C#:   async Task F() { await G(); }
来源：http://hz.hywenlv.cn/gtpsiqcevo.html

[O05] 并发执行并等待全部完成
来源：http://hz.daxiang520.top/gtkjniruko.html

Py:   asyncio.gather(*tasks)
来源：http://hz.hnqzz.top/gtsakkoiqm.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.52xcode.cn/gtxcqkzfxs.html

JS:   await Promise.all(tasks)
来源：http://hz.chenlongwang.top/gtrmcrwfky.html

TS:   await Promise.all(tasks)
来源：http://hz.ppjwa.cn/gtxjixflqt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.birdmap.top/gtdivcjmmx.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.nanxinkj.top/gtqqsgakjf.html

Ruby: threads.map(&:join)
来源：http://hz.yj20258888.top/gtjlruzzsg.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.xuanzx.com/gtrmsrvdvu.html

[O06] 使用进程池
来源：http://hz.hammf.cn/gtuuelwvre.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.zhengqikj.top/gtqzezbqhn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.vqdsnc.cn/gtowzzerfx.html

JS:   // child_process / cluster 模块
来源：http://hz.wangdashe.top/gtukpyifzh.html

TS:   // child_process / cluster 模块
来源：http://hz.chenlongwang.top/gtuxnocbzg.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.9152youxi.cn/gtgkluqorw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.9152youxi.cn/gtgspwuxte.html

Ruby: // fork 块
来源：http://hz.hnqzz.top/gtiyauketv.html

C#:   Parallel.For
来源：http://hz.daria6918.cn/gtpnpoferz.html

================================================================================
来源：http://hz.jinqigfzy.top/gtqqqrwxrw.html

P. 常用工具函数
来源：http://hz.daria6918.cn/gthievjaoe.html

================================================================================
来源：http://hz.tanke756.top/gtlifdwzvz.html

[P01] 生成 UUID
来源：http://hz.havefunace.top/gtrhuuuong.html

Py:   str(uuid.uuid4())
来源：http://hz.52xcode.cn/gtjjmiiqpw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jqgufenzy.top/gtbbiopkrd.html

JS:   crypto.randomUUID()
来源：http://hz.xziqi.cn/gthdbmiblr.html

TS:   crypto.randomUUID()
来源：http://hz.sxryk.cn/gtbdhmhhwa.html

Java: UUID.randomUUID().toString()
来源：http://hz.dashuyun.cn/gtwovtmyyt.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yj20258.top/gtisxolmxk.html

Ruby: SecureRandom.uuid
来源：http://hz.pengpengdd.cyou/gtgxojiaoo.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.chenjidiqi.icu/gtdackpaen.html

[P02] MD5 / SHA256 摘要
来源：http://hz.aibaodan.cn/gtestpbker.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.meibo888.top/gtjdxyavhe.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.chenzaomai.com/gtjlnpuinp.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.ydzc1.top/gtxeqdnyfm.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.sufxvd.cn/gtatrrduzf.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.shanyushiyangkeji.top/gtfazswrjm.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.jqgufenzy.top/gtbjpltqnn.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.0kj1m.cn/gtffenzear.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.xuanzx.com/gtrjxzsmdh.html

[P03] 生成短随机字符串
来源：http://hz.chenzaomai.com/gttumomuby.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.tianlin.xyz/gteguxoybb.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.wangshuangyany.cn/gtsnkjglsz.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yanxiufei.cn/gtclfvfhqq.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jinyuanbaomall.cn/gtanvzoylx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.wangshuangyany.cn/gtorbqnwqm.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.ydzc1.top/gtavfgjjwp.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.shanyushiyangtech.top/gtkqqurnrf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.sufxvd.cn/gtxuhdyuio.html

[P04] 求长度
来源：http://hz.ywan-chungtsiang.top/gtqpsnkhmc.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.guannengcc.top/gtlbftkati.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhiwuduotai.top/gtkpbroham.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xinyue.icu/gtntkfxtjn.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.iojbl.cn/gtzgbirsqf.html

Java: list.size();  map.size();  s.length()
来源：http://hz.zhixingplan.top/gttynuefje.html

Go:   len(arr);  len(m)
来源：http://hz.shuidangran.top/gteozobuvi.html

Ruby: x.length;  x.size
来源：http://hz.yongpay.top/gtwqotmugt.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.gotoacloud.top/gtqttbddvq.html

[P05] 判断两个对象内容是否相等
来源：http://hz.nwbrower.top/gtuqjsurjp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.xuanzx.com/gtlnrnuacb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.gotoacloud.top/gtyaxjqcvj.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.c1oappe.top/gtlaymablp.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.haohaochexian.top/gtkptwelrh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.shzxlz.cn/gtgnjxcetr.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.hfpthk.cn/gtyuquwwgu.html

Ruby: a == b
来源：http://hz.guannengcc.top/gtjtcnbcrs.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.hnxiangtu.top/gtddmqvzka.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.zhoulong.xyz/gtpjvamfjg.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.yonumen.top/gtqejztbuh.html

PHP:  if (empty($x)) {}
来源：http://hz.xinyue.icu/gtysqflvgl.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.wangdashe.top/gtguoesivo.html

TS:   if (x == null) {}
来源：http://hz.zhixingplan.top/gtxbxshsno.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.9152youxi.cn/gtsfixkiun.html

Go:   if x == nil {}
来源：http://hz.chenlongwang.top/gtprvhvcfl.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.cdnleiting.top/gtrqwjqkjd.html

C#:   if (x is null) {}
来源：http://hz.zhiwuduotai.top/gthanhcuzo.html

[P07] 防抖与节流
来源：http://hz.cucudq.cn/gtflxnojdd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.shanyushiyangkeji.top/gtdppsofnr.html

PHP:  // 手写时间戳比较
来源：http://hz.aibaodan.cn/gtkgzqrwrm.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.pengpengdd.cyou/gtvnldbfrz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.haohaochexian.top/gtdtfccvlu.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.dianchejie.cn/gtqwatsrmk.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.sufxvd.cn/gtzrlntsah.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.jiagoushi.top/gtffcttast.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.jinqigufen.top/gtevedzoqa.html

[P08] 处理浮点精度问题
来源：http://hz.shanyushiyangtech.top/gtqdutvvna.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.fengsongda.top/gtgspuvsqs.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.meibo888.top/gtrjtjwxhw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.ydzc1.top/gtzzbhexbm.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.jlsjyb.cn/gttvhjdvir.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.zhoulong.xyz/gtnhbtvbnr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.316326.xyz/gthxvqylub.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.shanyushiyangkeji.top/gtudjnynoi.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.guowangkeji.top/gtmixbilbj.html

================================================================================
来源：http://hz.cheryme.top/gtbpppvixp.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.wangshuangyany.cn/gtvvncosli.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtybadlahv.html

[Q01] 创建表
来源：http://hz.yanxiufei.cn/gtipiuigfn.html

CREATE TABLE users (
来源：http://hz.svipenyu.cn/gtkmmonnzn.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.aizwys.cn/gtaqmhtujj.html

name VARCHAR(50) NOT NULL,
来源：http://hz.redwolf501.top/gtdwxvukmf.html

email VARCHAR(100) UNIQUE,
来源：http://hz.dianchejie.cn/gticgkihrl.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.ppjwa.cn/gthfajjbhu.html

);
来源：http://hz.fzhhl.top/gtyfisplgj.html

[Q02] 创建带外键的表
来源：http://hz.zhiwuduotai.top/gtaeziuxoh.html

CREATE TABLE orders (
来源：http://hz.guowangkeji.top/gtefjdacoh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.svipenyu.cn/gtkldunmqj.html

user_id INT NOT NULL,
来源：http://hz.zhiwuduotai.top/gtzsnelxxp.html

amount DECIMAL(10, 2),
来源：http://hz.ywan-chungtsiang.top/gtjbprwgqk.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.dashuyun.cn/gtzqfcvzrc.html

);
来源：http://hz.yonumen.top/gtxjivliys.html

[Q03] 增加列
来源：http://hz.fengsongda.top/gthxpszxxk.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.hfpthk.cn/gtvbgakpnl.html

[Q04] 修改列类型
来源：http://hz.jiagoushi.top/gtokneslkc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.nanxuanxn.top/gtjpqbbztm.html

[Q05] 重命名列
来源：http://hz.hnqzz.top/gtltmwukie.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.mhx1999.top/gttvdudssi.html

[Q06] 删除列
来源：http://hz.jqgfzy.top/gtfhxopoua.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.ppjwa.cn/gtkkrwcscv.html

[Q07] 删除表
来源：http://hz.9152youxi.cn/gtyvnddyhr.html

DROP TABLE IF EXISTS orders;
来源：http://hz.yuxming.cn/gtfazonwbi.html

[Q08] 创建普通索引
来源：http://hz.zhaomingkeji.xyz/gtilsxcelf.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.ehwqpu.com/gtaruarvgo.html

[Q09] 创建唯一索引
来源：http://hz.fzhhl.top/gtggdvlgtl.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.shanyushiyangkeji.top/gtryduslwv.html

[Q10] 插入单行
来源：http://hz.zhengqikj.top/gtlnkdmjxs.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.yanxiufei.cn/gtgwpoxmqb.html

[Q11] 一次插入多行
来源：http://hz.shanyushiyangtech.top/gtckwctltd.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yongpay.top/gtennobdsw.html

[Q12] 插入后取自增 ID
来源：http://hz.yvedp.cn/gtxwdqdzva.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.cheryme.top/gtohhmhady.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yj202588.top/gtwlzlznwm.html

[Q13] 忽略重复插入
来源：http://hz.redwolf501.top/gtzsrujajo.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.daxiang520.top/gtyrkxrwtj.html

[Q14] 存在则更新（upsert）
来源：http://hz.yuxming.cn/gtbrppuvsz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.nanxuanxn.top/gtaedgphna.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.andypj.xyz/gtutmcelkj.html

[Q15] 查询全部
来源：http://hz.feifeiyinyue.top/gtolxcfxkt.html

SELECT * FROM users;
来源：http://hz.shanyushiyangtech.top/gtrnkkvexn.html

[Q16] 查询指定列
来源：http://hz.yvedp.cn/gtxliwookz.html

SELECT id, name FROM users;
来源：http://hz.zhijiandao.cn/gtkekcpuka.html

[Q17] 条件查询
来源：http://hz.xingfuxueyuan.xyz/gtfugwanwr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.gzhubu.top/gtkmreypbg.html

[Q18] 模糊匹配
来源：http://hz.meibo888.top/gtxwlxxvbk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.zhaomingkeji.xyz/gttnfkhodb.html

[Q19] 范围查询
来源：http://hz.andypj.xyz/gtwwnjqnab.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.chenlongwang.top/gtpedciist.html

[Q20] IN 列表
来源：http://hz.chenlongwang.top/gtdisaxxqp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.ehwqpu.com/gtbhfjikpd.html

[Q21] 空值判断
来源：http://hz.chenlongwang.top/gttsqrkmur.html


<!-- 参考信息 -->