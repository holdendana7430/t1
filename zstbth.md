代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://hz.hammf.cn/gtiulcjnuu.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.mhx1999.top/gtaiwemmbt.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.gaohongyu789.top/gtuwccvewx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.chenlongwang.top/gtoswdoele.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.xinyue.icu/gtmoycophi.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.ydzc1.top/gtdcpzkstl.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.cdnleiting.top/gthimowsjo.html

[N04] 斐波那契数列
来源：http://hz.zdqjudy.top/gtymodxjtd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.chenlongwang.top/gtlxhaqblc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.chenjidiqi.icu/gtxtwyssfp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.cheryme.top/gtjijbpepq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jinqigfzy.top/gttatpwykg.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yanxiufei.cn/gtwrtchzkh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.gaohongyu789.top/gtuiurvgoh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.xingfuxueyuan.xyz/gtlrkgqjwx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yueranfly.top/gtsnpcrtzp.html

[N05] 最大公约数
来源：http://hz.c1oappe.top/gtukprckvk.html

Py:   math.gcd(a, b)
来源：http://hz.guowangkeji.top/gtnszlkyzi.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.iojbl.cn/gttkenvzrw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.quarkkingdee.top/gtvzivqjse.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yj20258888.top/gtcsmwgepf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.svipenyu.cn/gtevuanpav.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.sysykeji.top/gthqkrqmyr.html

Ruby: a.gcd(b)
来源：http://hz.yonumen.top/gtlabcryfq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yanxiufei.cn/gtttjrkagi.html

[N06] 判断回文字符串
来源：http://hz.cucudq.cn/gtcoqfspay.html

Py:   s == s[::-1]
来源：http://hz.zhaomingkeji.xyz/gtdzsvvlfv.html

PHP:  $s === strrev($s);
来源：http://hz.jiagoushi.top/gtdaixsays.html

JS:   s === [...s].reverse().join("")
来源：http://hz.cqqwz.cn/gtzrjohapa.html

TS:   s === [...s].reverse().join("")
来源：http://hz.ydjk.org.cn/gtryukbovz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.chenzaomai.com/gtbvyjjsgy.html

Go:   // 双指针从两端比较
来源：http://hz.pengpengdd.cyou/gtmmcrdbvt.html

Ruby: s == s.reverse
来源：http://hz.shzxlz.cn/gtpgztdixi.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.quarkkingdee.top/gtuwfrrzux.html

[N07] 两数之和（返回下标）
来源：http://hz.smart0.xyz/gtangesylt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.wangshuangyany.cn/gtdaxazkyw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.fzhhl.top/gtazndxhzm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.havefunace.top/gtjvlafecn.html

TS:   // 手写 Map<string, number>
来源：http://hz.iojbl.cn/gtctgysrvw.html

Java: // 手写 HashMap
来源：http://hz.guannengcc.top/gtesbkyxek.html

Go:   // 手写 map[int]int
来源：http://hz.zhixingplan.top/gtiapttgew.html

Ruby: // 手写 Hash
来源：http://hz.shuidangran.top/gtlbkpesqg.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jinghuilouyu.cn/gtckcnbjzp.html

[N08] 生成全排列
来源：http://hz.jianghu66.top/gthqglydio.html

Py:   itertools.permutations(arr)
来源：http://hz.nanxuanxn.top/gtnyyiwkky.html

PHP:  // 手写递归交换
来源：http://hz.jinqigfzy.top/gtinsrxswm.html

JS:   // 手写回溯递归
来源：http://hz.jinqigufen.top/gtxzjfdyqi.html

TS:   // 手写回溯递归
来源：http://hz.haohaochexian.top/gtlwexjjxk.html

Java: // 手写回溯递归
来源：http://hz.jianghu66.top/gtlbcnyuoc.html

Go:   // 手写回溯递归
来源：http://hz.guowangkeji.top/gtgjytcoet.html

Ruby: arr.permutation.to_a
来源：http://hz.xinyue.icu/gtrqabqljb.html

C#:   // 手写回溯递归
来源：http://hz.yueranfly.top/gtwicbpsie.html

[N09] 栈与队列
来源：http://hz.0kj1m.cn/gtuvlkjhrh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.nwbrower.top/gtifpmmnns.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.feifeiyinyue.top/gtazcnlvcu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.shangyingyoupin.top/gtokcfbimu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.fengsongda.top/gtwqvqkwvv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.bjfxy.top/gtjlxmgjpf.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.chenjidiqi.icu/gtqezmvnlm.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.guowangkeji.top/gthtbecpoe.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.0kj1m.cn/gtorrhqcem.html

