代发 wailian999

Ruby: arr.sort
来源：http://hz.sxryk.cn/gtgvxwidgy.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.xingfuxueyuan.xyz/gttqiwbygs.html

[N03] 快速排序（分治示例）
来源：http://hz.yueranfly.top/gtuuzvgtjn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.hnxiangtu.top/gtrfdokuwo.html

PHP:  // 递归实现，或用 usort
来源：http://hz.yvedp.cn/gtrfnlrjwn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.fengsongda.top/gtbwodnyzu.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ppjwa.cn/gtgsrjjyqh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.chenzaomai.com/gtwpkfjwwe.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.hnqzz.top/gtjwuzxhre.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.0kj1m.cn/gtsojqprqg.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.ybcxt.top/gtgjtktllr.html

[N04] 斐波那契数列
来源：http://hz.hfpthk.cn/gtagxklsxy.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.hnqzz.top/gtqojvuqyg.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.jinghuilouyu.cn/gtctkaksnh.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.cdnleiting.top/gtlqicnozl.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.dianchejie.cn/gtggtqestu.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.zhixingplan.top/gtxlnlynnp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.cqqwz.cn/gtusjpthnf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.hongshengwenyu.top/gttuiwpxso.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.aibaodan.cn/gtsimklqos.html

[N05] 最大公约数
来源：http://hz.yonumen.top/gtcqmnapqn.html

Py:   math.gcd(a, b)
来源：http://hz.xuetiantiany.cn/gtbmgycbjx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.ppjwa.cn/gtucufwvjl.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.daxiang520.top/gtwdbnphgp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhiwuduotai.top/gtmmponnyw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.chenjidiqi.icu/gteidjtjzo.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.yonumen.top/gtvlackxvu.html

Ruby: a.gcd(b)
来源：http://hz.dashuyun.cn/gtfjftbqmf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jianghu66.top/gtouepvltb.html

[N06] 判断回文字符串
来源：http://hz.vqdsnc.cn/gtoefmtnvf.html

Py:   s == s[::-1]
来源：http://hz.daxiang520.top/gtuktesnja.html

PHP:  $s === strrev($s);
来源：http://hz.cashguo.top/gtagdsgord.html

JS:   s === [...s].reverse().join("")
来源：http://hz.yvedp.cn/gttzjgnwfy.html

TS:   s === [...s].reverse().join("")
来源：http://hz.vqdsnc.cn/gtptmnkiio.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.xziqi.cn/gtceuswbml.html

Go:   // 双指针从两端比较
来源：http://hz.redwolf501.top/gtyswobomx.html

Ruby: s == s.reverse
来源：http://hz.tianlin.xyz/gtcsnidtut.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.shuidangran.top/gtefyurxqc.html

[N07] 两数之和（返回下标）
来源：http://hz.jinghuilouyu.cn/gtbdcwuwfj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.yuanzhike.top/gtpjaoypmo.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yonumen.top/gthdsvcdss.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.jinyuanbaomall.cn/gtpjlluswm.html

TS:   // 手写 Map<string, number>
来源：http://hz.guannengcc.top/gtpnwspaut.html

Java: // 手写 HashMap
来源：http://hz.jianghu66.top/gthwpmytcd.html

Go:   // 手写 map[int]int
来源：http://hz.jqgufenzy.top/gtrhtchehd.html

Ruby: // 手写 Hash
来源：http://hz.hywenlv.cn/gtmifrneqr.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.nanxinkj.top/gtkhsyugmz.html

[N08] 生成全排列
来源：http://hz.zhengqikj.top/gtnacawohk.html

Py:   itertools.permutations(arr)
来源：http://hz.guowangkeji.top/gtadxcfpmt.html

PHP:  // 手写递归交换
来源：http://hz.zhoulong.xyz/gtwoxbksze.html

JS:   // 手写回溯递归
来源：http://hz.xylfe.cn/gtjvxibzcm.html

TS:   // 手写回溯递归
来源：http://hz.chenzaomai.com/gtyywamlqy.html

Java: // 手写回溯递归
来源：http://hz.wangdashe.top/gtsrnnmxfp.html

Go:   // 手写回溯递归
来源：http://hz.nanxinkj.top/gtwcgbntsr.html

Ruby: arr.permutation.to_a
来源：http://hz.hnxiangtu.top/gtnalzacgu.html

C#:   // 手写回溯递归
来源：http://hz.xylfe.cn/gtxguiwdpi.html

