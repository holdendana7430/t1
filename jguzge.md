代发 wailian999

Ruby: arr.sort
来源：http://hz.daria6918.cn/gttrsbgjpa.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.chenjidiqi.icu/gtegltjugu.html

[N03] 快速排序（分治示例）
来源：http://hz.yvedp.cn/gtljaitare.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.cashguo.top/gtrhvuwbdq.html

PHP:  // 递归实现，或用 usort
来源：http://hz.yueranfly.top/gtzouuxhmh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jqgufenzy.top/gtswlsrdpa.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.tian-w.cn/gtemkygtea.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.daxiang520.top/gtvsyelrbt.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.ehwqpu.com/gtojuhzdbp.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yongpay.top/gtcnwlnjtm.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.hnqzz.top/gtyulqxpac.html

[N04] 斐波那契数列
来源：http://hz.birdmap.top/gtgfyhdncj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jinyuanbaomall.cn/gthcsgxmef.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.shanyushiyangtech.top/gtipeikbdc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yj20258.top/gtrwclsqsk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.fzhhl.top/gtcnlbvlwd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.sysykeji.top/gtfepqpkab.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yonumen.top/gtvibgwmly.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.xylfe.cn/gtuvjiijms.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.ywan-chungtsiang.top/gtjevgkewd.html

[N05] 最大公约数
来源：http://hz.ydzc1.top/gtnzavvhki.html

Py:   math.gcd(a, b)
来源：http://hz.shangyingyoupin.top/gteuxprfhv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.feifeiyinyue.top/gttqvtarax.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.redwolf501.top/gtbcwkbndw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ywan-chungtsiang.top/gtlfmckzwb.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.jinqigufen.top/gtngnkdtup.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.shzxlz.cn/gtigdnpxwo.html

Ruby: a.gcd(b)
来源：http://hz.dashuyun.cn/gtdmykgfzg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.fengsongda.top/gtinxbduho.html

[N06] 判断回文字符串
来源：http://hz.iojbl.cn/gtdpnqkwja.html

Py:   s == s[::-1]
来源：http://hz.guannengcc.top/gtwiybjtsy.html

PHP:  $s === strrev($s);
来源：http://hz.zhiwuduotai.top/gtrtqoqtpc.html

JS:   s === [...s].reverse().join("")
来源：http://hz.zhiwuduotai.top/gtnivgdras.html

TS:   s === [...s].reverse().join("")
来源：http://hz.ivvv.top/gtdtovxqlx.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jlsjyb.cn/gtmpfbtdzh.html

Go:   // 双指针从两端比较
来源：http://hz.yueranfly.top/gtqeadkvri.html

Ruby: s == s.reverse
来源：http://hz.chenjidiqi.icu/gtlldsfsac.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.hammf.cn/gtqtbtazht.html

[N07] 两数之和（返回下标）
来源：http://hz.pengpengdd.cyou/gtllpfdpgn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.jiagoushi.top/gtoqpxfpkv.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.ivvv.top/gtnqcidwql.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.gaohongyu789.top/gtygwradoe.html

TS:   // 手写 Map<string, number>
来源：http://hz.cheryme.top/gtlyjlwnvs.html

Java: // 手写 HashMap
来源：http://hz.hywenlv.cn/gtdycpydob.html

Go:   // 手写 map[int]int
来源：http://hz.zycfv.cn/gtfidjqevz.html

Ruby: // 手写 Hash
来源：http://hz.dianchejie.cn/gtjftsbtcg.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.tanke756.top/gtcsrdtsif.html

[N08] 生成全排列
来源：http://hz.hnxiangtu.top/gtpqovtvae.html

Py:   itertools.permutations(arr)
来源：http://hz.jlsjyb.cn/gtifuqbzpu.html

PHP:  // 手写递归交换
来源：http://hz.sxryk.cn/gtqqeagyuo.html

JS:   // 手写回溯递归
来源：http://hz.hammf.cn/gtzjthgbmq.html

TS:   // 手写回溯递归
来源：http://hz.cucudq.cn/gtyrrphbzy.html

Java: // 手写回溯递归
来源：http://hz.zhiwuduotai.top/gtetzgowcy.html

Go:   // 手写回溯递归
来源：http://hz.yangfankeji.com/gtsaxgixtj.html

Ruby: arr.permutation.to_a
来源：http://hz.hongshengwenyu.top/gtlidqwyia.html

C#:   // 手写回溯递归
来源：http://hz.zhixingplan.top/gtxnrekrdj.html