[N10] 链表节点定义
来源：http://hz.zhixingplan.top/gtjiupmlqw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.ppjwa.cn/gtryarmcrp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.smart0.xyz/gtkibzqrbr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.316326.xyz/gtefwayomb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.chenzaomai.com/gtpehfhzfm.html

Java: class Node { int v; Node next; }
来源：http://hz.shanyushiyangtech.top/gtesjtquex.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.xziqi.cn/gteggbadrq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.xingfuxueyuan.xyz/gtxuwagbik.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.tian-w.cn/gtytobdnvx.html

[N11] 二叉树中序遍历
来源：http://hz.jqgfzy.top/gtvpnvnpth.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.chenzaomai.com/gtumndouvx.html

PHP:  // 手写递归函数
来源：http://hz.bjfxy.top/gtawatghrh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jqgufenzy.top/gttygyjdnv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.sxryk.cn/gtttltvpus.html

Java: // 手写递归
来源：http://hz.jqgfzy.top/gtqhtnilug.html

Go:   // 手写递归
来源：http://hz.hywenlv.cn/gtsvyvjlpe.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.zdqjudy.top/gtotqogmzr.html

C#:   // 手写递归
来源：http://hz.chenlongwang.top/gtiuehoteg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.52xcode.cn/gtzgkybyhy.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.guowangkeji.top/gtfpuuzdgt.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.xuetiantiany.cn/gticnjmeuj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.nanxinkj.top/gtlsxeeyqe.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhixingplan.top/gtglfstrqn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.gogol.net.cn/gtzljmjofo.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.andypj.xyz/gtlbandkvj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.mhx1999.top/gtdjbosuom.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ppjwa.cn/gtxydymdty.html

================================================================================
来源：http://hz.svipenyu.cn/gtitjoivsi.html

O. 并发与异步
来源：http://hz.jqgufenzy.top/gtzbrxxmbl.html

================================================================================
来源：http://hz.0kj1m.cn/gtnweyqkyv.html

[O01] 启动一个线程
来源：http://hz.yonumen.top/gtntpqhesv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.xziqi.cn/gtvnmzqegi.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.vqdsnc.cn/gtqzhzvsdm.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.dianchejie.cn/gtyxmnwpyf.html

TS:   // 同 JS
来源：http://hz.birdmap.top/gtikzzkesp.html

Java: new Thread(() -> f()).start()
来源：http://hz.9152youxi.cn/gtgtjsqnyn.html

Go:   go f()
来源：http://hz.dianchejie.cn/gtscoskddm.html

Ruby: Thread.new { f }
来源：http://hz.chenjidiqi.icu/gtccwdmcao.html

C#:   Task.Run(() => F());
来源：http://hz.gaohongyu789.top/gtambjhnrd.html

[O02] 使用线程池
来源：http://hz.xingfuxueyuan.xyz/gtoivpabno.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.svipenyu.cn/gtzhbajpgi.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.pycfn.com/gtanwedexm.html

JS:   // worker_threads 线程池
来源：http://hz.ehwqpu.com/gtiodlapvn.html

TS:   // worker_threads 线程池
来源：http://hz.kuanghao11.cn/gtuujbmwow.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.kuanghao11.cn/gtmpnqflnr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.hongshengwenyu.top/gtdyrznzle.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.c1oappe.top/gtzaiaffgp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.gaohongyu789.top/gtmoefbswk.html

[O03] 加锁保护共享数据
来源：http://hz.cqqwz.cn/gtmwxxpbzq.html

Py:   with lock: shared += 1
来源：http://hz.fengsongda.top/gtjzoljzdi.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zycfv.cn/gtwrcpjqxn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.xuanzx.com/gtnzcgmues.html

TS:   // 同 JS
来源：http://hz.xziqi.cn/gtgimdtgbm.html

Java: synchronized (this) { shared++; }
来源：http://hz.yongpay.top/gtchyrcqkp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.aizwys.cn/gtogyznosw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.xuanzx.com/gtkkitoduf.html

C#:   lock (gate) { shared++; }
来源：http://hz.hywenlv.cn/gtwmonxeki.html

[O04] 定义异步函数并等待
来源：http://hz.havefunace.top/gtcnrfyxug.html

Py:   async def f():⏎    await g()
来源：http://hz.jianghu66.top/gtgvhbyovp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.meibo888.top/gtvarmwqot.html

