代发 wailian999

Ruby: arr.sort
来源：http://hz.zhaomingkeji.xyz/gteziebkec.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.tian-w.cn/gtmdhwthvq.html

[N03] 快速排序（分治示例）
来源：http://hz.yanxiufei.cn/gtfgchihln.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.xuetiantiany.cn/gtmtevlouc.html

PHP:  // 递归实现，或用 usort
来源：http://hz.daria6918.cn/gtptrlutkx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xylfe.cn/gtawdeexxd.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.gzhubu.top/gttmqigadl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.tianlin.xyz/gtzsvxywyo.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jinghuilouyu.cn/gtkzjvtmwl.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.cashguo.top/gtopckvsfa.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yongpay.top/gtwrqwgyay.html

[N04] 斐波那契数列
来源：http://hz.cheryme.top/gteczsvpsd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.kuanghao11.cn/gtaqqcdpdg.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.quarkkingdee.top/gtbazqrkcp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.cashguo.top/gtpaerjswr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhaomingkeji.xyz/gtatyhhpck.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.zycfv.cn/gtkhgjfjbl.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.c1oappe.top/gtvrohauvc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.hnxiangtu.top/gtrfvvquit.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yj202588.top/gtdvmcjdcz.html

[N05] 最大公约数
来源：http://hz.sufxvd.cn/gtcjhejxku.html

Py:   math.gcd(a, b)
来源：http://hz.shuidangran.top/gtbqbnwybh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.shuidangran.top/gturklroxm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hfpthk.cn/gtakduidul.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xuetiantiany.cn/gtacgawdaw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.mhx1999.top/gtzsgidyws.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.havefunace.top/gtxxihrgqd.html

Ruby: a.gcd(b)
来源：http://hz.yvedp.cn/gtyqdrbxbh.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.ivvv.top/gtuguwfuqs.html

[N06] 判断回文字符串
来源：http://hz.yanxiufei.cn/gtruurxfsz.html

Py:   s == s[::-1]
来源：http://hz.xziqi.cn/gtzwqwzklw.html

PHP:  $s === strrev($s);
来源：http://hz.zhoulong.xyz/gtdforypnp.html

JS:   s === [...s].reverse().join("")
来源：http://hz.aizwys.cn/gtunbtmmyc.html

TS:   s === [...s].reverse().join("")
来源：http://hz.pengpengdd.cyou/gtsyfqxthy.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.zhengqikj.top/gtuvsypksr.html

Go:   // 双指针从两端比较
来源：http://hz.feifeiyinyue.top/gtrzsdslkk.html

Ruby: s == s.reverse
来源：http://hz.nwbrower.top/gtdsyoqsqs.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.jinqigfzy.top/gtyvzjflcb.html

[N07] 两数之和（返回下标）
来源：http://hz.hnxiangtu.top/gtxazzfpsi.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.daria6918.cn/gtmmmbluie.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.gogol.net.cn/gtfdyptvsw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.yuanzhike.top/gtycolkubb.html

TS:   // 手写 Map<string, number>
来源：http://hz.wangdashe.top/gtfnjmeldq.html

Java: // 手写 HashMap
来源：http://hz.quarkkingdee.top/gtusrqlxuh.html

Go:   // 手写 map[int]int
来源：http://hz.shangyingyoupin.top/gtxpgkprnw.html

Ruby: // 手写 Hash
来源：http://hz.hysaishi.cn/gtkgivripd.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.sufxvd.cn/gtrhkeqakv.html

[N08] 生成全排列
来源：http://hz.svipenyu.cn/gtvixjqtuu.html

Py:   itertools.permutations(arr)
来源：http://hz.tianlin.xyz/gtarcubpsk.html

PHP:  // 手写递归交换
来源：http://hz.jqgufenzy.top/gtuhukiqrb.html

JS:   // 手写回溯递归
来源：http://hz.xuetiantiany.cn/gtkzvgyufv.html

TS:   // 手写回溯递归
来源：http://hz.smart0.xyz/gtycxusjzk.html

Java: // 手写回溯递归
来源：http://hz.ywan-chungtsiang.top/gtronzdhbw.html

Go:   // 手写回溯递归
来源：http://hz.ppjwa.cn/gtoxqeukse.html

Ruby: arr.permutation.to_a
来源：http://hz.hnxiangtu.top/gtdhkbujhx.html

C#:   // 手写回溯递归
来源：http://hz.jlsjyb.cn/gtazilgcvb.html

