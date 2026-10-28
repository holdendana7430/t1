代发 wailian999

Ruby: arr.sort
来源：http://hz.chenjidiqi.icu/gtndhauydx.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.ydjk.org.cn/gtvaaotfzo.html

[N03] 快速排序（分治示例）
来源：http://hz.yongpay.top/gtmvvxemun.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.ehwqpu.com/gtixvbedbn.html

PHP:  // 递归实现，或用 usort
来源：http://hz.dianchejie.cn/gtzfvypbln.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.chenjidiqi.icu/gtpavlmsas.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.gotoacloud.top/gtpfsahqum.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.feifeiyinyue.top/gtknjjsjdk.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.gotoacloud.top/gtvcbxzanm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.birdmap.top/gtqmhpkdjq.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yangfankeji.com/gtygsfrxke.html

[N04] 斐波那契数列
来源：http://hz.nanxuanxn.top/gtssrdtysf.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.wangshuangyany.cn/gtzmkanejw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.cashguo.top/gtntppncgu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yj20258888.top/gtvyhbbpdr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jyoumei.cn/gtkqfwyqzr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.zhoulong.xyz/gtaodrxzxw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.mhx1999.top/gtcertrijo.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.wangshuangyany.cn/gtduemkevn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.bjfxy.top/gtrvghtdcl.html

[N05] 最大公约数
来源：http://hz.nanxinkj.top/gthpgrhela.html

Py:   math.gcd(a, b)
来源：http://hz.tanke756.top/gtzbexoeqd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.aizwys.cn/gthqpotaqv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.nwbrower.top/gtopjaeftq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.aizwys.cn/gtgjrttwdw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.shuidangran.top/gtkgollyrp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.zhengqikj.top/gtfcgeserl.html

Ruby: a.gcd(b)
来源：http://hz.gaohongyu789.top/gtwctsrqiq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.sufxvd.cn/gtoyehhfjb.html

[N06] 判断回文字符串
来源：http://hz.chenlongwang.top/gtrdyfrmay.html

Py:   s == s[::-1]
来源：http://hz.aibaodan.cn/gtsieohcyb.html

PHP:  $s === strrev($s);
来源：http://hz.chenjidiqi.icu/gtvnvgzklj.html

JS:   s === [...s].reverse().join("")
来源：http://hz.9152youxi.cn/gtlvgslozd.html

TS:   s === [...s].reverse().join("")
来源：http://hz.zycfv.cn/gtxlwikowb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jinqigfzy.top/gtopljfdpp.html

Go:   // 双指针从两端比较
来源：http://hz.xuetiantiany.cn/gtyrihzffk.html

Ruby: s == s.reverse
来源：http://hz.wangdashe.top/gtxtoqinlg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.ivvv.top/gtxsepbmfk.html

[N07] 两数之和（返回下标）
来源：http://hz.bjfxy.top/gtekvezwyv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.shanyushiyangkeji.top/gtighahqsq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yanxiufei.cn/gtsethfuec.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.zhiwuduotai.top/gtfjrbcjws.html

TS:   // 手写 Map<string, number>
来源：http://hz.xinyue.icu/gttmvivlnk.html

Java: // 手写 HashMap
来源：http://hz.cqqwz.cn/gtuacanjjl.html

Go:   // 手写 map[int]int
来源：http://hz.cucudq.cn/gthqzabood.html

Ruby: // 手写 Hash
来源：http://hz.ivvv.top/gtgxjeyvme.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.redwolf501.top/gteihlirjs.html

[N08] 生成全排列
来源：http://hz.sweek.top/gthxsqicze.html

Py:   itertools.permutations(arr)
来源：http://hz.vqdsnc.cn/gtbkqxvldo.html

PHP:  // 手写递归交换
来源：http://hz.ywan-chungtsiang.top/gtjadmczxc.html

JS:   // 手写回溯递归
来源：http://hz.zhaomingkeji.xyz/gtpvqgfwxb.html

TS:   // 手写回溯递归
来源：http://hz.zhengqikj.top/gtxcocvqyu.html

Java: // 手写回溯递归
来源：http://hz.jyoumei.cn/gtakbpsqlh.html

Go:   // 手写回溯递归
来源：http://hz.gzhubu.top/gtfrlufaxl.html

Ruby: arr.permutation.to_a
来源：http://hz.dianchejie.cn/gtkwfqivzy.html

C#:   // 手写回溯递归
来源：http://hz.jinghuilouyu.cn/gtjkfzcmof.html

