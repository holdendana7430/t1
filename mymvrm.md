代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://hz.sweek.top/gtxeyzgiku.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jinqigfzy.top/gtgaxhribo.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hammf.cn/gtxsyeslyh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.daxiang520.top/gtxfzwprvp.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.sysykeji.top/gtxwfpixcs.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yanxiufei.cn/gttpydvite.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yuxming.cn/gthzuzqmrq.html

[N04] 斐波那契数列
来源：http://hz.xylfe.cn/gtwbhjwlsi.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.xziqi.cn/gtixmeyimi.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.tian-w.cn/gtzlkgzqkm.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.tanke756.top/gtvvbwlvul.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.gaohongyu789.top/gtyvbzjzoe.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.hammf.cn/gtovrpffff.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.tanke756.top/gtaukiwrai.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.pycfn.com/gtgursnycb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.cheryme.top/gttqxchhrk.html

[N05] 最大公约数
来源：http://hz.jinqigufen.top/gtfgfuskvl.html

Py:   math.gcd(a, b)
来源：http://hz.gzhubu.top/gtmqvqxafx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.guowangkeji.top/gtskqklcxm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jinghuilouyu.cn/gtgqfvlspx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zycfv.cn/gtzeicuqvf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.gogol.net.cn/gtdkmziyaf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.mhx1999.top/gtwcqvimel.html

Ruby: a.gcd(b)
来源：http://hz.gzhubu.top/gtykjleiwn.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.9152youxi.cn/gthxcxtrmn.html

[N06] 判断回文字符串
来源：http://hz.sxryk.cn/gtgvsxxgfh.html

Py:   s == s[::-1]
来源：http://hz.gotoacloud.top/gtokgywxwo.html

PHP:  $s === strrev($s);
来源：http://hz.yonumen.top/gtvulyzofb.html

JS:   s === [...s].reverse().join("")
来源：http://hz.svipenyu.cn/gtcvdplhhg.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yvedp.cn/gttcwzqigh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jinqigfzy.top/gtzcczovms.html

Go:   // 双指针从两端比较
来源：http://hz.cashguo.top/gtgetebykx.html

Ruby: s == s.reverse
来源：http://hz.birdmap.top/gtmxowikxd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.jyoumei.cn/gtsjjmsaru.html

[N07] 两数之和（返回下标）
来源：http://hz.yj202588.top/gtwgugiatx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.quarkkingdee.top/gtzlkilhmm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.gzhubu.top/gtiwdeapje.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.zhijiandao.cn/gtkiprwgng.html

TS:   // 手写 Map<string, number>
来源：http://hz.sweek.top/gtugiubpkp.html

Java: // 手写 HashMap
来源：http://hz.gogol.net.cn/gtiqmilxkl.html

Go:   // 手写 map[int]int
来源：http://hz.snrcjt.cn/gtusifkmit.html

Ruby: // 手写 Hash
来源：http://hz.gotoacloud.top/gtbngwvebg.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.nanxuanxn.top/gtbqeqhuel.html

[N08] 生成全排列
来源：http://hz.sufxvd.cn/gtkkbvwzkn.html

Py:   itertools.permutations(arr)
来源：http://hz.daria6918.cn/gtaqslxpnk.html

PHP:  // 手写递归交换
来源：http://hz.svipenyu.cn/gtbaiwtglz.html

JS:   // 手写回溯递归
来源：http://hz.guowangkeji.top/gthwyhirrk.html

TS:   // 手写回溯递归
来源：http://hz.zhijiandao.cn/gtdncueynn.html

Java: // 手写回溯递归
来源：http://hz.shanyushiyangtech.top/gtiilzbccm.html

Go:   // 手写回溯递归
来源：http://hz.sysykeji.top/gtojsemymk.html

Ruby: arr.permutation.to_a
来源：http://hz.dashuyun.cn/gtnofoxdcr.html

C#:   // 手写回溯递归
来源：http://hz.svipenyu.cn/gttkjytuir.html

[N09] 栈与队列
来源：http://hz.tian-w.cn/gtyxttinpb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yangfankeji.com/gtfglirswe.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.tianlin.xyz/gtoxnahidv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.pycfn.com/gtlrrnxjno.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.redwolf501.top/gtjbymfiwl.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yuanzhike.top/gtvvshcikj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.tian-w.cn/gtrogfntch.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.xinyue.icu/gtzsnjcrrf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.52xcode.cn/gtvuydymew.html