[N09] 栈与队列
来源：http://hz.pycfn.com/gtpringfax.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.guannengcc.top/gtddhtqrrl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.9152youxi.cn/gtulzovpkg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.meibo888.top/gtexbkhqut.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yonumen.top/gtzhzpmapd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.aizwys.cn/gtbkzpzwmr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.nanxuanxn.top/gtpehnyade.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.zhongyouzk.top/gtcnnsllyi.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.wangshuangyany.cn/gtdfefgzof.html

[N10] 链表节点定义
来源：http://hz.aibaodan.cn/gtxoedfpai.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.tanke756.top/gthakeuaro.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.ivvv.top/gterotktwp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.gaohongyu789.top/gtqctqbbzk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.zhijiandao.cn/gthaformwn.html

Java: class Node { int v; Node next; }
来源：http://hz.ydzc1.top/gtnmtlfdku.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.yongpay.top/gtzcclsdzc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.ywan-chungtsiang.top/gtjrlfpwei.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.fzhhl.top/gtskzrmxno.html

[N11] 二叉树中序遍历
来源：http://hz.yongpay.top/gtsnehemet.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.zycfv.cn/gtxlaxlrgo.html

PHP:  // 手写递归函数
来源：http://hz.smart0.xyz/gtxhizujlp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.shuidangran.top/gtvqcebtlf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhengqikj.top/gtizyectvw.html

Java: // 手写递归
来源：http://hz.9152youxi.cn/gtpctdkury.html

Go:   // 手写递归
来源：http://hz.smart0.xyz/gthyrqhcld.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.birdmap.top/gtnciktfue.html

C#:   // 手写递归
来源：http://hz.nanxuanxn.top/gtlqvkkoge.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yonumen.top/gtwwexaino.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.jlsjyb.cn/gttqtljfmn.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.zhengqikj.top/gtrsjaybyu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ydjk.org.cn/gturiyagny.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xuanzx.com/gtbycruyel.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.tianlin.xyz/gtnhboltyg.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.zhiwuduotai.top/gtrknzwzna.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.shuidangran.top/gthmsxjbsm.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.tianlin.xyz/gteqipvkur.html

================================================================================
来源：http://hz.yj20258888.top/gtvtbykdnx.html

O. 并发与异步
来源：http://hz.smart0.xyz/gtzoiqexsp.html

================================================================================
来源：http://hz.yongpay.top/gtwbisflgf.html

[O01] 启动一个线程
来源：http://hz.xylfe.cn/gtzrdlpppg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.quarkkingdee.top/gtpzenwomd.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.hnqzz.top/gtpotrefly.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.bjfxy.top/gtynvlnozz.html

TS:   // 同 JS
来源：http://hz.andypj.xyz/gtlpgdhzqi.html

Java: new Thread(() -> f()).start()
来源：http://hz.sxryk.cn/gtasfyimmy.html

Go:   go f()
来源：http://hz.nanxuanxn.top/gtvasnzjsv.html

Ruby: Thread.new { f }
来源：http://hz.meibo888.top/gtgnscrmau.html

C#:   Task.Run(() => F());
来源：http://hz.c1oappe.top/gtekvfcsxb.html

[O02] 使用线程池
来源：http://hz.sufxvd.cn/gtzzifhgir.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yueranfly.top/gteasxxzyt.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.guannengcc.top/gtpmcbjgvt.html

JS:   // worker_threads 线程池
来源：http://hz.hnqzz.top/gtidekdcgc.html

TS:   // worker_threads 线程池
来源：http://hz.cucudq.cn/gtbtfakltx.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.hnqzz.top/gtetsvodyv.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.vqdsnc.cn/gtrqktmtxv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.chenjidiqi.icu/gthcpvyrpc.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.zhongyouzk.top/gthrcxgbvw.html

[O03] 加锁保护共享数据
来源：http://hz.snrcjt.cn/gtgzcdsjhb.html

Py:   with lock: shared += 1
来源：http://hz.haohaochexian.top/gtumlneqje.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.guowangkeji.top/gtukxigaje.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.hnqzz.top/gtdqeeryhi.html

TS:   // 同 JS
来源：http://hz.jinghuilouyu.cn/gtweslhihd.html

Java: synchronized (this) { shared++; }
来源：http://hz.daria6918.cn/gtbyokrsrm.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.nwbrower.top/gtvarorlgy.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.birdmap.top/gtamfzkckk.html

C#:   lock (gate) { shared++; }
来源：http://hz.haohaochexian.top/gtvmkekiby.html