[N09] 栈与队列
来源：http://hz.dashuyun.cn/gttaorimkk.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.guowangkeji.top/gtfrihnste.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.dashuyun.cn/gtkxhdskqc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.sweek.top/gtakibndaz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.zdqjudy.top/gtlnoqxjkf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.mhx1999.top/gtewjbvybo.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.yuxming.cn/gtohjflwbt.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yongpay.top/gtxidreitr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.bjfxy.top/gtkfexzcyg.html

[N10] 链表节点定义
来源：http://hz.chenzaomai.com/gtpstilxba.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.ivvv.top/gtxtajezjh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.iojbl.cn/gtpnipahfx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.daria6918.cn/gtscnrwfoe.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.gzhubu.top/gtjpjcmflq.html

Java: class Node { int v; Node next; }
来源：http://hz.hfpthk.cn/gtetfnyciq.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.zdqjudy.top/gtxhhxgduo.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.sxryk.cn/gtvqjlltsd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.feifeiyinyue.top/gtabfgvgtq.html

[N11] 二叉树中序遍历
来源：http://hz.ywan-chungtsiang.top/gtxsnrpags.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.zhaomingkeji.xyz/gtibyeeslt.html

PHP:  // 手写递归函数
来源：http://hz.quarkkingdee.top/gtlrfhngsk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hysaishi.cn/gtbvrnykno.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jqgufenzy.top/gtstxvegdk.html

Java: // 手写递归
来源：http://hz.birdmap.top/gtdkkztimp.html

Go:   // 手写递归
来源：http://hz.gaohongyu789.top/gtupjywvwh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.sxryk.cn/gtnlmqybqc.html

C#:   // 手写递归
来源：http://hz.cheryme.top/gtcegbjlgb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.xuanzx.com/gtlllymwtt.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.9152youxi.cn/gtyunkdami.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.gogol.net.cn/gtdixfkklz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yuxming.cn/gtavflsebz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.wangdashe.top/gtdfsvfsib.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.tian-w.cn/gtkculihyn.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.zhaomingkeji.xyz/gttyrhflem.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.nanxinkj.top/gtrvnerdqs.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.haohaochexian.top/gtczqnpjay.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtjxywmwqv.html

O. 并发与异步
来源：http://hz.havefunace.top/gtysysopcl.html

================================================================================
来源：http://hz.hammf.cn/gtopsqjmri.html

[O01] 启动一个线程
来源：http://hz.ydzc1.top/gttfauhwae.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.cqqwz.cn/gtfmnxprqo.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.haohaochexian.top/gtjkhzbjcw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.gogol.net.cn/gtdttxkyvw.html

TS:   // 同 JS
来源：http://hz.jinyuanbaomall.cn/gtcfunsvea.html

Java: new Thread(() -> f()).start()
来源：http://hz.zhengqikj.top/gtyssbteso.html

Go:   go f()
来源：http://hz.hongshengwenyu.top/gttogqwxsf.html

Ruby: Thread.new { f }
来源：http://hz.feifeiyinyue.top/gtpdysuvry.html

C#:   Task.Run(() => F());
来源：http://hz.xuanzx.com/gtqiuakkod.html

[O02] 使用线程池
来源：http://hz.nanxuanxn.top/gttlspjgwa.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.sufxvd.cn/gtfelcgexn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.hfpthk.cn/gtocyhmosg.html

JS:   // worker_threads 线程池
来源：http://hz.cdnleiting.top/gtxuwhgaeu.html

TS:   // worker_threads 线程池
来源：http://hz.zhaomingkeji.xyz/gtwemcilbw.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.aibaodan.cn/gtjyblygzj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.sufxvd.cn/gtbxgdhjrc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.jiagoushi.top/gtvzbfihws.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.sysykeji.top/gtrnokxyov.html

[O03] 加锁保护共享数据
来源：http://hz.zhijiandao.cn/gtgltklpcg.html

Py:   with lock: shared += 1
来源：http://hz.xingfuxueyuan.xyz/gtlavoztwm.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.feifeiyinyue.top/gtxaglfafq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.cqqwz.cn/gtsidvvvgu.html

TS:   // 同 JS
来源：http://hz.pycfn.com/gtkjdcpqlu.html

Java: synchronized (this) { shared++; }
来源：http://hz.ywan-chungtsiang.top/gtjbdktdgx.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.pycfn.com/gtvabdofwf.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.yj20258.top/gtpcsslaxx.html