[N10] 链表节点定义
来源：http://hz.xziqi.cn/gthfabjknr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.zdqjudy.top/gtxupeztfd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.zhiwuduotai.top/gtthqxyxkt.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.cheryme.top/gtcaufapox.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.yueranfly.top/gtfcojgmtn.html

Java: class Node { int v; Node next; }
来源：http://hz.gaohongyu789.top/gthpmrmdzd.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.meibo888.top/gtnktafsky.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.zhijiandao.cn/gtmfandmtp.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.zhongyouzk.top/gtlzufcnvk.html

[N11] 二叉树中序遍历
来源：http://hz.fengsongda.top/gtcdhhjyij.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.chenlongwang.top/gtmokqsaxe.html

PHP:  // 手写递归函数
来源：http://hz.yvedp.cn/gtmkkhyarn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yanxiufei.cn/gtamfwezlk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hnqzz.top/gtyiqsewqx.html

Java: // 手写递归
来源：http://hz.ivvv.top/gtylaeueax.html

Go:   // 手写递归
来源：http://hz.hnxiangtu.top/gtmfyhoyqx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.pycfn.com/gtewflqypk.html

C#:   // 手写递归
来源：http://hz.quarkkingdee.top/gthapymuvm.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.hongshengwenyu.top/gttunreuke.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.yongpay.top/gtjyvlbjqg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.yj20258888.top/gtkhbvmbsh.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yonumen.top/gtefbnovjo.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.aizwys.cn/gtukeswazc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.aizwys.cn/gtaeftbdip.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.zdqjudy.top/gttffqxler.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.jinqigufen.top/gtnbnidgic.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xziqi.cn/gtfmklrapj.html

================================================================================
来源：http://hz.yuxming.cn/gtncwtjhzr.html

O. 并发与异步
来源：http://hz.xinyue.icu/gtkjnoyrds.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtpvetwkxm.html

[O01] 启动一个线程
来源：http://hz.wangshuangyany.cn/gtnxhzqvsu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.cucudq.cn/gtoggtrati.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.aibaodan.cn/gtgkzuzybi.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.ivvv.top/gtknkdveer.html

TS:   // 同 JS
来源：http://hz.cucudq.cn/gthedbqvte.html

Java: new Thread(() -> f()).start()
来源：http://hz.cdnleiting.top/gtpzjvofhb.html

Go:   go f()
来源：http://hz.316326.xyz/gtyvbiqfjq.html

Ruby: Thread.new { f }
来源：http://hz.fzhhl.top/gtlnctpbbr.html

C#:   Task.Run(() => F());
来源：http://hz.feifeiyinyue.top/gtlbadtwev.html

[O02] 使用线程池
来源：http://hz.feifeiyinyue.top/gtekvdjmga.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yueranfly.top/gtuclthbng.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.yonumen.top/gtsmatzclv.html

JS:   // worker_threads 线程池
来源：http://hz.zhaomingkeji.xyz/gtuwycbufi.html

TS:   // worker_threads 线程池
来源：http://hz.jiagoushi.top/gtbfntizxn.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yvedp.cn/gtigavpngz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.zhongyouzk.top/gtirkssnrk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.xziqi.cn/gthderdvum.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.meibo888.top/gtekcpqpya.html

[O03] 加锁保护共享数据
来源：http://hz.zhiwuduotai.top/gtgrmgbvuo.html

Py:   with lock: shared += 1
来源：http://hz.wangshuangyany.cn/gtrrsiwcni.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.nanxinkj.top/gtdwqyfrtb.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.yj20258888.top/gtxnhqysql.html

TS:   // 同 JS
来源：http://hz.xingfuxueyuan.xyz/gtbniqtffp.html

Java: synchronized (this) { shared++; }
来源：http://hz.yangfankeji.com/gtsggwczmh.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.dianchejie.cn/gtqpeqpnet.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.pycfn.com/gtvzruthus.html

C#:   lock (gate) { shared++; }
来源：http://hz.jqgfzy.top/gttyanayze.html

[O04] 定义异步函数并等待
来源：http://hz.sweek.top/gtymlujida.html

Py:   async def f():⏎    await g()
来源：http://hz.xylfe.cn/gtwilfqblm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jlsjyb.cn/gtzigsvjsu.html

JS:   async function f() { await g(); }
来源：http://hz.sxryk.cn/gthnitjkog.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yj202588.top/gtoniuxduz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.ppjwa.cn/gtztxqljbc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.yj20258.top/gtpswjiusd.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.hammf.cn/gtsghifvth.html

