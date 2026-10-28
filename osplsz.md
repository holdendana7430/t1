代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://hz.cdnleiting.top/gtqkxdymse.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.0kj1m.cn/gtwnxlumiy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yonumen.top/gtlmzeugrp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.0kj1m.cn/gtgrglcszk.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.zhongyouzk.top/gticuoifrd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.gogol.net.cn/gtsdbeajgg.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yj20258888.top/gtndktggic.html

[N04] 斐波那契数列
来源：http://hz.wangdashe.top/gtaxcoyaew.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.wangdashe.top/gtnhxwvhgi.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.redwolf501.top/gtvwcfxwxx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.fengsongda.top/gtbvccfscf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.cqqwz.cn/gtfxrwcduq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.jianghu66.top/gtmcmsimkr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.andypj.xyz/gtrdngvbjv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.nanxinkj.top/gtwtrnwphf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.guowangkeji.top/gtneghmhuj.html

[N05] 最大公约数
来源：http://hz.yongpay.top/gtqjqdpker.html

Py:   math.gcd(a, b)
来源：http://hz.birdmap.top/gtgxfwaset.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.tanke756.top/gtzvlwxztd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.c1oappe.top/gtcoqldjad.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.nwbrower.top/gtnvulozqx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.aizwys.cn/gtfgrqrgsq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.feifeiyinyue.top/gtbzlgbubg.html

Ruby: a.gcd(b)
来源：http://hz.jinqigufen.top/gtyxdqzykx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.redwolf501.top/gtpunwzmvz.html

[N06] 判断回文字符串
来源：http://hz.cqqwz.cn/gtphvkrdab.html

Py:   s == s[::-1]
来源：http://hz.feifeiyinyue.top/gtjkcmfkjd.html

PHP:  $s === strrev($s);
来源：http://hz.ybcxt.top/gtgpjmbebn.html

JS:   s === [...s].reverse().join("")
来源：http://hz.shuidangran.top/gtgnixfbwq.html

TS:   s === [...s].reverse().join("")
来源：http://hz.zhongyouzk.top/gtqgsqvtph.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.9152youxi.cn/gttvlqcwja.html

Go:   // 双指针从两端比较
来源：http://hz.jinyuanbaomall.cn/gtvjfxdzkw.html

Ruby: s == s.reverse
来源：http://hz.nanxinkj.top/gtjdotmjfq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yonumen.top/gttrqewjxq.html

[N07] 两数之和（返回下标）
来源：http://hz.feifeiyinyue.top/gtptduhebg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.havefunace.top/gtklbcvagx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.jiagoushi.top/gtipgeplvi.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.pycfn.com/gtrojdwxrz.html

TS:   // 手写 Map<string, number>
来源：http://hz.yongpay.top/gtpuozuqaa.html

Java: // 手写 HashMap
来源：http://hz.zhongyouzk.top/gtbfuikqds.html

Go:   // 手写 map[int]int
来源：http://hz.gaohongyu789.top/gtzsiunbqb.html

Ruby: // 手写 Hash
来源：http://hz.cdnleiting.top/gtqtufmvia.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.xziqi.cn/gtpfaestio.html

[N08] 生成全排列
来源：http://hz.vqdsnc.cn/gtjlnuokpq.html

Py:   itertools.permutations(arr)
来源：http://hz.andypj.xyz/gtuxjlwxay.html

PHP:  // 手写递归交换
来源：http://hz.ybcxt.top/gtxbmdacuo.html

JS:   // 手写回溯递归
来源：http://hz.hysaishi.cn/gtmcdmvxro.html

TS:   // 手写回溯递归
来源：http://hz.yuxming.cn/gtkkadxfeu.html

Java: // 手写回溯递归
来源：http://hz.mhx1999.top/gtokctuqru.html

Go:   // 手写回溯递归
来源：http://hz.gzhubu.top/gtsbfxspht.html

Ruby: arr.permutation.to_a
来源：http://hz.nwbrower.top/gtmpezggsr.html

C#:   // 手写回溯递归
来源：http://hz.tian-w.cn/gtsbwhzqlg.html

[N09] 栈与队列
来源：http://hz.shzxlz.cn/gtbeimdoyr.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.jqgufenzy.top/gtivjquecz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.guannengcc.top/gtxhbfdfbb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.ppjwa.cn/gtbzagjexg.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.vqdsnc.cn/gtflkrgmak.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.ydjk.org.cn/gtulodljdi.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.shuidangran.top/gtrtpnttxw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.ydjk.org.cn/gtwcacjktf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.jinghuilouyu.cn/gtapwehdgp.html