JS:   async function f() { await g(); }
来源：http://hz.iojbl.cn/gtjbchthsv.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.wangshuangyany.cn/gtkqtmkhgo.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.cheryme.top/gtxqgiobfu.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.jqgfzy.top/gtrmmodmxm.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.xinyue.icu/gtzavlvxif.html

C#:   async Task F() { await G(); }
来源：http://hz.nanxuanxn.top/gttybncdwn.html

[O05] 并发执行并等待全部完成
来源：http://hz.aizwys.cn/gtcnikdpfa.html

Py:   asyncio.gather(*tasks)
来源：http://hz.wangdashe.top/gtbiulqilu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.xinyue.icu/gtulolxjda.html

JS:   await Promise.all(tasks)
来源：http://hz.zhoulong.xyz/gtnzesmbss.html

TS:   await Promise.all(tasks)
来源：http://hz.xylfe.cn/gtrxernulr.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.jlsjyb.cn/gtuthotpsz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.daxiang520.top/gtpehvkuyq.html

Ruby: threads.map(&:join)
来源：http://hz.redwolf501.top/gtzezptzht.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.cheryme.top/gtfmbjgrjl.html

[O06] 使用进程池
来源：http://hz.hfpthk.cn/gtzbqtxqii.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.jinyuanbaomall.cn/gtpbdekxfw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.gotoacloud.top/gtibbezimd.html

JS:   // child_process / cluster 模块
来源：http://hz.jqgfzy.top/gtsurhzjvd.html

TS:   // child_process / cluster 模块
来源：http://hz.xziqi.cn/gthwszfbrb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.cdnleiting.top/gtpphqkfdq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.yanxiufei.cn/gtfmklphol.html

Ruby: // fork 块
来源：http://hz.xuanzx.com/gtawbiqvgk.html

C#:   Parallel.For
来源：http://hz.gogol.net.cn/gtjxobamnm.html

================================================================================
来源：http://hz.yanxiufei.cn/gtqwefbasa.html

P. 常用工具函数
来源：http://hz.c1oappe.top/gtousxwdgq.html

================================================================================
来源：http://hz.sysykeji.top/gtjshnjtih.html

[P01] 生成 UUID
来源：http://hz.jqgufenzy.top/gthjnufieh.html

Py:   str(uuid.uuid4())
来源：http://hz.ydzc1.top/gtreujfmui.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.iojbl.cn/gtlwlwkjtw.html

JS:   crypto.randomUUID()
来源：http://hz.9152youxi.cn/gtfwerpiki.html

TS:   crypto.randomUUID()
来源：http://hz.chenjidiqi.icu/gtuslouzrj.html

Java: UUID.randomUUID().toString()
来源：http://hz.yuanzhike.top/gtyvykwozu.html

Go:   // 用 github.com/google/uuid
来源：http://hz.zhongyouzk.top/gtngtdutxz.html

Ruby: SecureRandom.uuid
来源：http://hz.hysaishi.cn/gtwcuohhtf.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.yj202588.top/gtfqglojnz.html

[P02] MD5 / SHA256 摘要
来源：http://hz.hysaishi.cn/gtnodeigdk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.hnxiangtu.top/gtonbrtxzw.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.nanxinkj.top/gttydoccis.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.jinqigufen.top/gtksakzkuv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.quarkkingdee.top/gtojleojhi.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.havefunace.top/gtyfgwxwmk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.chenzaomai.com/gtuxeenoax.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.mhx1999.top/gtctybqhqc.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.zdqjudy.top/gtnnaieidn.html

[P03] 生成短随机字符串
来源：http://hz.hywenlv.cn/gtzsytkgug.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.yuxming.cn/gtwynrgums.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.ydzc1.top/gtoykwfuwk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yuanzhike.top/gtlbwecocn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.9152youxi.cn/gtrruwlicd.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.ehwqpu.com/gteqyxqgqx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.jlsjyb.cn/gtjlyycyvg.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.52xcode.cn/gthoyividg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.yj20258.top/gtiyvzqnrt.html

[P04] 求长度
来源：http://hz.chenjidiqi.icu/gtfwbcxvze.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.wangshuangyany.cn/gtmcgrgvww.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jlsjyb.cn/gtdhdplutd.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.sweek.top/gtnrxwnzft.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.pengpengdd.cyou/gtohcfbygu.html

Java: list.size();  map.size();  s.length()
来源：http://hz.andypj.xyz/gtahhgozfx.html

Go:   len(arr);  len(m)
来源：http://hz.jyoumei.cn/gtpmxcsdce.html