C#:   lock (gate) { shared++; }
来源：http://hz.316326.xyz/gtqfxvhavv.html

[O04] 定义异步函数并等待
来源：http://hz.gogol.net.cn/gtxylausqc.html

Py:   async def f():⏎    await g()
来源：http://hz.guowangkeji.top/gtnxnapcfb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.yongpay.top/gtmphzbknp.html

JS:   async function f() { await g(); }
来源：http://hz.fzhhl.top/gtauidodtr.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.daria6918.cn/gtiuhfsjez.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.cashguo.top/gtdqcmniqz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.daxiang520.top/gtlaidbifq.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.vqdsnc.cn/gtztdgncvy.html

C#:   async Task F() { await G(); }
来源：http://hz.aibaodan.cn/gtserxtlgs.html

[O05] 并发执行并等待全部完成
来源：http://hz.tianlin.xyz/gtdzvwuikf.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jinyuanbaomall.cn/gtkgvahdzh.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.daxiang520.top/gthccbzdif.html

JS:   await Promise.all(tasks)
来源：http://hz.jinyuanbaomall.cn/gtqhmziwtt.html

TS:   await Promise.all(tasks)
来源：http://hz.xinyue.icu/gtdvfzktir.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.yvedp.cn/gtiucodctg.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.xuetiantiany.cn/gtfwizgbxl.html

Ruby: threads.map(&:join)
来源：http://hz.meibo888.top/gttetzdtzn.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.sysykeji.top/gtokfwfdnv.html

[O06] 使用进程池
来源：http://hz.yanxiufei.cn/gtegxelhra.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.xuetiantiany.cn/gtyfigavpo.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.yj202588.top/gtccumvjba.html

JS:   // child_process / cluster 模块
来源：http://hz.nanxinkj.top/gtficfstwb.html

TS:   // child_process / cluster 模块
来源：http://hz.yuanzhike.top/gtilblrhpm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.zhengqikj.top/gtbihsipwi.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.nanxinkj.top/gtcyfdzdif.html

Ruby: // fork 块
来源：http://hz.jqgfzy.top/gtwxthezhu.html

C#:   Parallel.For
来源：http://hz.cqqwz.cn/gtviqqpcre.html

================================================================================
来源：http://hz.0kj1m.cn/gtgmwionrw.html

P. 常用工具函数
来源：http://hz.316326.xyz/gtevfahkgc.html

================================================================================
来源：http://hz.hywenlv.cn/gtsoyaurtg.html

[P01] 生成 UUID
来源：http://hz.nwbrower.top/gtdcpeczqo.html

Py:   str(uuid.uuid4())
来源：http://hz.meibo888.top/gthbppduvl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.ppjwa.cn/gtefomzxto.html

JS:   crypto.randomUUID()
来源：http://hz.c1oappe.top/gthetvpudr.html

TS:   crypto.randomUUID()
来源：http://hz.yonumen.top/gtyywiwmpk.html

Java: UUID.randomUUID().toString()
来源：http://hz.hywenlv.cn/gtlszoovza.html

Go:   // 用 github.com/google/uuid
来源：http://hz.hysaishi.cn/gtblfbbxne.html

Ruby: SecureRandom.uuid
来源：http://hz.xuanzx.com/gtuaghytpz.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.aizwys.cn/gtwsjlmdmj.html

[P02] MD5 / SHA256 摘要
来源：http://hz.tian-w.cn/gtaprmjpmi.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.iojbl.cn/gtuyfzmdty.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.andypj.xyz/gtbycsilqw.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yuanzhike.top/gtgxawnjjn.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.iojbl.cn/gtmtaexddg.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.chenjidiqi.icu/gtdklfvzoy.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.dashuyun.cn/gtwjmqwphu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jqgufenzy.top/gtezjhobuv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.dianchejie.cn/gtphgdvnwn.html

[P03] 生成短随机字符串
来源：http://hz.kuanghao11.cn/gtexxrqvpd.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.yuxming.cn/gtgpswfinw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.redwolf501.top/gtrlspekjg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.vqdsnc.cn/gtqccfbejc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zdqjudy.top/gtqiblgtif.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.tanke756.top/gtwzciszpe.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.zhengqikj.top/gtclumahhp.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.hysaishi.cn/gtrmknexka.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.hnxiangtu.top/gtzowxvbcp.html

[P04] 求长度
来源：http://hz.xuanzx.com/gtpifaqnwn.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.hnxiangtu.top/gtlxgulnkp.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xuetiantiany.cn/gtclzqyugp.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hysaishi.cn/gtdjxlnjjs.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ivvv.top/gtqnsgkmqa.html