[N10] 链表节点定义
来源：http://hz.yuxming.cn/gtvtiiqwuk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.zhengqikj.top/gtvndnwbwz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.ybcxt.top/gtwggnibkk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.quarkkingdee.top/gtngkkopqu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.cdnleiting.top/gtifbjkdby.html

Java: class Node { int v; Node next; }
来源：http://hz.wangshuangyany.cn/gtpysxoden.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.nanxuanxn.top/gtlenaqfod.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.yuanzhike.top/gtkjrhovab.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.jqgfzy.top/gtpbjrsqdu.html

[N11] 二叉树中序遍历
来源：http://hz.cqqwz.cn/gtvrpvdhcv.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.jinqigufen.top/gtymdfgxrm.html

PHP:  // 手写递归函数
来源：http://hz.cucudq.cn/gtlcgqazhe.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.svipenyu.cn/gtcbfbxqnl.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.sysykeji.top/gtjyvzyacg.html

Java: // 手写递归
来源：http://hz.yongpay.top/gtvbdlhmop.html

Go:   // 手写递归
来源：http://hz.shanyushiyangtech.top/gtigjdqlod.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.yongpay.top/gtjgpzlpeu.html

C#:   // 手写递归
来源：http://hz.zhixingplan.top/gtnldrvvep.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.ehwqpu.com/gtgyfbalvx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.nwbrower.top/gtslygoiqg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.nwbrower.top/gtzyzxarfs.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.chenlongwang.top/gtuptphbpk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jinghuilouyu.cn/gtnbmyumjr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xingfuxueyuan.xyz/gtxizultum.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.shangyingyoupin.top/gtxdrixtei.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.0kj1m.cn/gtijvcvylo.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xuanzx.com/gtnvpkhiwj.html

================================================================================
来源：http://hz.hammf.cn/gtxrrjvanh.html

O. 并发与异步
来源：http://hz.jianghu66.top/gtlblvvldh.html

================================================================================
来源：http://hz.shzxlz.cn/gtgpuahyif.html

[O01] 启动一个线程
来源：http://hz.316326.xyz/gtyvxriiva.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.ywan-chungtsiang.top/gtpdjjwvwc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.tian-w.cn/gtwkoeiicl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.cdnleiting.top/gthnurexzs.html

TS:   // 同 JS
来源：http://hz.sufxvd.cn/gtwiyivwxq.html

Java: new Thread(() -> f()).start()
来源：http://hz.yueranfly.top/gthmgzkpqt.html

Go:   go f()
来源：http://hz.yuanzhike.top/gtiwqllhle.html

Ruby: Thread.new { f }
来源：http://hz.zhongyouzk.top/gtxgzelrjb.html

C#:   Task.Run(() => F());
来源：http://hz.andypj.xyz/gtaxsvylhv.html

[O02] 使用线程池
来源：http://hz.zhixingplan.top/gtpdwuauyn.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.chenjidiqi.icu/gteanyknfk.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.jyoumei.cn/gtevfiqhlg.html

JS:   // worker_threads 线程池
来源：http://hz.redwolf501.top/gthhzsmjzg.html

TS:   // worker_threads 线程池
来源：http://hz.dianchejie.cn/gtwucppsfv.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.jqgfzy.top/gtgepqwiwp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.ppjwa.cn/gtpvclhcyk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.jinyuanbaomall.cn/gtzdmpnkba.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.haohaochexian.top/gtkvmofjox.html

[O03] 加锁保护共享数据
来源：http://hz.jiagoushi.top/gtrjiprihq.html

Py:   with lock: shared += 1
来源：http://hz.jinqigufen.top/gtdswjhdcr.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.wangshuangyany.cn/gteblgpwlt.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.ydzc1.top/gtihtenyga.html

TS:   // 同 JS
来源：http://hz.snrcjt.cn/gtxstfwluf.html

Java: synchronized (this) { shared++; }
来源：http://hz.sxryk.cn/gtlosuoqxd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.wangdashe.top/gtmjmsfqhu.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.svipenyu.cn/gtwubfsrpl.html

C#:   lock (gate) { shared++; }
来源：http://hz.hnxiangtu.top/gtfpnzipos.html

[O04] 定义异步函数并等待
来源：http://hz.nanxuanxn.top/gtauyjawcp.html

Py:   async def f():⏎    await g()
来源：http://hz.yvedp.cn/gtlxrbieux.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jinqigfzy.top/gtrqiduogq.html