[N09] 栈与队列
来源：http://hz.xinyue.icu/gtknanyuds.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.daxiang520.top/gtrdqakbnl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.ivvv.top/gtqduniuvb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.jinqigufen.top/gtevgsczfi.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.dashuyun.cn/gtqtefehuf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.havefunace.top/gteqavkqig.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.nwbrower.top/gtkuoonjgl.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.xuetiantiany.cn/gtvupcjiue.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.tanke756.top/gtbrmahrgu.html

[N10] 链表节点定义
来源：http://hz.jyoumei.cn/gtjmgrceav.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yvedp.cn/gtpubmcxpp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.ydzc1.top/gtbnhboufj.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.xziqi.cn/gtgnfjzijy.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.jqgufenzy.top/gtcwclsesc.html

Java: class Node { int v; Node next; }
来源：http://hz.birdmap.top/gtgflqgrma.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.cdnleiting.top/gtirkzpyeg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.wangdashe.top/gtesluoqtk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.fzhhl.top/gtiltjzrjk.html

[N11] 二叉树中序遍历
来源：http://hz.tian-w.cn/gtiqkthcog.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.dashuyun.cn/gtzfkanvac.html

PHP:  // 手写递归函数
来源：http://hz.zhongyouzk.top/gtfkuogbfh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.cqqwz.cn/gtaywigqtu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yangfankeji.com/gttsrbovax.html

Java: // 手写递归
来源：http://hz.quarkkingdee.top/gtemizjnoa.html

Go:   // 手写递归
来源：http://hz.aizwys.cn/gtgfnutndg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.jinghuilouyu.cn/gtsqclswpm.html

C#:   // 手写递归
来源：http://hz.pycfn.com/gtceqetjko.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.ppjwa.cn/gtgxljftat.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.nwbrower.top/gtrhtdnqqn.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.hywenlv.cn/gtaaeilyvm.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.sufxvd.cn/gtgpiwkene.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xinyue.icu/gtvnwornsx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.snrcjt.cn/gtnaspzipd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.havefunace.top/gtdgapmdmy.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.dianchejie.cn/gtydurmlbl.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yj20258888.top/gtdljtgibo.html

================================================================================
来源：http://hz.pycfn.com/gttegdxoqn.html

O. 并发与异步
来源：http://hz.yongpay.top/gttolzleyl.html

================================================================================
来源：http://hz.jlsjyb.cn/gtycayoxsw.html

[O01] 启动一个线程
来源：http://hz.jianghu66.top/gtzxdifjpv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.yangfankeji.com/gtkkhtkczs.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.zhongyouzk.top/gtbsxxephw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.cucudq.cn/gtgpvdpsyp.html

TS:   // 同 JS
来源：http://hz.havefunace.top/gtmhfwzbao.html

Java: new Thread(() -> f()).start()
来源：http://hz.zhixingplan.top/gtyqwgnpfn.html

Go:   go f()
来源：http://hz.vqdsnc.cn/gtiqekefhh.html

Ruby: Thread.new { f }
来源：http://hz.zhixingplan.top/gtxxcxojvs.html

C#:   Task.Run(() => F());
来源：http://hz.yj20258888.top/gthsejvmot.html

[O02] 使用线程池
来源：http://hz.wangshuangyany.cn/gtafcouxzd.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.chenjidiqi.icu/gtjzkirkcc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.ydzc1.top/gtmyftqmha.html

JS:   // worker_threads 线程池
来源：http://hz.cheryme.top/gtwickiaof.html

TS:   // worker_threads 线程池
来源：http://hz.shangyingyoupin.top/gtocsyylry.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.hnxiangtu.top/gtkhybneql.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.cqqwz.cn/gtxzpwqugx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.kuanghao11.cn/gtpmocusee.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.hywenlv.cn/gtpbholypn.html

[O03] 加锁保护共享数据
来源：http://hz.pycfn.com/gtirfpmxpk.html

Py:   with lock: shared += 1
来源：http://hz.tian-w.cn/gtrzzqcwll.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.meibo888.top/gtjunlydxe.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.hnqzz.top/gtrkvgzutd.html

TS:   // 同 JS
来源：http://hz.cheryme.top/gtwhuyzumk.html

Java: synchronized (this) { shared++; }
来源：http://hz.haohaochexian.top/gtsskstsmb.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.tian-w.cn/gtuqnwqdjj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.c1oappe.top/gtldpsckla.html