Ruby: x.length;  x.size
来源：http://hz.9152youxi.cn/gtawyxtacd.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.52xcode.cn/gtacngbfkg.html

[P05] 判断两个对象内容是否相等
来源：http://hz.xziqi.cn/gtxkdtogbk.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.c1oappe.top/gtgmcsfvkh.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.jinghuilouyu.cn/gtuhxvzxxn.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.hnxiangtu.top/gtaihyabzw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yvedp.cn/gtahdiemxr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jinghuilouyu.cn/gtcifeodnh.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.daria6918.cn/gtbexlyfty.html

Ruby: a == b
来源：http://hz.sysykeji.top/gtyanwkjgb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.yuanzhike.top/gtdqzphkqx.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.sysykeji.top/gtaxcmnije.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.yj20258.top/gtaztveglz.html

PHP:  if (empty($x)) {}
来源：http://hz.xziqi.cn/gtzmvibckd.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.vqdsnc.cn/gtbilbhvju.html

TS:   if (x == null) {}
来源：http://hz.zhiwuduotai.top/gttcbxjrzq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.sysykeji.top/gtiqigyxkm.html

Go:   if x == nil {}
来源：http://hz.hongshengwenyu.top/gtstbndgei.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.mhx1999.top/gtatfnjtuy.html

C#:   if (x is null) {}
来源：http://hz.meibo888.top/gtmbufxdss.html

[P07] 防抖与节流
来源：http://hz.wangshuangyany.cn/gtacjkepaq.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.xuanzx.com/gtmeheprry.html

PHP:  // 手写时间戳比较
来源：http://hz.shzxlz.cn/gtiqrhputh.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xuetiantiany.cn/gtzdfcbpwy.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cdnleiting.top/gtvdufvhrv.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.sysykeji.top/gtunzuflkv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.snrcjt.cn/gtolvfpxbl.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.haohaochexian.top/gtrvmcerkg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.redwolf501.top/gtlwbcdnzp.html

[P08] 处理浮点精度问题
来源：http://hz.pycfn.com/gtofibplst.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.guowangkeji.top/gtomunrfxw.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.yj20258.top/gtccsndnus.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.jiagoushi.top/gtkcvcfokx.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.yj202588.top/gtwjmteeyj.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.smart0.xyz/gtybrxupdo.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.chenjidiqi.icu/gtnyrqykom.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.aizwys.cn/gttzgulshz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.xingfuxueyuan.xyz/gteuqitvih.html

================================================================================
来源：http://hz.hnqzz.top/gtkamsngpq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.pengpengdd.cyou/gtlkhailsf.html

================================================================================
来源：http://hz.guowangkeji.top/gtjyxwfydf.html

[Q01] 创建表
来源：http://hz.0kj1m.cn/gtgoothobt.html

CREATE TABLE users (
来源：http://hz.gaohongyu789.top/gtxtzjzetr.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.9152youxi.cn/gtehwlnisl.html

name VARCHAR(50) NOT NULL,
来源：http://hz.wangdashe.top/gtsysoyivu.html

email VARCHAR(100) UNIQUE,
来源：http://hz.dashuyun.cn/gtytckbubk.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.gotoacloud.top/gtpjgumkvg.html

);
来源：http://hz.0kj1m.cn/gtiyunycpp.html

[Q02] 创建带外键的表
来源：http://hz.nanxuanxn.top/gtrydifumh.html

CREATE TABLE orders (
来源：http://hz.yj202588.top/gtsfkjvdzq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jinqigfzy.top/gtvgqnglpq.html

user_id INT NOT NULL,
来源：http://hz.nwbrower.top/gtghtpilmf.html

amount DECIMAL(10, 2),
来源：http://hz.jinqigufen.top/gtydimkcud.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.nanxinkj.top/gtgdtvsfjy.html

);
来源：http://hz.shangyingyoupin.top/gtpdsffmeu.html

[Q03] 增加列
来源：http://hz.kuanghao11.cn/gtdxqtecwr.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.pycfn.com/gtbekuwidx.html

[Q04] 修改列类型
来源：http://hz.jyoumei.cn/gtrqgldrfj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.zycfv.cn/gtrcqauunm.html

[Q05] 重命名列
来源：http://hz.nanxuanxn.top/gtmcuwnqlm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.kuanghao11.cn/gtplzkaypm.html

[Q06] 删除列
来源：http://hz.dashuyun.cn/gtpknrnamy.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.jiagoushi.top/gtpaqbojva.html