[O04] 定义异步函数并等待
来源：http://hz.yvedp.cn/gtmzbwrazg.html

Py:   async def f():⏎    await g()
来源：http://hz.zhijiandao.cn/gteblmvzub.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.yj20258.top/gtlcjjlrap.html

JS:   async function f() { await g(); }
来源：http://hz.9152youxi.cn/gtgsrztocz.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yangfankeji.com/gtcgtrowrd.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.nanxuanxn.top/gtwrruejmg.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.shanyushiyangtech.top/gtfghbeeei.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.shuidangran.top/gtxwzrufli.html

C#:   async Task F() { await G(); }
来源：http://hz.aibaodan.cn/gtcemhnxjt.html

[O05] 并发执行并等待全部完成
来源：http://hz.hammf.cn/gtpwvwjpnb.html

Py:   asyncio.gather(*tasks)
来源：http://hz.gogol.net.cn/gtvtvazkyh.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.shuidangran.top/gtmdghiewr.html

JS:   await Promise.all(tasks)
来源：http://hz.zhoulong.xyz/gtcsspjzil.html

TS:   await Promise.all(tasks)
来源：http://hz.jyoumei.cn/gtwhxmhpjd.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.xingfuxueyuan.xyz/gtszxuxvso.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.guannengcc.top/gtbgueswrc.html

Ruby: threads.map(&:join)
来源：http://hz.shzxlz.cn/gtpqvzgpjx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.sufxvd.cn/gtgznzyspo.html

[O06] 使用进程池
来源：http://hz.fzhhl.top/gtiflvwprg.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.tanke756.top/gttdorxwva.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.9152youxi.cn/gtqrzwfulz.html

JS:   // child_process / cluster 模块
来源：http://hz.hfpthk.cn/gtaqovmzol.html

TS:   // child_process / cluster 模块
来源：http://hz.mhx1999.top/gtfsdasuoq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.kuanghao11.cn/gtwohvkmec.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.kuanghao11.cn/gtkkmqhgrk.html

Ruby: // fork 块
来源：http://hz.gzhubu.top/gtwbgtciur.html

C#:   Parallel.For
来源：http://hz.jlsjyb.cn/gtszlzrgkn.html

================================================================================
来源：http://hz.yongpay.top/gtlioclykh.html

P. 常用工具函数
来源：http://hz.daria6918.cn/gtlcceupgl.html

================================================================================
来源：http://hz.zhongyouzk.top/gtyzslyasi.html

[P01] 生成 UUID
来源：http://hz.gaohongyu789.top/gtfrilprou.html

Py:   str(uuid.uuid4())
来源：http://hz.zdqjudy.top/gtbgdxyndt.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.hongshengwenyu.top/gtglvnrtdz.html

JS:   crypto.randomUUID()
来源：http://hz.guowangkeji.top/gtkxfwgdye.html

TS:   crypto.randomUUID()
来源：http://hz.pengpengdd.cyou/gtaymwsibu.html

Java: UUID.randomUUID().toString()
来源：http://hz.gotoacloud.top/gtlaeppskm.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yongpay.top/gtwgcllgkn.html

Ruby: SecureRandom.uuid
来源：http://hz.redwolf501.top/gtgcfgwppc.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.aizwys.cn/gtemuogjia.html

[P02] MD5 / SHA256 摘要
来源：http://hz.jinqigfzy.top/gtmsraumkl.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.yongpay.top/gtrlfaunou.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.jianghu66.top/gtooxmqvrg.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.316326.xyz/gtszqkjrux.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.yuanzhike.top/gthjuqhuty.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.gzhubu.top/gthoemcxly.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.iojbl.cn/gtdmispjrl.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.shanyushiyangkeji.top/gtejgbdtno.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.pengpengdd.cyou/gtoxocmkev.html

[P03] 生成短随机字符串
来源：http://hz.shangyingyoupin.top/gtdgarrewi.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jinghuilouyu.cn/gtyklvjtfv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.mhx1999.top/gtpvhgsvwx.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xingfuxueyuan.xyz/gttlnsqvmc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yj20258888.top/gtbeyqocqq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.hnqzz.top/gtfeyrlgle.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.xziqi.cn/gtbyvpyiok.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jinqigfzy.top/gttvgltmzs.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.xuanzx.com/gtmdhptuqx.html

[P04] 求长度
来源：http://hz.sufxvd.cn/gtnwadihol.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.9152youxi.cn/gtvlxmqoku.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.mhx1999.top/gtoyyhdsbz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.meibo888.top/gtqhrptonh.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.havefunace.top/gtdooneaod.html