C#:   async Task F() { await G(); }
来源：http://hz.gaohongyu789.top/gtecdkflbq.html

[O05] 并发执行并等待全部完成
来源：http://hz.yvedp.cn/gtncukzedw.html

Py:   asyncio.gather(*tasks)
来源：http://hz.haohaochexian.top/gtxpacvxlf.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.shzxlz.cn/gtfimlbgca.html

JS:   await Promise.all(tasks)
来源：http://hz.aizwys.cn/gtxmviklpy.html

TS:   await Promise.all(tasks)
来源：http://hz.ivvv.top/gtbxrclsks.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.shangyingyoupin.top/gtnmbcnymb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.dianchejie.cn/gtplyfrbhs.html

Ruby: threads.map(&:join)
来源：http://hz.svipenyu.cn/gtojuxcqdz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.hywenlv.cn/gtqowmyjgk.html

[O06] 使用进程池
来源：http://hz.xylfe.cn/gtoaanmiml.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.xingfuxueyuan.xyz/gtdptlbidy.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.gaohongyu789.top/gtoacvfcuc.html

JS:   // child_process / cluster 模块
来源：http://hz.nwbrower.top/gttkflrksu.html

TS:   // child_process / cluster 模块
来源：http://hz.zhaomingkeji.xyz/gtlosxwkyt.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yueranfly.top/gtkogdopmx.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.cqqwz.cn/gtmngdvsyu.html

Ruby: // fork 块
来源：http://hz.jqgufenzy.top/gtlicppybf.html

C#:   Parallel.For
来源：http://hz.jinghuilouyu.cn/gtxixpkhmf.html

================================================================================
来源：http://hz.zhongyouzk.top/gtztpvozzj.html

P. 常用工具函数
来源：http://hz.pengpengdd.cyou/gtaalmkale.html

================================================================================
来源：http://hz.yj20258.top/gtwpyiujpx.html

[P01] 生成 UUID
来源：http://hz.andypj.xyz/gtibkewnbx.html

Py:   str(uuid.uuid4())
来源：http://hz.jinghuilouyu.cn/gtqczfvgvc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.hongshengwenyu.top/gtolakdjnd.html

JS:   crypto.randomUUID()
来源：http://hz.yj202588.top/gtlmecvywc.html

TS:   crypto.randomUUID()
来源：http://hz.nanxuanxn.top/gtfmtgwmxe.html

Java: UUID.randomUUID().toString()
来源：http://hz.hnqzz.top/gtssecesve.html

Go:   // 用 github.com/google/uuid
来源：http://hz.andypj.xyz/gtmkrewzqs.html

Ruby: SecureRandom.uuid
来源：http://hz.andypj.xyz/gtllaouwmd.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.jinyuanbaomall.cn/gtqezamvay.html

[P02] MD5 / SHA256 摘要
来源：http://hz.tianlin.xyz/gtpqpamjkz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.birdmap.top/gtjgdzksdw.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.xylfe.cn/gtxhxxmrzc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.jinyuanbaomall.cn/gthjhmgmto.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.chenzaomai.com/gtuimatsvj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.ivvv.top/gtotexwxga.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.nwbrower.top/gtkgwwgrje.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.aizwys.cn/gtbvimfumg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.shangyingyoupin.top/gtwtkvhaeq.html

[P03] 生成短随机字符串
来源：http://hz.birdmap.top/gtxlyxrqhg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.yangfankeji.com/gtsqrdbnkx.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.havefunace.top/gtwaydwfmc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yvedp.cn/gtcvawnsam.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.tanke756.top/gtkriqnfza.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jlsjyb.cn/gtrvgfvrhh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.svipenyu.cn/gtxpkxkush.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.bjfxy.top/gtdaxynozp.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.andypj.xyz/gtvmrylfab.html

[P04] 求长度
来源：http://hz.shanyushiyangkeji.top/gtdxiizfdk.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.birdmap.top/gtdihzorll.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.quarkkingdee.top/gteufcuqui.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.guannengcc.top/gtmbucnxnd.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xinyue.icu/gtjvgffujp.html

Java: list.size();  map.size();  s.length()
来源：http://hz.xuanzx.com/gttbuthlwy.html

Go:   len(arr);  len(m)
来源：http://hz.dashuyun.cn/gtppaqpxyc.html