Java: list.size();  map.size();  s.length()
来源：http://hz.daxiang520.top/gtuhfnbhmh.html

Go:   len(arr);  len(m)
来源：http://hz.wangdashe.top/gtgpwqouqm.html

Ruby: x.length;  x.size
来源：http://hz.ywan-chungtsiang.top/gtursjdosj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.redwolf501.top/gtfgvktjfv.html

[P05] 判断两个对象内容是否相等
来源：http://hz.xuanzx.com/gtqxlggkmm.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.daxiang520.top/gtdjkurkdl.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.sweek.top/gtwbdpsbbw.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.fengsongda.top/gtuyjzmuuc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.shanyushiyangtech.top/gtsgilhexi.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.chenzaomai.com/gtimqumuhc.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.smart0.xyz/gtrnyvieid.html

Ruby: a == b
来源：http://hz.hnxiangtu.top/gtfclnfnni.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.andypj.xyz/gtlcgaslwp.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.hammf.cn/gtjpilnsum.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.hnqzz.top/gtunynxvox.html

PHP:  if (empty($x)) {}
来源：http://hz.0kj1m.cn/gtsfzpiofc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.zhoulong.xyz/gtyfkhleic.html

TS:   if (x == null) {}
来源：http://hz.gogol.net.cn/gtropgjlhw.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.zycfv.cn/gtrqlgihcm.html

Go:   if x == nil {}
来源：http://hz.tanke756.top/gtnodcfpyj.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.shangyingyoupin.top/gtjcwtmxcg.html

C#:   if (x is null) {}
来源：http://hz.yanxiufei.cn/gtkkiiunui.html

[P07] 防抖与节流
来源：http://hz.gotoacloud.top/gtkuflhhgn.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jinqigufen.top/gtsmfglchc.html

PHP:  // 手写时间戳比较
来源：http://hz.sufxvd.cn/gtszyaabzh.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.pengpengdd.cyou/gtexhjzxvk.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ivvv.top/gtcxweaoip.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.tian-w.cn/gtyikjnpsx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.yonumen.top/gtystrtobh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.cdnleiting.top/gtylhiftge.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.yongpay.top/gtewtfmyur.html

[P08] 处理浮点精度问题
来源：http://hz.zhengqikj.top/gtmoknlpxq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.hysaishi.cn/gtgypxwljx.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.ppjwa.cn/gtaxmpcazc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.feifeiyinyue.top/gtunwufmyf.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.xinyue.icu/gterdbpjum.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.ppjwa.cn/gtmnyebjsk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.yonumen.top/gtqkiryqij.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.hnqzz.top/gtlryhanwc.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.hfpthk.cn/gtsoyizbzz.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtdoeekuur.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.jqgufenzy.top/gtrcvfmcoj.html

================================================================================
来源：http://hz.nanxinkj.top/gtirfrppqt.html

[Q01] 创建表
来源：http://hz.chenzaomai.com/gtcvkllzbo.html

CREATE TABLE users (
来源：http://hz.gotoacloud.top/gtonjhaoda.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.havefunace.top/gtkdnhfikb.html

name VARCHAR(50) NOT NULL,
来源：http://hz.ehwqpu.com/gtpvyxqund.html

email VARCHAR(100) UNIQUE,
来源：http://hz.bjfxy.top/gtywoitvgb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.hnxiangtu.top/gtajxegkaf.html

);
来源：http://hz.hysaishi.cn/gtmrbwayop.html

[Q02] 创建带外键的表
来源：http://hz.pengpengdd.cyou/gtfntlakog.html

CREATE TABLE orders (
来源：http://hz.ppjwa.cn/gtzlxsvdqg.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.shanyushiyangtech.top/gtzwivxcep.html

user_id INT NOT NULL,
来源：http://hz.shanyushiyangkeji.top/gtulhzfxli.html

amount DECIMAL(10, 2),
来源：http://hz.hfpthk.cn/gtqmzvrwtx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.shanyushiyangtech.top/gtauttejhj.html

);
来源：http://hz.nwbrower.top/gtrjcpuhrd.html

[Q03] 增加列
来源：http://hz.jinqigfzy.top/gtlpyylmes.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.hnqzz.top/gtejgpbtzw.html

[Q04] 修改列类型
来源：http://hz.aizwys.cn/gtqodjfkpp.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.cashguo.top/gtujuswpfx.html