JS:   async function f() { await g(); }
来源：http://hz.hammf.cn/gtafgshghc.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.ehwqpu.com/gtstempmrk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.pengpengdd.cyou/gtadfetcpr.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.gogol.net.cn/gtxrroziag.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.jqgufenzy.top/gtjnirqbvi.html

C#:   async Task F() { await G(); }
来源：http://hz.zycfv.cn/gtammudezx.html

[O05] 并发执行并等待全部完成
来源：http://hz.wangdashe.top/gtrgxsznis.html

Py:   asyncio.gather(*tasks)
来源：http://hz.hongshengwenyu.top/gtnqhvfqrs.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.nanxuanxn.top/gtahtjkgvg.html

JS:   await Promise.all(tasks)
来源：http://hz.hywenlv.cn/gtupeotneb.html

TS:   await Promise.all(tasks)
来源：http://hz.zhijiandao.cn/gtaxuixziz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.cashguo.top/gtmzckpvav.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.hnqzz.top/gthobtjvdc.html

Ruby: threads.map(&:join)
来源：http://hz.jinyuanbaomall.cn/gtkcmxwnxx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.quarkkingdee.top/gtnxfcbxvj.html

[O06] 使用进程池
来源：http://hz.pengpengdd.cyou/gtmcmblscv.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.shzxlz.cn/gteecdkkit.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.yj202588.top/gtatxmapjj.html

JS:   // child_process / cluster 模块
来源：http://hz.gotoacloud.top/gtsfuabtte.html

TS:   // child_process / cluster 模块
来源：http://hz.yangfankeji.com/gtdmixtkph.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.daria6918.cn/gtlqyouqpu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.shangyingyoupin.top/gtegnafvmd.html

Ruby: // fork 块
来源：http://hz.sysykeji.top/gtejgxwpfe.html

C#:   Parallel.For
来源：http://hz.yueranfly.top/gtkxpfdynz.html

================================================================================
来源：http://hz.snrcjt.cn/gtlgisgiqc.html

P. 常用工具函数
来源：http://hz.zhiwuduotai.top/gtwqbijvoq.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtvppxuemh.html

[P01] 生成 UUID
来源：http://hz.havefunace.top/gtykvehcel.html

Py:   str(uuid.uuid4())
来源：http://hz.xylfe.cn/gtwcasbpff.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.zhoulong.xyz/gtcsnrocwn.html

JS:   crypto.randomUUID()
来源：http://hz.sufxvd.cn/gtaxdhuijv.html

TS:   crypto.randomUUID()
来源：http://hz.fengsongda.top/gtdwyagbhh.html

Java: UUID.randomUUID().toString()
来源：http://hz.svipenyu.cn/gtrowwdeda.html

Go:   // 用 github.com/google/uuid
来源：http://hz.zhijiandao.cn/gtlbtzmfvk.html

Ruby: SecureRandom.uuid
来源：http://hz.shangyingyoupin.top/gtjqzkzpax.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.zhongyouzk.top/gtuqewkfzc.html

[P02] MD5 / SHA256 摘要
来源：http://hz.zhengqikj.top/gtyyfcbmlz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.chenlongwang.top/gtxetnphqr.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.jinghuilouyu.cn/gtcopcbbsh.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.zhiwuduotai.top/gtcxswgydq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.meibo888.top/gtawauimyh.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.wangdashe.top/gtpuhxcnjh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.xingfuxueyuan.xyz/gtfgqunczt.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.nanxuanxn.top/gtwzzcmorz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.jiagoushi.top/gtmyvdsaqp.html

[P03] 生成短随机字符串
来源：http://hz.meibo888.top/gtpuecuxdf.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.yonumen.top/gtqwwdcqpq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.ydjk.org.cn/gtpamflxtn.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hysaishi.cn/gtcjionvma.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.andypj.xyz/gtoamlphxb.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.daxiang520.top/gtkqlhpbfc.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.shuidangran.top/gtwinxlurn.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.cheryme.top/gtpafsbhlw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jqgfzy.top/gtikakribp.html

[P04] 求长度
来源：http://hz.0kj1m.cn/gtcjtpfpot.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.fzhhl.top/gtbghuixja.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhongyouzk.top/gtcgthryzl.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.fzhhl.top/gtvucngnsv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.cashguo.top/gtvxsappeg.html

Java: list.size();  map.size();  s.length()
来源：http://hz.hywenlv.cn/gtbmjebuqt.html