[N09] 栈与队列
来源：http://hz.sxryk.cn/gtxvohemrz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yj20258.top/gttvjtwyut.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.feifeiyinyue.top/gtgxauibrs.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.gogol.net.cn/gtfhtqyyox.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.ppjwa.cn/gtsjqrxhvb.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.pycfn.com/gtgvibfrnu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.zhijiandao.cn/gtvuwsjinq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.xuetiantiany.cn/gtxqcoutgd.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.gotoacloud.top/gtfghduvde.html

[N10] 链表节点定义
来源：http://hz.zhiwuduotai.top/gtxydbersq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.zhijiandao.cn/gtcwkjsdps.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.xinyue.icu/gtnxjmzlag.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.sufxvd.cn/gtlwifkylf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.cqqwz.cn/gttnhgbglf.html

Java: class Node { int v; Node next; }
来源：http://hz.pengpengdd.cyou/gtizltnbea.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.shuidangran.top/gtlxeslnen.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.mhx1999.top/gthxwkbrhc.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.cheryme.top/gtvnckgefx.html

[N11] 二叉树中序遍历
来源：http://hz.9152youxi.cn/gtwwwmubly.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.zhongyouzk.top/gtzcbbvabb.html

PHP:  // 手写递归函数
来源：http://hz.andypj.xyz/gtqayszcgj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jqgfzy.top/gtjnighncx.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.iojbl.cn/gtgrhsymyc.html

Java: // 手写递归
来源：http://hz.vqdsnc.cn/gtrmfztcej.html

Go:   // 手写递归
来源：http://hz.9152youxi.cn/gtqsbwqcdt.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.xylfe.cn/gtjyqmcyuv.html

C#:   // 手写递归
来源：http://hz.0kj1m.cn/gtyzbnujzr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.316326.xyz/gtgxqsymmw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.fengsongda.top/gtdcwuppkz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.kuanghao11.cn/gtlunhfmle.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jlsjyb.cn/gtogsljhyy.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.shanyushiyangkeji.top/gtrjdyvtfs.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.gaohongyu789.top/gtxekcepwp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.wangdashe.top/gtohiqketg.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.daxiang520.top/gtkxomdzcu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.bjfxy.top/gtlfyerwww.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtrmavgsjm.html

O. 并发与异步
来源：http://hz.daxiang520.top/gtzpxgglyl.html

================================================================================
来源：http://hz.ppjwa.cn/gtujznzvqj.html

[O01] 启动一个线程
来源：http://hz.gogol.net.cn/gtzczbtcza.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.feifeiyinyue.top/gtkrlwkrsi.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.jinghuilouyu.cn/gtvjwwhubx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.wangdashe.top/gtatochite.html

TS:   // 同 JS
来源：http://hz.zhiwuduotai.top/gtveejdxfa.html

Java: new Thread(() -> f()).start()
来源：http://hz.mhx1999.top/gttwtcwvvb.html

Go:   go f()
来源：http://hz.jinghuilouyu.cn/gtwguglnyd.html

Ruby: Thread.new { f }
来源：http://hz.gaohongyu789.top/gtcnbxandq.html

C#:   Task.Run(() => F());
来源：http://hz.dashuyun.cn/gtboluecsc.html

[O02] 使用线程池
来源：http://hz.havefunace.top/gttmwraugc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yuxming.cn/gtvdntceve.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.gotoacloud.top/gtyzmmvxop.html

JS:   // worker_threads 线程池
来源：http://hz.kuanghao11.cn/gtbgmgmski.html

TS:   // worker_threads 线程池
来源：http://hz.chenlongwang.top/gtjevsgexa.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.dianchejie.cn/gtammdphdl.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yanxiufei.cn/gtwtcbqmnw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.jinghuilouyu.cn/gtcjqragve.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.nanxuanxn.top/gtpiyzkybh.html

[O03] 加锁保护共享数据
来源：http://hz.vqdsnc.cn/gtizpyipar.html

Py:   with lock: shared += 1
来源：http://hz.ywan-chungtsiang.top/gtgwszllxj.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.xingfuxueyuan.xyz/gtsnbrquez.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.quarkkingdee.top/gttsmtonqb.html

TS:   // 同 JS
来源：http://hz.cucudq.cn/gturuyhnhm.html

Java: synchronized (this) { shared++; }
来源：http://hz.jqgufenzy.top/gtrvryhpyk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.pengpengdd.cyou/gtjxyekxgy.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.xuanzx.com/gtvyobbkrb.html