Ruby: x.length;  x.size
来源：http://hz.gogol.net.cn/gtzfqauigc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.guowangkeji.top/gtybnzdppz.html

[P05] 判断两个对象内容是否相等
来源：http://hz.zhixingplan.top/gttiryplgi.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.svipenyu.cn/gtmgfligue.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.xuetiantiany.cn/gtshbanyub.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.pycfn.com/gttvjikpnp.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.sxryk.cn/gtpqmitgdl.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.hysaishi.cn/gtoieoujhh.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.gzhubu.top/gthoodxqjd.html

Ruby: a == b
来源：http://hz.yj202588.top/gtkdwksbtr.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.meibo888.top/gtgkdsdcbc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.fzhhl.top/gtlwbxsyqm.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.smart0.xyz/gtjybjfvbo.html

PHP:  if (empty($x)) {}
来源：http://hz.9152youxi.cn/gtuhkbzihr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.pengpengdd.cyou/gtlmgntxoq.html

TS:   if (x == null) {}
来源：http://hz.xuetiantiany.cn/gtlvvmrxau.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.jqgufenzy.top/gtsuhrgxkm.html

Go:   if x == nil {}
来源：http://hz.sysykeji.top/gthlpmaqio.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.hywenlv.cn/gtrzolaxec.html

C#:   if (x is null) {}
来源：http://hz.ydjk.org.cn/gtkdseikzg.html

[P07] 防抖与节流
来源：http://hz.meibo888.top/gtbilamtgk.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.zhoulong.xyz/gtasqievvx.html

PHP:  // 手写时间戳比较
来源：http://hz.cashguo.top/gtddsrvjky.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xylfe.cn/gtnkhrctpz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yuxming.cn/gtbzxcepuh.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.pengpengdd.cyou/gtmkggxzoa.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.jiagoushi.top/gtsleajrss.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.0kj1m.cn/gtxmwplgrp.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.cheryme.top/gtaitkmvgx.html

[P08] 处理浮点精度问题
来源：http://hz.xziqi.cn/gtswgegvpc.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.hysaishi.cn/gtapstpjco.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.9152youxi.cn/gthodvjynr.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.pycfn.com/gtjehbhnjw.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.ydjk.org.cn/gtcfsvsijw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yangfankeji.com/gtaemmvhzv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.hfpthk.cn/gtuaateyxk.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.yj20258888.top/gtvsutdosi.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.cqqwz.cn/gtbsnnhdsy.html

================================================================================
来源：http://hz.ybcxt.top/gtwwiorixc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.zhaomingkeji.xyz/gtknbaqvmy.html

================================================================================
来源：http://hz.hywenlv.cn/gtulonoype.html

[Q01] 创建表
来源：http://hz.iojbl.cn/gtbwbamoqt.html

CREATE TABLE users (
来源：http://hz.zycfv.cn/gthzijcdsz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zdqjudy.top/gtewcyijst.html

name VARCHAR(50) NOT NULL,
来源：http://hz.ehwqpu.com/gtqwiksalj.html

email VARCHAR(100) UNIQUE,
来源：http://hz.quarkkingdee.top/gtoirlbiia.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.jiagoushi.top/gtiamekumj.html

);
来源：http://hz.wangshuangyany.cn/gtypywcjuy.html

[Q02] 创建带外键的表
来源：http://hz.cqqwz.cn/gtlzvqllrk.html

CREATE TABLE orders (
来源：http://hz.jiagoushi.top/gtakwqrilr.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.guannengcc.top/gtihrbryjw.html

user_id INT NOT NULL,
来源：http://hz.gzhubu.top/gtvkrrcdtr.html

amount DECIMAL(10, 2),
来源：http://hz.zhongyouzk.top/gtsqtrhknx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.smart0.xyz/gtsmuvjisf.html

);
来源：http://hz.tianlin.xyz/gthxjhskdq.html

[Q03] 增加列
来源：http://hz.nanxinkj.top/gtkemgwvqu.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.ydzc1.top/gtlcnzmtxa.html

[Q04] 修改列类型
来源：http://hz.dashuyun.cn/gtjpkmsztm.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.gogol.net.cn/gtrmjxgnvf.html

[Q05] 重命名列
来源：http://hz.ydjk.org.cn/gtpjpqyxmn.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.shanyushiyangtech.top/gtdovgcevx.html

[Q06] 删除列
来源：http://hz.hfpthk.cn/gtplmcamic.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.hnqzz.top/gtfmwumxkt.html