Java: list.size();  map.size();  s.length()
来源：http://hz.hysaishi.cn/gtklxtzkuw.html

Go:   len(arr);  len(m)
来源：http://hz.shzxlz.cn/gthueqimxt.html

Ruby: x.length;  x.size
来源：http://hz.nanxinkj.top/gthimyxmzg.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.nanxinkj.top/gtyabcgxdt.html

[P05] 判断两个对象内容是否相等
来源：http://hz.redwolf501.top/gtaswekgdm.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.tianlin.xyz/gtldsgozxl.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.hnqzz.top/gtzufelwgg.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.yueranfly.top/gtqijlxfzn.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jqgufenzy.top/gtualnedth.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.zhiwuduotai.top/gtdaobsuvl.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.ehwqpu.com/gtzsnyeebe.html

Ruby: a == b
来源：http://hz.yj20258888.top/gtttocbuts.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.zdqjudy.top/gtvkwqanju.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.wangdashe.top/gtvlmqiuwe.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.chenjidiqi.icu/gtczcjxxog.html

PHP:  if (empty($x)) {}
来源：http://hz.smart0.xyz/gtpzuqcoav.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.zhengqikj.top/gtqynhziwe.html

TS:   if (x == null) {}
来源：http://hz.gogol.net.cn/gtctggzfbp.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.sufxvd.cn/gtquqhloww.html

Go:   if x == nil {}
来源：http://hz.svipenyu.cn/gtnxhclcwa.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.hfpthk.cn/gtfjscmyvh.html

C#:   if (x is null) {}
来源：http://hz.shanyushiyangkeji.top/gtittdahxb.html

[P07] 防抖与节流
来源：http://hz.guowangkeji.top/gtwotagcwo.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.guowangkeji.top/gtxkrfjofv.html

PHP:  // 手写时间戳比较
来源：http://hz.wangdashe.top/gtlhivjnjc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhoulong.xyz/gtibczlchd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.aizwys.cn/gtpbfxmsuf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.yuanzhike.top/gturpziwlj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.xuanzx.com/gtyfxylowt.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yj20258888.top/gtxrudiktn.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.birdmap.top/gtxdpnkcsh.html

[P08] 处理浮点精度问题
来源：http://hz.zhoulong.xyz/gtvjtfebrr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jyoumei.cn/gtgrnesvbl.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.xziqi.cn/gtsbinixae.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.feifeiyinyue.top/gtbuofdihh.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.yuanzhike.top/gtgxmyvnjg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.cdnleiting.top/gtqyenpzli.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.hnqzz.top/gtjtghnjsp.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.chenlongwang.top/gtbyxycxdb.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.daria6918.cn/gttvwwxuzx.html

================================================================================
来源：http://hz.ppjwa.cn/gtjpustxif.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.316326.xyz/gtbjuedrti.html

================================================================================
来源：http://hz.yuxming.cn/gtlpbxagxz.html

[Q01] 创建表
来源：http://hz.yanxiufei.cn/gtrieqfwqz.html

CREATE TABLE users (
来源：http://hz.quarkkingdee.top/gtbvytkhai.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhiwuduotai.top/gtvheowdnd.html

name VARCHAR(50) NOT NULL,
来源：http://hz.xingfuxueyuan.xyz/gtchdupffi.html

email VARCHAR(100) UNIQUE,
来源：http://hz.snrcjt.cn/gtzlsygxwc.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.xziqi.cn/gtwgpzxwqu.html

);
来源：http://hz.aizwys.cn/gtdxwyqalv.html

[Q02] 创建带外键的表
来源：http://hz.9152youxi.cn/gtlvlvaggr.html

CREATE TABLE orders (
来源：http://hz.yangfankeji.com/gtnuvsfrbx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.redwolf501.top/gtqrivnzfh.html

user_id INT NOT NULL,
来源：http://hz.c1oappe.top/gtjrcamkfc.html

amount DECIMAL(10, 2),
来源：http://hz.yanxiufei.cn/gtjoudghbv.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.yvedp.cn/gtazemyevw.html

);
来源：http://hz.gotoacloud.top/gtgqmvjmto.html

[Q03] 增加列
来源：http://hz.jinqigfzy.top/gtqejgfjwj.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.9152youxi.cn/gtefckatlw.html

[Q04] 修改列类型
来源：http://hz.aibaodan.cn/gtietdmbhl.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.nanxuanxn.top/gtyewmdtjo.html