C#:   lock (gate) { shared++; }
来源：http://hz.aibaodan.cn/gtgpoufdeh.html

[O04] 定义异步函数并等待
来源：http://hz.jqgufenzy.top/gthxxnkdzi.html

Py:   async def f():⏎    await g()
来源：http://hz.hnqzz.top/gtxonnucuu.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.ydjk.org.cn/gttvfypilm.html

JS:   async function f() { await g(); }
来源：http://hz.birdmap.top/gtcykuwmvg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.cashguo.top/gtqyhemmgq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.yangfankeji.com/gtpmvsqlzm.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.ehwqpu.com/gtglsacyld.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yanxiufei.cn/gtrhidexeh.html

C#:   async Task F() { await G(); }
来源：http://hz.jinqigfzy.top/gtjulfhphn.html

[O05] 并发执行并等待全部完成
来源：http://hz.sysykeji.top/gtanhrjzex.html

Py:   asyncio.gather(*tasks)
来源：http://hz.zhengqikj.top/gtbpfnfcos.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.dianchejie.cn/gtdzvvqyum.html

JS:   await Promise.all(tasks)
来源：http://hz.ydzc1.top/gtfzyreeow.html

TS:   await Promise.all(tasks)
来源：http://hz.bjfxy.top/gtdoawwiot.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.zycfv.cn/gtxzhmzzjg.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.xuanzx.com/gttrxykjib.html

Ruby: threads.map(&:join)
来源：http://hz.chenzaomai.com/gttpjziobx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.ydjk.org.cn/gtdvxihzjl.html

[O06] 使用进程池
来源：http://hz.0kj1m.cn/gtqrnosxxw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.daxiang520.top/gtjkcgflxu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.shuidangran.top/gtbgjzntvb.html

JS:   // child_process / cluster 模块
来源：http://hz.gogol.net.cn/gtolaczwsl.html

TS:   // child_process / cluster 模块
来源：http://hz.zhaomingkeji.xyz/gtbwfdapab.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.cheryme.top/gtjrgkuvwe.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.yj20258888.top/gtkadwmtmy.html

Ruby: // fork 块
来源：http://hz.kuanghao11.cn/gtnupkitlw.html

C#:   Parallel.For
来源：http://hz.aibaodan.cn/gtoxygwdhj.html

================================================================================
来源：http://hz.svipenyu.cn/gtfbsfokxo.html

P. 常用工具函数
来源：http://hz.xziqi.cn/gtxoylsqkx.html

================================================================================
来源：http://hz.chenlongwang.top/gtxwdwnplx.html

[P01] 生成 UUID
来源：http://hz.snrcjt.cn/gtnpeqiday.html

Py:   str(uuid.uuid4())
来源：http://hz.zhiwuduotai.top/gtecqonsij.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.kuanghao11.cn/gtwgfcoxxm.html

JS:   crypto.randomUUID()
来源：http://hz.jqgufenzy.top/gtcvjkgzfi.html

TS:   crypto.randomUUID()
来源：http://hz.yj20258.top/gtitmgphnc.html

Java: UUID.randomUUID().toString()
来源：http://hz.ydzc1.top/gtqpuzrelc.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yongpay.top/gtknlsjwxr.html

Ruby: SecureRandom.uuid
来源：http://hz.jinyuanbaomall.cn/gtaiaseomp.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.chenzaomai.com/gtadzrstir.html

[P02] MD5 / SHA256 摘要
来源：http://hz.shanyushiyangtech.top/gtvhnnvvia.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.hywenlv.cn/gtlpwmdcxs.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.xuanzx.com/gtjchcbzoo.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.zdqjudy.top/gtoxebpmnl.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.birdmap.top/gtcspbjslw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.cqqwz.cn/gtzqomoepj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.yangfankeji.com/gtueehqlsa.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.xinyue.icu/gtsiqqryhn.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.daria6918.cn/gtcvqolrnw.html

[P03] 生成短随机字符串
来源：http://hz.hammf.cn/gtnmutvysm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.ydjk.org.cn/gtqxnozqyw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.smart0.xyz/gtqtqrmfgk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.redwolf501.top/gtmatkemaz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.52xcode.cn/gtngnwnbwj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.ydzc1.top/gthmzsmxwa.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.0kj1m.cn/gtvpdbqnjj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.9152youxi.cn/gtqlvqsrow.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.cdnleiting.top/gtiyfnnnyv.html