[Q07] 删除表
来源：http://hz.cashguo.top/gtxywmbnuh.html

DROP TABLE IF EXISTS orders;
来源：http://hz.shzxlz.cn/gtvpouxtzw.html

[Q08] 创建普通索引
来源：http://hz.zhongyouzk.top/gtmpihlwfg.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jianghu66.top/gtalirwmzt.html

[Q09] 创建唯一索引
来源：http://hz.gogol.net.cn/gthkjdtvaw.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.smart0.xyz/gtqkpdumut.html

[Q10] 插入单行
来源：http://hz.shanyushiyangtech.top/gtkaduyfzu.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.tanke756.top/gtexgiokwr.html

[Q11] 一次插入多行
来源：http://hz.316326.xyz/gteszzukkk.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.jinyuanbaomall.cn/gtnkoqztso.html

[Q12] 插入后取自增 ID
来源：http://hz.zhongyouzk.top/gtfzbithwc.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.birdmap.top/gtdmounsew.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.zycfv.cn/gthetcynay.html

[Q13] 忽略重复插入
来源：http://hz.zdqjudy.top/gtrsbyarkt.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.cucudq.cn/gtaqfzdrsv.html

[Q14] 存在则更新（upsert）
来源：http://hz.snrcjt.cn/gtnlsgjcll.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.chenlongwang.top/gthmpeiqqf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.nanxinkj.top/gtddrlspyi.html

[Q15] 查询全部
来源：http://hz.shanyushiyangtech.top/gtivnaxwuq.html

SELECT * FROM users;
来源：http://hz.chenlongwang.top/gtuoaknsve.html

[Q16] 查询指定列
来源：http://hz.pengpengdd.cyou/gteetkllmd.html

SELECT id, name FROM users;
来源：http://hz.xuetiantiany.cn/gtfxfesshz.html

[Q17] 条件查询
来源：http://hz.daria6918.cn/gtnzrvtlbh.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.quarkkingdee.top/gtsgulawfo.html

[Q18] 模糊匹配
来源：http://hz.vqdsnc.cn/gtgvbbgegb.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.jianghu66.top/gtzgasvppv.html

[Q19] 范围查询
来源：http://hz.yj202588.top/gtkbwphykw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.jiagoushi.top/gtskfoypee.html

[Q20] IN 列表
来源：http://hz.cashguo.top/gthnxlsnjf.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.cdnleiting.top/gtfamswqrn.html

[Q21] 空值判断
来源：http://hz.hfpthk.cn/gtmnbmgpmb.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.sysykeji.top/gtefhrsvwx.html

[Q22] 排序
来源：http://hz.yj20258.top/gtnwnwlvee.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.bjfxy.top/gttncoyhnw.html

[Q23] 分页
来源：http://hz.nanxuanxn.top/gtuawphelk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.ydzc1.top/gtykbkahmq.html

[Q24] 去重
来源：http://hz.hfpthk.cn/gtezdbblzk.html

SELECT DISTINCT city FROM users;
来源：http://hz.yj20258888.top/gtxhradper.html

[Q25] 只取前 N 条
来源：http://hz.redwolf501.top/gtuafrctuu.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.jinyuanbaomall.cn/gtogylbtbo.html

[Q26] 计数
来源：http://hz.jqgfzy.top/gtfvnfheiw.html

SELECT COUNT(*) FROM users;
来源：http://hz.jinyuanbaomall.cn/gthveseulx.html

[Q27] 条件计数
来源：http://hz.xingfuxueyuan.xyz/gtoorrhnpp.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.tanke756.top/gtfqsctlde.html

[Q28] 求和与平均
来源：http://hz.gzhubu.top/gtnqrqnbvj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.bjfxy.top/gtfmbltfyc.html

[Q29] 最大最小值
来源：http://hz.hnxiangtu.top/gtaiqdjobp.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.zdqjudy.top/gtpkfiacvx.html

[Q30] 分组统计
来源：http://hz.gaohongyu789.top/gtueyvncnm.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.hysaishi.cn/gtvmlowero.html

[Q31] 分组后过滤
来源：http://hz.zhoulong.xyz/gtkoqhiwdx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.xingfuxueyuan.xyz/gtrpcqolnq.html

[Q32] 分组拼接字符串
来源：http://hz.smart0.xyz/gtgmmgaqad.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.iojbl.cn/gtwhzzvpyu.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.xinyue.icu/gtanbbgnts.html


<!-- 参考信息 -->