[Q05] 重命名列
来源：http://hz.0kj1m.cn/gtxioxscwb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.guowangkeji.top/gtipzjcbpe.html

[Q06] 删除列
来源：http://hz.ppjwa.cn/gttezeqnxf.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.daria6918.cn/gtsxauqlve.html

[Q07] 删除表
来源：http://hz.ydzc1.top/gtufmmzmds.html

DROP TABLE IF EXISTS orders;
来源：http://hz.cashguo.top/gtlkjwqqkv.html

[Q08] 创建普通索引
来源：http://hz.yuxming.cn/gtzldemlvf.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.chenlongwang.top/gtkojtplxx.html

[Q09] 创建唯一索引
来源：http://hz.fzhhl.top/gtohmzshcv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.zhongyouzk.top/gtpmbctoas.html

[Q10] 插入单行
来源：http://hz.yj20258888.top/gthzahqsus.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.yuxming.cn/gtlimmfper.html

[Q11] 一次插入多行
来源：http://hz.yuanzhike.top/gtjiuokuiu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.xuanzx.com/gtpdsdhiqf.html

[Q12] 插入后取自增 ID
来源：http://hz.yj20258.top/gtiniyzwmr.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.svipenyu.cn/gtxpkmzysj.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yj202588.top/gtybhexkzc.html

[Q13] 忽略重复插入
来源：http://hz.gotoacloud.top/gtbmfkfrta.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.wangshuangyany.cn/gtghaooyby.html

[Q14] 存在则更新（upsert）
来源：http://hz.fzhhl.top/gticvhapvg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.xuetiantiany.cn/gtbnnbtvza.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.tianlin.xyz/gtspnmubvd.html

[Q15] 查询全部
来源：http://hz.yuxming.cn/gtmzciktqg.html

SELECT * FROM users;
来源：http://hz.jlsjyb.cn/gtltmtszwk.html

[Q16] 查询指定列
来源：http://hz.shuidangran.top/gtrcpxlpts.html

SELECT id, name FROM users;
来源：http://hz.tian-w.cn/gtzgeyxddj.html

[Q17] 条件查询
来源：http://hz.cheryme.top/gtdufviwly.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.zdqjudy.top/gtoltqudek.html

[Q18] 模糊匹配
来源：http://hz.havefunace.top/gtnurrrtdf.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.aizwys.cn/gtvxqxjmlf.html

[Q19] 范围查询
来源：http://hz.feifeiyinyue.top/gtahefgbcn.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.xziqi.cn/gtqhqylwgq.html

[Q20] IN 列表
来源：http://hz.shangyingyoupin.top/gtwkkxldzo.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.quarkkingdee.top/gtcosrycqs.html

[Q21] 空值判断
来源：http://hz.sufxvd.cn/gtuszwzrgu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.quarkkingdee.top/gtdpwqznzh.html

[Q22] 排序
来源：http://hz.zhengqikj.top/gtdhzrwjbe.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.zhengqikj.top/gtzpwthent.html

[Q23] 分页
来源：http://hz.shzxlz.cn/gtgzkhapfp.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yueranfly.top/gtfhmvrvbu.html

[Q24] 去重
来源：http://hz.smart0.xyz/gtfhjgdutu.html

SELECT DISTINCT city FROM users;
来源：http://hz.hysaishi.cn/gttkgkuihi.html

[Q25] 只取前 N 条
来源：http://hz.nanxinkj.top/gtdzidthqo.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.hfpthk.cn/gtlsumjhkn.html

[Q26] 计数
来源：http://hz.zhixingplan.top/gtwkvggfnl.html

SELECT COUNT(*) FROM users;
来源：http://hz.hfpthk.cn/gtjistwish.html

[Q27] 条件计数
来源：http://hz.guowangkeji.top/gtamptijah.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.havefunace.top/gtpxvmewdy.html

[Q28] 求和与平均
来源：http://hz.hnqzz.top/gttdovxlhy.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.jinyuanbaomall.cn/gtlewujsqo.html

[Q29] 最大最小值
来源：http://hz.kuanghao11.cn/gtbqkkeihe.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.tian-w.cn/gthbmrliml.html

[Q30] 分组统计
来源：http://hz.shanyushiyangkeji.top/gtfcjghuap.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.sysykeji.top/gtmghujbnl.html

[Q31] 分组后过滤
来源：http://hz.dianchejie.cn/gtpopiyoka.html


<!-- 参考信息 -->