C#:   lock (gate) { shared++; }
来源：http://hz.fzhhl.top/gtaluvafjc.html

[O04] 定义异步函数并等待
来源：http://hz.ywan-chungtsiang.top/gtacshmirw.html

Py:   async def f():⏎    await g()
来源：http://hz.ydjk.org.cn/gtlwxkrdcx.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jqgufenzy.top/gtxguiaskw.html

JS:   async function f() { await g(); }
来源：http://hz.wangshuangyany.cn/gtpjxigtky.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.xziqi.cn/gtpccaerpz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.dianchejie.cn/gtskjizuxo.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.pengpengdd.cyou/gtmvwhohbf.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.zycfv.cn/gthfdrbanw.html

C#:   async Task F() { await G(); }
来源：http://hz.vqdsnc.cn/gtkeadhmfr.html

[O05] 并发执行并等待全部完成
来源：http://hz.hongshengwenyu.top/gtpgdvyzwn.html

Py:   asyncio.gather(*tasks)
来源：http://hz.quarkkingdee.top/gtwvwpdwcs.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.316326.xyz/gtncywspmn.html

JS:   await Promise.all(tasks)
来源：http://hz.cashguo.top/gtindjmwkr.html

TS:   await Promise.all(tasks)
来源：http://hz.kuanghao11.cn/gtegxrhhtq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.cucudq.cn/gtskieaggo.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.daria6918.cn/gtusugiwxf.html

Ruby: threads.map(&:join)
来源：http://hz.9152youxi.cn/gtqtelngum.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yuanzhike.top/gtxvfmuiss.html

[O06] 使用进程池
来源：http://hz.gaohongyu789.top/gtelmxzlkb.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.yj20258888.top/gtvskgoodr.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.cqqwz.cn/gtnzeungfr.html

JS:   // child_process / cluster 模块
来源：http://hz.nwbrower.top/gtubtxlbrv.html

TS:   // child_process / cluster 模块
来源：http://hz.cheryme.top/gtbpqhrkrs.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.c1oappe.top/gtvfkoadrk.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.jqgufenzy.top/gtymsskpgr.html

Ruby: // fork 块
来源：http://hz.gaohongyu789.top/gtttyupshy.html

C#:   Parallel.For
来源：http://hz.cdnleiting.top/gtxxrcpuvk.html

================================================================================
来源：http://hz.nanxinkj.top/gtsqbrvxhu.html

P. 常用工具函数
来源：http://hz.guowangkeji.top/gtfuieynyk.html

================================================================================
来源：http://hz.shuidangran.top/gtxfmvazfu.html

[P01] 生成 UUID
来源：http://hz.sufxvd.cn/gtebcfsnnq.html

Py:   str(uuid.uuid4())
来源：http://hz.zhiwuduotai.top/gtauvsjpup.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.shangyingyoupin.top/gthdgiyrfh.html

JS:   crypto.randomUUID()
来源：http://hz.wangdashe.top/gtuwngznja.html

TS:   crypto.randomUUID()
来源：http://hz.yanxiufei.cn/gtcrkvhnxc.html

Java: UUID.randomUUID().toString()
来源：http://hz.pengpengdd.cyou/gtmqtiagxk.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yueranfly.top/gtzzdnnmxu.html

Ruby: SecureRandom.uuid
来源：http://hz.zhaomingkeji.xyz/gtbwyiihtx.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.gaohongyu789.top/gttjrozpdr.html

[P02] MD5 / SHA256 摘要
来源：http://hz.shuidangran.top/gtterbjlkf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.haohaochexian.top/gtcvxcpcqh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.yvedp.cn/gtyzlimknk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yanxiufei.cn/gtwqcsncxk.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.9152youxi.cn/gtqxngkjnt.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.shangyingyoupin.top/gtdusxofxi.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.aibaodan.cn/gtngsvooom.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.gaohongyu789.top/gttfbjcahl.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yvedp.cn/gttudbmezs.html

[P03] 生成短随机字符串
来源：http://hz.cdnleiting.top/gthaiwavet.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.sxryk.cn/gtcjnlbshk.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.jinyuanbaomall.cn/gtklvpapdr.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yvedp.cn/gtkhsujmiq.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hywenlv.cn/gtesysslvc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jiagoushi.top/gtvfsoirfi.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yuxming.cn/gttjxfkuiz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.sufxvd.cn/gtgweyqunk.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.yanxiufei.cn/gtbgfkymfj.html