[P04] 求长度
来源：http://hz.snrcjt.cn/gtroetvyfs.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.gaohongyu789.top/gtlgvpoqbl.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.daxiang520.top/gtkpvfrrad.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.nanxuanxn.top/gtrovqfrmb.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yueranfly.top/gtanjaacvv.html

Java: list.size();  map.size();  s.length()
来源：http://hz.c1oappe.top/gtdzpbypjs.html

Go:   len(arr);  len(m)
来源：http://hz.redwolf501.top/gtbmpoccve.html

Ruby: x.length;  x.size
来源：http://hz.sxryk.cn/gtzxrnxsod.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.ivvv.top/gtsatpvjlx.html

[P05] 判断两个对象内容是否相等
来源：http://hz.yj20258888.top/gtvsvghqan.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.hnxiangtu.top/gtqyctvayg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.ydzc1.top/gtzalsftfe.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.tianlin.xyz/gtzsddptwm.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jqgufenzy.top/gtbveddmpf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.smart0.xyz/gtijqjswmg.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.ppjwa.cn/gtofthmlbg.html

Ruby: a == b
来源：http://hz.ivvv.top/gtyrreuoca.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.ehwqpu.com/gtbodzritp.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.cheryme.top/gtymehoqxf.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.sufxvd.cn/gtnqfmfcwj.html

PHP:  if (empty($x)) {}
来源：http://hz.kuanghao11.cn/gtztgyilbn.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jinqigufen.top/gtrniawipp.html

TS:   if (x == null) {}
来源：http://hz.hywenlv.cn/gtxrpyzzzs.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.hfpthk.cn/gtqodsbmji.html

Go:   if x == nil {}
来源：http://hz.quarkkingdee.top/gtmtttfazu.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.yuanzhike.top/gtwfxkoupd.html

C#:   if (x is null) {}
来源：http://hz.hysaishi.cn/gtajuoqttz.html

[P07] 防抖与节流
来源：http://hz.jinyuanbaomall.cn/gtqwggjweh.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.bjfxy.top/gtqtogquso.html

PHP:  // 手写时间戳比较
来源：http://hz.316326.xyz/gtesjxnfog.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.wangshuangyany.cn/gtxirbdqek.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.sxryk.cn/gtwfnnqavf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.jiagoushi.top/gttrwzfimc.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.sxryk.cn/gtdihxebax.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.haohaochexian.top/gtykusmspu.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.tanke756.top/gtnadxgnqh.html

[P08] 处理浮点精度问题
来源：http://hz.aizwys.cn/gtbnvxponw.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.daria6918.cn/gtggtwdsic.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.tianlin.xyz/gtxrthqljn.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.zhiwuduotai.top/gtbgtncnhe.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.guannengcc.top/gtkwtlawkh.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.pengpengdd.cyou/gtduvkpjsv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.c1oappe.top/gttprzmnsp.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.sufxvd.cn/gtyvjegppd.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.aizwys.cn/gtyolaxiuc.html

================================================================================
来源：http://hz.svipenyu.cn/gtirkhumoj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.jlsjyb.cn/gtgwsfbrih.html

================================================================================
来源：http://hz.sysykeji.top/gtpivvbojm.html

[Q01] 创建表
来源：http://hz.cashguo.top/gtubhviprs.html

CREATE TABLE users (
来源：http://hz.yj202588.top/gthxfnsetp.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hnxiangtu.top/gteubjghel.html

name VARCHAR(50) NOT NULL,
来源：http://hz.aizwys.cn/gtxnhkjnap.html

email VARCHAR(100) UNIQUE,
来源：http://hz.hfpthk.cn/gtttzwqoew.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.sufxvd.cn/gtgyptglln.html

);
来源：http://hz.wangshuangyany.cn/gtlwuvarxu.html

[Q02] 创建带外键的表
来源：http://hz.yj20258888.top/gtqqojgjwy.html

CREATE TABLE orders (
来源：http://hz.meibo888.top/gtgsapsfpq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jqgufenzy.top/gtliqftvrn.html

user_id INT NOT NULL,
来源：http://hz.yvedp.cn/gtawfffkqu.html

amount DECIMAL(10, 2),
来源：http://hz.snrcjt.cn/gtgakchuzs.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.yuanzhike.top/gtxbatjiyb.html

);
来源：http://hz.haohaochexian.top/gtgaizudph.html

[Q03] 增加列
来源：http://hz.meibo888.top/gtzkavasxo.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.52xcode.cn/gtivwfmbfn.html

[Q04] 修改列类型
来源：http://hz.hnxiangtu.top/gtsllvgjpu.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.fzhhl.top/gtchmqvmwj.html