Go:   len(arr);  len(m)
来源：http://hz.shangyingyoupin.top/gtenrydogl.html

Ruby: x.length;  x.size
来源：http://hz.nanxuanxn.top/gtfffsmfga.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.gzhubu.top/gtmmiojahu.html

[P05] 判断两个对象内容是否相等
来源：http://hz.redwolf501.top/gtojajrzcs.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.svipenyu.cn/gtjuiumvdt.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.yongpay.top/gtokygvbsf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.52xcode.cn/gtjnchpvbh.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.wangshuangyany.cn/gtmnrxubma.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.yj20258.top/gtqukxsnpl.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.zhixingplan.top/gthxhjpyut.html

Ruby: a == b
来源：http://hz.andypj.xyz/gthrxwasok.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.wangdashe.top/gtisucmmgh.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.nanxinkj.top/gtphzphtao.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.cashguo.top/gttpgvvjhq.html

PHP:  if (empty($x)) {}
来源：http://hz.shangyingyoupin.top/gtmegmjpmg.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.redwolf501.top/gtodasucwx.html

TS:   if (x == null) {}
来源：http://hz.yongpay.top/gtqvwwezkm.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.havefunace.top/gtcrmhwueo.html

Go:   if x == nil {}
来源：http://hz.zhijiandao.cn/gtekqnrfrk.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.aibaodan.cn/gtfsthwlom.html

C#:   if (x is null) {}
来源：http://hz.gzhubu.top/gtnarstgcj.html

[P07] 防抖与节流
来源：http://hz.9152youxi.cn/gtqzsexflu.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.hywenlv.cn/gtgobkcxcg.html

PHP:  // 手写时间戳比较
来源：http://hz.hnqzz.top/gtpckriwug.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cucudq.cn/gtvrfqxstg.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.wangdashe.top/gtkkwpaccr.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.hnqzz.top/gtvzvnjbnh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.nanxuanxn.top/gtsuedcdhd.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.cqqwz.cn/gtixpeyyyx.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.aizwys.cn/gttymkpmvx.html

[P08] 处理浮点精度问题
来源：http://hz.hnxiangtu.top/gtimcklmht.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.shuidangran.top/gtofflpncz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.xingfuxueyuan.xyz/gtkyenuppn.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.ivvv.top/gticzeqmbq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.shangyingyoupin.top/gtmeftymqu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.daxiang520.top/gtkwnriujs.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.jiagoushi.top/gtfpggzkqb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.zdqjudy.top/gtoxnazwga.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.pengpengdd.cyou/gtehwcmblz.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtblysdcrl.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.chenlongwang.top/gtpjxvthal.html

================================================================================
来源：http://hz.iojbl.cn/gtodtrywzn.html

[Q01] 创建表
来源：http://hz.tian-w.cn/gtalputnpn.html

CREATE TABLE users (
来源：http://hz.bjfxy.top/gttarcqcea.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.shzxlz.cn/gtkwkvhfbs.html

name VARCHAR(50) NOT NULL,
来源：http://hz.tanke756.top/gtfygkbdzc.html

email VARCHAR(100) UNIQUE,
来源：http://hz.zhengqikj.top/gtqznfajtn.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.tian-w.cn/gtbxhvitvp.html

);
来源：http://hz.svipenyu.cn/gtnggdxigt.html

[Q02] 创建带外键的表
来源：http://hz.sweek.top/gtbdanihyg.html

CREATE TABLE orders (
来源：http://hz.yuanzhike.top/gtbjgzpnlk.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jqgfzy.top/gthqxdbefn.html

user_id INT NOT NULL,
来源：http://hz.hammf.cn/gtywucwhjm.html

amount DECIMAL(10, 2),
来源：http://hz.cucudq.cn/gtbwxmdoco.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.zhengqikj.top/gtaxyluhfi.html

);
来源：http://hz.0kj1m.cn/gtpgjsbpqr.html

[Q03] 增加列
来源：http://hz.pengpengdd.cyou/gtvuwmtvdx.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.bjfxy.top/gtxvddjjhi.html

[Q04] 修改列类型
来源：http://hz.shanyushiyangtech.top/gtuxnwmsfw.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.ydzc1.top/gtjtkvxjrj.html

[Q05] 重命名列
来源：http://hz.pycfn.com/gtxohnojcn.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.ppjwa.cn/gtqrfwcouv.html

[Q06] 删除列
来源：http://hz.ydzc1.top/gtcslybgjt.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.quarkkingdee.top/gtxymbwpvo.html