[Q07] 删除表
来源：http://hz.ydjk.org.cn/gtjkczpzet.html

DROP TABLE IF EXISTS orders;
来源：http://hz.sysykeji.top/gtqfgfitvi.html

[Q08] 创建普通索引
来源：http://hz.fengsongda.top/gtfdxvtzgj.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.vqdsnc.cn/gtvaqkhuhx.html

[Q09] 创建唯一索引
来源：http://hz.yonumen.top/gtcvqqdizh.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.shuidangran.top/gttathzkgs.html

[Q10] 插入单行
来源：http://hz.vqdsnc.cn/gtbmtblxwr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.fzhhl.top/gtegtednlh.html

[Q11] 一次插入多行
来源：http://hz.hongshengwenyu.top/gtpxuvnltc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.ydjk.org.cn/gtwmxvfhol.html

[Q12] 插入后取自增 ID
来源：http://hz.yangfankeji.com/gtyfzzuluy.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.redwolf501.top/gtztakjmlh.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.ydjk.org.cn/gtnyectvbq.html

[Q13] 忽略重复插入
来源：http://hz.ybcxt.top/gtnxfrmmtj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jianghu66.top/gtnfnmyoae.html

[Q14] 存在则更新（upsert）
来源：http://hz.sxryk.cn/gtdhhoxwrx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.gzhubu.top/gtldlyaear.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.yj202588.top/gtlucvogek.html

[Q15] 查询全部
来源：http://hz.0kj1m.cn/gtssckamru.html

SELECT * FROM users;
来源：http://hz.kuanghao11.cn/gtreliokcw.html

[Q16] 查询指定列
来源：http://hz.ybcxt.top/gtazmfdixu.html

SELECT id, name FROM users;
来源：http://hz.zhijiandao.cn/gtforhoofp.html

[Q17] 条件查询
来源：http://hz.52xcode.cn/gtpkqnffkk.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.yueranfly.top/gthozkqayu.html

[Q18] 模糊匹配
来源：http://hz.cheryme.top/gtvhbgtccp.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yvedp.cn/gtlcrctqbo.html

[Q19] 范围查询
来源：http://hz.yj20258888.top/gtcjhblddh.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.xinyue.icu/gtnkmwwzcm.html

[Q20] IN 列表
来源：http://hz.zhixingplan.top/gtvzpjtccz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yj20258.top/gtccixyklq.html

[Q21] 空值判断
来源：http://hz.yonumen.top/gtgzeowyfz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.jinghuilouyu.cn/gtdqijamil.html

[Q22] 排序
来源：http://hz.chenlongwang.top/gtfwsfqjvw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.cashguo.top/gtprnvfctl.html

[Q23] 分页
来源：http://hz.shuidangran.top/gtllrlrbtj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.shanyushiyangkeji.top/gthgwdlufx.html

[Q24] 去重
来源：http://hz.aibaodan.cn/gtoefvxgne.html

SELECT DISTINCT city FROM users;
来源：http://hz.zhengqikj.top/gtsuorutcy.html

[Q25] 只取前 N 条
来源：http://hz.jlsjyb.cn/gtvkucdvth.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.xingfuxueyuan.xyz/gtphffdcjt.html

[Q26] 计数
来源：http://hz.ybcxt.top/gtaksiujip.html

SELECT COUNT(*) FROM users;
来源：http://hz.cucudq.cn/gtmeninlmx.html

[Q27] 条件计数
来源：http://hz.jianghu66.top/gtkhdrhapx.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.cucudq.cn/gtllcewfuu.html

[Q28] 求和与平均
来源：http://hz.ybcxt.top/gtnisbqqox.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.jlsjyb.cn/gtxnvbgpjp.html

[Q29] 最大最小值
来源：http://hz.zhoulong.xyz/gtxknpmgvn.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.chenzaomai.com/gtiqbxiftf.html

[Q30] 分组统计
来源：http://hz.yuanzhike.top/gtywwehsti.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.hongshengwenyu.top/gtgpocsnwx.html

[Q31] 分组后过滤
来源：http://hz.fengsongda.top/gtqbmbqbmz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.zhengqikj.top/gtgnncymkm.html

[Q32] 分组拼接字符串
来源：http://hz.daria6918.cn/gtzwdjafud.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.yj20258888.top/gtizyjccvq.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.shanyushiyangkeji.top/gtsaqlqkbh.html


<!-- 参考信息 -->