[Q05] 重命名列
来源：http://hz.chenlongwang.top/gtrsneijzq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.tianlin.xyz/gthdqxmnhf.html

[Q06] 删除列
来源：http://hz.smart0.xyz/gtvfkgwwsu.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.cqqwz.cn/gtvozfrowv.html

[Q07] 删除表
来源：http://hz.yuxming.cn/gtiervpqob.html

DROP TABLE IF EXISTS orders;
来源：http://hz.jiagoushi.top/gttxdwgwkl.html

[Q08] 创建普通索引
来源：http://hz.cashguo.top/gtjpcuzwdd.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.shangyingyoupin.top/gtqpsyfper.html

[Q09] 创建唯一索引
来源：http://hz.jinqigufen.top/gtmptjoaci.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.316326.xyz/gtszbospqn.html

[Q10] 插入单行
来源：http://hz.zhaomingkeji.xyz/gtladpunbl.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.xuetiantiany.cn/gtunthbedc.html

[Q11] 一次插入多行
来源：http://hz.tian-w.cn/gtoihofkzk.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.316326.xyz/gtqyrzffai.html

[Q12] 插入后取自增 ID
来源：http://hz.sufxvd.cn/gtilmckohg.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.guowangkeji.top/gtipeazlyz.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.aizwys.cn/gtutybweya.html

[Q13] 忽略重复插入
来源：http://hz.yongpay.top/gttnufitci.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.nanxinkj.top/gtjiieykpu.html

[Q14] 存在则更新（upsert）
来源：http://hz.hnxiangtu.top/gtoiztwiom.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.svipenyu.cn/gtvvrwfqxd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.hongshengwenyu.top/gtcchrerkk.html

[Q15] 查询全部
来源：http://hz.yj202588.top/gtcunlzaia.html

SELECT * FROM users;
来源：http://hz.yj20258.top/gtnqzepncq.html

[Q16] 查询指定列
来源：http://hz.yongpay.top/gtnuqnwyeg.html

SELECT id, name FROM users;
来源：http://hz.yvedp.cn/gtntinrzbn.html

[Q17] 条件查询
来源：http://hz.nanxinkj.top/gtrtvredjv.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.aibaodan.cn/gtjjsdfcqk.html

[Q18] 模糊匹配
来源：http://hz.zhiwuduotai.top/gtmdoeedcd.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.jinqigufen.top/gtczjywbxw.html

[Q19] 范围查询
来源：http://hz.yuxming.cn/gtrxfmrlio.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.wangshuangyany.cn/gtbcyxvcly.html

[Q20] IN 列表
来源：http://hz.yj202588.top/gtwygawocv.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.ywan-chungtsiang.top/gtderwbcfs.html

[Q21] 空值判断
来源：http://hz.zhongyouzk.top/gtzgwuxnvn.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.dianchejie.cn/gteubfvrnb.html

[Q22] 排序
来源：http://hz.shuidangran.top/gtggjiqqnp.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.yueranfly.top/gteeoeojgd.html

[Q23] 分页
来源：http://hz.pycfn.com/gtewnjzpma.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.jinghuilouyu.cn/gtxykptpdy.html

[Q24] 去重
来源：http://hz.cucudq.cn/gttlqsknhw.html

SELECT DISTINCT city FROM users;
来源：http://hz.redwolf501.top/gtmrnvhpjk.html

[Q25] 只取前 N 条
来源：http://hz.kuanghao11.cn/gtseihyybz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.nanxinkj.top/gtdpcxqbed.html

[Q26] 计数
来源：http://hz.pycfn.com/gththzxbxn.html

SELECT COUNT(*) FROM users;
来源：http://hz.c1oappe.top/gtzqvzezix.html

[Q27] 条件计数
来源：http://hz.shzxlz.cn/gtndckgycp.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.dashuyun.cn/gttnipnrlg.html

[Q28] 求和与平均
来源：http://hz.bjfxy.top/gtkugvcxya.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.jinqigfzy.top/gtnhcpxovx.html

[Q29] 最大最小值
来源：http://hz.jianghu66.top/gtdbkpyedc.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.guowangkeji.top/gtbozrnqax.html

[Q30] 分组统计
来源：http://hz.ydzc1.top/gthpajzsjp.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.havefunace.top/gtbsgytqtd.html

[Q31] 分组后过滤
来源：http://hz.sufxvd.cn/gttqkqxckm.html


<!-- 参考信息 -->