[Q05] 重命名列
来源：http://hz.daxiang520.top/gtwnsyjmkp.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.jinqigufen.top/gtjddspkjk.html

[Q06] 删除列
来源：http://hz.hnqzz.top/gtyjxvqtuw.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.sufxvd.cn/gtnpnslswy.html

[Q07] 删除表
来源：http://hz.zhijiandao.cn/gtfmivcrcd.html

DROP TABLE IF EXISTS orders;
来源：http://hz.zhaomingkeji.xyz/gttdgymada.html

[Q08] 创建普通索引
来源：http://hz.sweek.top/gtmdlquuce.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.yvedp.cn/gtnykqqmqf.html

[Q09] 创建唯一索引
来源：http://hz.pengpengdd.cyou/gtlxwhkjde.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.daria6918.cn/gtsniweqfy.html

[Q10] 插入单行
来源：http://hz.ehwqpu.com/gtusrlmbod.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jinqigfzy.top/gtjfxsokdh.html

[Q11] 一次插入多行
来源：http://hz.smart0.xyz/gtklfavejf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.chenjidiqi.icu/gtwxlfgjww.html

[Q12] 插入后取自增 ID
来源：http://hz.pycfn.com/gtauraluxk.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.hywenlv.cn/gtpjrzwtzu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.xuanzx.com/gtlzvqjigi.html

[Q13] 忽略重复插入
来源：http://hz.zhongyouzk.top/gtowmbenvg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jinqigfzy.top/gtzsjymsmu.html

[Q14] 存在则更新（upsert）
来源：http://hz.birdmap.top/gtewylxgqq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.chenlongwang.top/gtbabndvzn.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.yanxiufei.cn/gtarmiuusz.html

[Q15] 查询全部
来源：http://hz.quarkkingdee.top/gtzgimqjil.html

SELECT * FROM users;
来源：http://hz.andypj.xyz/gtekouwgqe.html

[Q16] 查询指定列
来源：http://hz.ivvv.top/gthkufnykx.html

SELECT id, name FROM users;
来源：http://hz.hysaishi.cn/gtxezcjmky.html

[Q17] 条件查询
来源：http://hz.yuanzhike.top/gttsqeaxao.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.vqdsnc.cn/gtbtbhfxuk.html

[Q18] 模糊匹配
来源：http://hz.zhoulong.xyz/gtxbjlqbkn.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yj20258888.top/gtflguvljx.html

[Q19] 范围查询
来源：http://hz.jianghu66.top/gtdpcpiyjn.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.bjfxy.top/gtwemncqox.html

[Q20] IN 列表
来源：http://hz.kuanghao11.cn/gtmwvdzznl.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.hammf.cn/gtfyxpsscu.html

[Q21] 空值判断
来源：http://hz.tanke756.top/gtpdlbnjbo.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.nwbrower.top/gtdhmangut.html

[Q22] 排序
来源：http://hz.yuanzhike.top/gtfstvjvjo.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.xylfe.cn/gtlbhdrdxw.html

[Q23] 分页
来源：http://hz.aizwys.cn/gtdlcadsim.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.ydjk.org.cn/gtvcicoyrv.html

[Q24] 去重
来源：http://hz.hammf.cn/gtpurwlxfa.html

SELECT DISTINCT city FROM users;
来源：http://hz.tian-w.cn/gtjkqoouah.html

[Q25] 只取前 N 条
来源：http://hz.hfpthk.cn/gtdidigcrm.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.tian-w.cn/gtcpjkybab.html

[Q26] 计数
来源：http://hz.xuanzx.com/gtqqahiqjj.html

SELECT COUNT(*) FROM users;
来源：http://hz.ybcxt.top/gteektpoqy.html

[Q27] 条件计数
来源：http://hz.xinyue.icu/gtyssugrec.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.zhaomingkeji.xyz/gtalticdmf.html

[Q28] 求和与平均
来源：http://hz.yanxiufei.cn/gtgdnpcyqw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.gogol.net.cn/gtdoxolgsl.html

[Q29] 最大最小值
来源：http://hz.hywenlv.cn/gtimaqeqkl.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.hongshengwenyu.top/gtlpvdsowp.html

[Q30] 分组统计
来源：http://hz.0kj1m.cn/gtzwmciycd.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.sufxvd.cn/gtyzcsqasz.html

[Q31] 分组后过滤
来源：http://hz.jinyuanbaomall.cn/gtuakffjca.html


<!-- 参考信息 -->