[P04] 求长度
来源：http://hz.zycfv.cn/gttqdcxokx.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.xylfe.cn/gteyyfdnwg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xylfe.cn/gtnodqjcmf.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jqgufenzy.top/gtmurkzejp.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xylfe.cn/gtucuqpxbl.html

Java: list.size();  map.size();  s.length()
来源：http://hz.shuidangran.top/gtracwckex.html

Go:   len(arr);  len(m)
来源：http://hz.zhengqikj.top/gtkweeqhuh.html

Ruby: x.length;  x.size
来源：http://hz.sufxvd.cn/gtocfbtxsp.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.sxryk.cn/gtpfmoxsce.html

[P05] 判断两个对象内容是否相等
来源：http://hz.guannengcc.top/gtdutraypn.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.tian-w.cn/gtwfegcaqm.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.yueranfly.top/gtxcmomdia.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.hnqzz.top/gtgwoqkjro.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.meibo888.top/gtarezjgye.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.hammf.cn/gtrzjulxvs.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.aizwys.cn/gttxqwqppl.html

Ruby: a == b
来源：http://hz.pengpengdd.cyou/gtctajlzpa.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.chenjidiqi.icu/gtdbiufons.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.nanxinkj.top/gteznthlwc.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.shangyingyoupin.top/gtltrioskr.html

PHP:  if (empty($x)) {}
来源：http://hz.yj202588.top/gtytwtmvoq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.yj202588.top/gtkzbhomgm.html

TS:   if (x == null) {}
来源：http://hz.fzhhl.top/gtayuqacwy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.jqgufenzy.top/gtfbbeawyj.html

Go:   if x == nil {}
来源：http://hz.wangdashe.top/gtheaqottr.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.tian-w.cn/gtvkbsjokf.html

C#:   if (x is null) {}
来源：http://hz.zhoulong.xyz/gtnxbfbrhc.html

[P07] 防抖与节流
来源：http://hz.jqgfzy.top/gtgowoydfy.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.gaohongyu789.top/gtjphvbsxq.html

PHP:  // 手写时间戳比较
来源：http://hz.tianlin.xyz/gtclifqtqn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.sysykeji.top/gtfbcspntp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.quarkkingdee.top/gtsgwqmzny.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.quarkkingdee.top/gtdvwuepmp.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.ydjk.org.cn/gtmfjahkeo.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.guowangkeji.top/gtbdfahsrk.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.jlsjyb.cn/gtayevzdit.html

[P08] 处理浮点精度问题
来源：http://hz.yueranfly.top/gtwtugvxde.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.ydzc1.top/gtvcudyuge.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.hnxiangtu.top/gtcwuhwdzy.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.yangfankeji.com/gtqtywbrzb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.aizwys.cn/gtxngnotnd.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.hywenlv.cn/gtgxudqdbl.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.quarkkingdee.top/gtjhjstsad.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.bjfxy.top/gtueznyyra.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.pycfn.com/gturbinvxw.html

================================================================================
来源：http://hz.yj202588.top/gtoepzhixt.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.zhengqikj.top/gttxnnmkgl.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtvotanpec.html

[Q01] 创建表
来源：http://hz.cqqwz.cn/gtjenliiol.html

CREATE TABLE users (
来源：http://hz.gogol.net.cn/gtqedbuaxj.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.nanxuanxn.top/gtffvccrzk.html

name VARCHAR(50) NOT NULL,
来源：http://hz.hywenlv.cn/gtlrtidgcw.html

email VARCHAR(100) UNIQUE,
来源：http://hz.xylfe.cn/gtpjwtiycp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.hnqzz.top/gtucglqztl.html

);
来源：http://hz.shuidangran.top/gttlmnznwe.html

[Q02] 创建带外键的表
来源：http://hz.ydzc1.top/gtsgpnlzfj.html

CREATE TABLE orders (
来源：http://hz.yonumen.top/gtcygulmze.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jqgufenzy.top/gtxrmnxydt.html

user_id INT NOT NULL,
来源：http://hz.nwbrower.top/gtxcknifco.html

amount DECIMAL(10, 2),
来源：http://hz.hywenlv.cn/gtletdfvtq.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.xylfe.cn/gttnmpsbfe.html

);
来源：http://hz.zhaomingkeji.xyz/gtfeshmhil.html

[Q03] 增加列
来源：http://hz.svipenyu.cn/gteqnsaqau.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.hammf.cn/gtyxifvzsa.html

[Q04] 修改列类型
来源：http://hz.zhaomingkeji.xyz/gthvjcqebd.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.zycfv.cn/gtkwkxuguj.html