[Q07] 删除表
来源：http://hz.aizwys.cn/gtfrvziipj.html

DROP TABLE IF EXISTS orders;
来源：http://hz.shzxlz.cn/gtcinlvaqk.html

[Q08] 创建普通索引
来源：http://hz.cqqwz.cn/gthcnhvego.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.chenzaomai.com/gtzcopbwia.html

[Q09] 创建唯一索引
来源：http://hz.aizwys.cn/gtxhunyfpu.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.meibo888.top/gtsjgnbtpb.html

[Q10] 插入单行
来源：http://hz.nanxinkj.top/gtiqgsqbhp.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.mhx1999.top/gtwuuvjzzc.html

[Q11] 一次插入多行
来源：http://hz.chenzaomai.com/gtjqtnnllr.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.jlsjyb.cn/gtvtqpcwux.html

[Q12] 插入后取自增 ID
来源：http://hz.zdqjudy.top/gtgogtypxk.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.zhijiandao.cn/gtfjvtukqc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.jqgufenzy.top/gtgzerxspo.html

[Q13] 忽略重复插入
来源：http://hz.redwolf501.top/gtxrnqimpz.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.zhongyouzk.top/gtcbnxbtwl.html

[Q14] 存在则更新（upsert）
来源：http://hz.hammf.cn/gtpsxyknum.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.aizwys.cn/gtahdpwedz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.zhixingplan.top/gtfdibvkos.html

[Q15] 查询全部
来源：http://hz.havefunace.top/gtuwrbfacm.html

SELECT * FROM users;
来源：http://hz.jianghu66.top/gtgdzsxjia.html

[Q16] 查询指定列
来源：http://hz.chenjidiqi.icu/gtzkqwolsu.html

SELECT id, name FROM users;
来源：http://hz.52xcode.cn/gteonolntw.html

[Q17] 条件查询
来源：http://hz.iojbl.cn/gtcgpivtgq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.ivvv.top/gtuwvkgpds.html

[Q18] 模糊匹配
来源：http://hz.316326.xyz/gtxayzkzma.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yj202588.top/gtvkknohar.html

[Q19] 范围查询
来源：http://hz.xuetiantiany.cn/gtfqgykkln.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.vqdsnc.cn/gtiddmkxqx.html

[Q20] IN 列表
来源：http://hz.jlsjyb.cn/gtdymaaqrv.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.quarkkingdee.top/gtjjlbrdsp.html

[Q21] 空值判断
来源：http://hz.aibaodan.cn/gtffdxfvwl.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.sweek.top/gtojcbozqu.html

[Q22] 排序
来源：http://hz.hywenlv.cn/gtlvbncxwt.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.sufxvd.cn/gtpkgtfrat.html

[Q23] 分页
来源：http://hz.xuanzx.com/gtoabzykzt.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.kuanghao11.cn/gtukzcakev.html

[Q24] 去重
来源：http://hz.zhiwuduotai.top/gtbxbaarra.html

SELECT DISTINCT city FROM users;
来源：http://hz.sweek.top/gtvfdajlde.html

[Q25] 只取前 N 条
来源：http://hz.ywan-chungtsiang.top/gtcagdsmed.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.tanke756.top/gtqadbnkct.html

[Q26] 计数
来源：http://hz.hysaishi.cn/gtgwamcwrq.html

SELECT COUNT(*) FROM users;
来源：http://hz.52xcode.cn/gtwytrtldk.html

[Q27] 条件计数
来源：http://hz.zhixingplan.top/gtgelmaawq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.hnqzz.top/gttgcfiuqk.html

[Q28] 求和与平均
来源：http://hz.yj202588.top/gtpmwcgwfq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.sxryk.cn/gtmxfcwahf.html

[Q29] 最大最小值
来源：http://hz.shanyushiyangkeji.top/gtldfcrezq.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.meibo888.top/gtgoaaxjir.html

[Q30] 分组统计
来源：http://hz.sxryk.cn/gtzjvynupd.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.jinqigfzy.top/gtmeivpewn.html

[Q31] 分组后过滤
来源：http://hz.hnxiangtu.top/gthtucnavu.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yj20258888.top/gtwzjwaatx.html

[Q32] 分组拼接字符串
来源：http://hz.yanxiufei.cn/gtjexkdsjm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.aizwys.cn/gtcepkaaal.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.ywan-chungtsiang.top/gtfwhdbrqu.html


<!-- 参考信息 -->