[Q05] 重命名列
来源：http://hz.sysykeji.top/gtivcdrdcx.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.zhengqikj.top/gtdveoavcl.html

[Q06] 删除列
来源：http://hz.svipenyu.cn/gtgpmswozn.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.chenlongwang.top/gtlelkiyhp.html

[Q07] 删除表
来源：http://hz.hywenlv.cn/gtnacyvkua.html

DROP TABLE IF EXISTS orders;
来源：http://hz.jinqigfzy.top/gtmouxynbx.html

[Q08] 创建普通索引
来源：http://hz.xuetiantiany.cn/gtsghfichh.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.wangshuangyany.cn/gtoiysconf.html

[Q09] 创建唯一索引
来源：http://hz.tianlin.xyz/gtevwwzvoi.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.cucudq.cn/gtbyejmffa.html

[Q10] 插入单行
来源：http://hz.vqdsnc.cn/gtnjnnifwr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.ivvv.top/gtlqmmrjvn.html

[Q11] 一次插入多行
来源：http://hz.jinyuanbaomall.cn/gtdzzbnmno.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yj20258888.top/gtaprlkxub.html

[Q12] 插入后取自增 ID
来源：http://hz.daria6918.cn/gtuewmigok.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yj20258.top/gtufokfsma.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.sweek.top/gtvxtrgouj.html

[Q13] 忽略重复插入
来源：http://hz.nanxinkj.top/gtqpgjcgsg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.meibo888.top/gtecmlyawm.html

[Q14] 存在则更新（upsert）
来源：http://hz.gaohongyu789.top/gtuqmantgm.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.zhaomingkeji.xyz/gtgybbossv.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.wangshuangyany.cn/gtegubuykm.html

[Q15] 查询全部
来源：http://hz.pengpengdd.cyou/gtezgbfsha.html

SELECT * FROM users;
来源：http://hz.sxryk.cn/gtjzlnnopg.html

[Q16] 查询指定列
来源：http://hz.guowangkeji.top/gtfsljoscl.html

SELECT id, name FROM users;
来源：http://hz.52xcode.cn/gtltgzlojr.html

[Q17] 条件查询
来源：http://hz.sysykeji.top/gtutaajjxa.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.meibo888.top/gthrskmiku.html

[Q18] 模糊匹配
来源：http://hz.wangshuangyany.cn/gtmatqqnvw.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.nwbrower.top/gtcrlgarmk.html

[Q19] 范围查询
来源：http://hz.yj20258888.top/gtoiezsjzx.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.svipenyu.cn/gtshvjxfqf.html

[Q20] IN 列表
来源：http://hz.quarkkingdee.top/gtfitrnlud.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.9152youxi.cn/gtoyjbfzcl.html

[Q21] 空值判断
来源：http://hz.yuxming.cn/gtpttsfnif.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.daxiang520.top/gtessqhrsd.html

[Q22] 排序
来源：http://hz.svipenyu.cn/gtdctmzwla.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.redwolf501.top/gtmzoqetej.html

[Q23] 分页
来源：http://hz.shzxlz.cn/gtmaqwhuix.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.daxiang520.top/gtbzbxgfac.html

[Q24] 去重
来源：http://hz.gaohongyu789.top/gtjbyzfvdf.html

SELECT DISTINCT city FROM users;
来源：http://hz.cheryme.top/gtiqhsodfy.html

[Q25] 只取前 N 条
来源：http://hz.ywan-chungtsiang.top/gtazklbvdb.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.bjfxy.top/gtvcmantem.html

[Q26] 计数
来源：http://hz.xziqi.cn/gtxucskskw.html

SELECT COUNT(*) FROM users;
来源：http://hz.chenlongwang.top/gtczztsimi.html

[Q27] 条件计数
来源：http://hz.pycfn.com/gtqvmftser.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yvedp.cn/gtxdzhwnlk.html

[Q28] 求和与平均
来源：http://hz.wangdashe.top/gtjqkkbxgg.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.redwolf501.top/gtmazdzzis.html

[Q29] 最大最小值
来源：http://hz.ivvv.top/gtxhiiwpgv.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.ybcxt.top/gtedyiyjji.html

[Q30] 分组统计
来源：http://hz.fengsongda.top/gtnawmlwky.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.aizwys.cn/gtnenmvotp.html

[Q31] 分组后过滤
来源：http://hz.pycfn.com/gtladjyjii.html


<!-- 参考信息 -->