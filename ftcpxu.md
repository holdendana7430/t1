代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://hz.shanyushiyangtech.top/gthrmmigxc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xziqi.cn/gtgwgkognf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.daria6918.cn/gtbmiepdkr.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.wangshuangyany.cn/gtkyqixpgn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.ybcxt.top/gtvpdiwior.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yvedp.cn/gtcdyeblca.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.sxryk.cn/gtmcodqhcz.html

[N04] 斐波那契数列
来源：http://hz.hysaishi.cn/gtgfaifdcb.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jinghuilouyu.cn/gtpdlxnaqc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.shzxlz.cn/gtulxakyzy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yj20258.top/gtquxssjag.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yj20258888.top/gtsrnwrsxl.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.smart0.xyz/gtkoelcqna.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.shzxlz.cn/gtzaqamofk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.snrcjt.cn/gtxyvrtqve.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.cdnleiting.top/gttgtarpom.html

[N05] 最大公约数
来源：http://hz.zhaomingkeji.xyz/gtwnrowlka.html

Py:   math.gcd(a, b)
来源：http://hz.nwbrower.top/gtucbkwyze.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yj20258888.top/gtyshrgkpi.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhengqikj.top/gtkmzpqiuz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.316326.xyz/gtcbtdpgnd.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.cashguo.top/gtnkhscegu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.zhoulong.xyz/gtfigxvvez.html

Ruby: a.gcd(b)
来源：http://hz.wangdashe.top/gttbxiwsku.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.meibo888.top/gtblyzedvv.html

[N06] 判断回文字符串
来源：http://hz.andypj.xyz/gtlwabcfeu.html

Py:   s == s[::-1]
来源：http://hz.dianchejie.cn/gtdsxxifih.html

PHP:  $s === strrev($s);
来源：http://hz.redwolf501.top/gtqgqhjteu.html

JS:   s === [...s].reverse().join("")
来源：http://hz.tianlin.xyz/gttbfioyld.html

TS:   s === [...s].reverse().join("")
来源：http://hz.xingfuxueyuan.xyz/gtdghklsjm.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jyoumei.cn/gtrmwrgrms.html

Go:   // 双指针从两端比较
来源：http://hz.zhijiandao.cn/gtbvzyyjtg.html

Ruby: s == s.reverse
来源：http://hz.ybcxt.top/gtlmhzouko.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.shzxlz.cn/gtwhuzwlym.html

[N07] 两数之和（返回下标）
来源：http://hz.jinqigufen.top/gtpfweldfs.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.shzxlz.cn/gtbetefwcw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.gzhubu.top/gtdhagamcx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.jlsjyb.cn/gtyxjjtyim.html

TS:   // 手写 Map<string, number>
来源：http://hz.xziqi.cn/gtnwllnzkw.html

Java: // 手写 HashMap
来源：http://hz.jinqigfzy.top/gtkedqebhh.html

Go:   // 手写 map[int]int
来源：http://hz.jinyuanbaomall.cn/gtojmyamls.html

Ruby: // 手写 Hash
来源：http://hz.316326.xyz/gtysynsvvi.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.sxryk.cn/gtgxekihmq.html

[N08] 生成全排列
来源：http://hz.cashguo.top/gtqgszveis.html

Py:   itertools.permutations(arr)
来源：http://hz.hywenlv.cn/gttqqhhqes.html

PHP:  // 手写递归交换
来源：http://hz.cqqwz.cn/gtmcukpuds.html

JS:   // 手写回溯递归
来源：http://hz.hfpthk.cn/gtjwlvdjlm.html

TS:   // 手写回溯递归
来源：http://hz.jinyuanbaomall.cn/gtveziowua.html

Java: // 手写回溯递归
来源：http://hz.pengpengdd.cyou/gtjxlizvsx.html

Go:   // 手写回溯递归
来源：http://hz.gaohongyu789.top/gtmnmouycd.html

Ruby: arr.permutation.to_a
来源：http://hz.yuanzhike.top/gtgrjkpapf.html

C#:   // 手写回溯递归
来源：http://hz.vqdsnc.cn/gtdpyglxru.html

[N09] 栈与队列
来源：http://hz.52xcode.cn/gtjmlaycrt.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yj20258888.top/gtvnkxzleu.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.fengsongda.top/gtzaknzoac.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.mhx1999.top/gtryaryfxc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yj202588.top/gtidfefhnm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yj20258888.top/gtngnpqvoy.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.bjfxy.top/gtywikjwgm.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.hongshengwenyu.top/gtfgugxzyz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.jianghu66.top/gtcphwqpwo.html

[N10] 链表节点定义
来源：http://hz.cheryme.top/gtvsfuisnh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.jyoumei.cn/gtmtbhuzqs.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.wangdashe.top/gtrbvdtjty.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.haohaochexian.top/gtltrtgacm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.shanyushiyangtech.top/gtuzkpwikg.html

Java: class Node { int v; Node next; }
来源：http://hz.cqqwz.cn/gtroofikur.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.chenjidiqi.icu/gtfojtawzf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.xingfuxueyuan.xyz/gtsuizqwdd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.chenzaomai.com/gtrdqtkwic.html

[N11] 二叉树中序遍历
来源：http://hz.shanyushiyangtech.top/gtypicxhai.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.aibaodan.cn/gtwortoers.html

PHP:  // 手写递归函数
来源：http://hz.hongshengwenyu.top/gtmvckofzq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.svipenyu.cn/gtqwlqwpeb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.cdnleiting.top/gtbrnvyxwv.html

Java: // 手写递归
来源：http://hz.iojbl.cn/gtggvtntqb.html

Go:   // 手写递归
来源：http://hz.pengpengdd.cyou/gtboqitvit.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.chenjidiqi.icu/gtwgrzzpeo.html

C#:   // 手写递归
来源：http://hz.zhixingplan.top/gtuwwplhaw.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.nwbrower.top/gteqrpixzp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.havefunace.top/gtkzscdmma.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.0kj1m.cn/gtjonvopfn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xylfe.cn/gtlqrskzza.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yvedp.cn/gtipqiyqbe.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yonumen.top/gtydymonqo.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.hysaishi.cn/gthgnjmlpa.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.yongpay.top/gtwvqykjbs.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ppjwa.cn/gtgudxeykd.html

================================================================================
来源：http://hz.fzhhl.top/gtuiydimqn.html

O. 并发与异步
来源：http://hz.birdmap.top/gttbnueyna.html

================================================================================
来源：http://hz.nanxinkj.top/gttwkzcxfn.html

[O01] 启动一个线程
来源：http://hz.ywan-chungtsiang.top/gtiyezrybz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.daxiang520.top/gtwrfglnvu.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.hnqzz.top/gtnpolpwce.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.vqdsnc.cn/gtuoproxhg.html

TS:   // 同 JS
来源：http://hz.xziqi.cn/gtjooiooai.html

Java: new Thread(() -> f()).start()
来源：http://hz.sufxvd.cn/gtnrotxrbv.html

Go:   go f()
来源：http://hz.jqgufenzy.top/gtvinzwwdj.html

Ruby: Thread.new { f }
来源：http://hz.yangfankeji.com/gtkcpribpv.html

C#:   Task.Run(() => F());
来源：http://hz.aibaodan.cn/gttzzkejzy.html

[O02] 使用线程池
来源：http://hz.tianlin.xyz/gtbjpjarlp.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.guowangkeji.top/gtiqajmvew.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.meibo888.top/gtzeglirzy.html

JS:   // worker_threads 线程池
来源：http://hz.jinqigfzy.top/gtiwsqolsh.html

TS:   // worker_threads 线程池
来源：http://hz.hfpthk.cn/gtirohidjh.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.wangdashe.top/gtwxdmqrsa.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.xziqi.cn/gtreopvyxp.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.cqqwz.cn/gtcblmchqe.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.hfpthk.cn/gtkhedfxng.html

[O03] 加锁保护共享数据
来源：http://hz.feifeiyinyue.top/gtjljsjnkc.html

Py:   with lock: shared += 1
来源：http://hz.pengpengdd.cyou/gtnkjyznvq.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.dashuyun.cn/gthoscmhmo.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.52xcode.cn/gtkxwzwqxs.html

TS:   // 同 JS
来源：http://hz.jyoumei.cn/gtdtlvrgjs.html

Java: synchronized (this) { shared++; }
来源：http://hz.zhaomingkeji.xyz/gtzfmnepef.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.cheryme.top/gtovhzcwxp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.pycfn.com/gtwynatjjb.html

C#:   lock (gate) { shared++; }
来源：http://hz.guannengcc.top/gtckjbrooi.html

[O04] 定义异步函数并等待
来源：http://hz.ydjk.org.cn/gtevrcaxly.html

Py:   async def f():⏎    await g()
来源：http://hz.yueranfly.top/gtrvxuoxqe.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.shanyushiyangtech.top/gtwkyiauka.html

JS:   async function f() { await g(); }
来源：http://hz.xziqi.cn/gtrqqeeqdl.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.xziqi.cn/gtmzhrytqg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.xuanzx.com/gtfllbhevx.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.gotoacloud.top/gtcanonfon.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.xuetiantiany.cn/gtckfyglyz.html

C#:   async Task F() { await G(); }
来源：http://hz.hywenlv.cn/gtwfxxeayp.html

[O05] 并发执行并等待全部完成
来源：http://hz.pengpengdd.cyou/gtueilgixq.html

Py:   asyncio.gather(*tasks)
来源：http://hz.tianlin.xyz/gtrhdjvbov.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.yj202588.top/gtfdlrlovd.html

JS:   await Promise.all(tasks)
来源：http://hz.dashuyun.cn/gthtbcoptu.html

TS:   await Promise.all(tasks)
来源：http://hz.shangyingyoupin.top/gtxdznbaga.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.cucudq.cn/gtqydsvhsj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.jinqigufen.top/gtmsyaoxnp.html

Ruby: threads.map(&:join)
来源：http://hz.nwbrower.top/gtwrfkdbmu.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.smart0.xyz/gtvnytsccu.html

[O06] 使用进程池
来源：http://hz.yonumen.top/gtlcnhypwp.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.redwolf501.top/gtymlchbwu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.zhaomingkeji.xyz/gtotyjdnto.html

JS:   // child_process / cluster 模块
来源：http://hz.52xcode.cn/gtdlgaremq.html

TS:   // child_process / cluster 模块
来源：http://hz.guannengcc.top/gticshfdyg.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.gzhubu.top/gtktkujabl.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.sxryk.cn/gtpaikvrhe.html

Ruby: // fork 块
来源：http://hz.daria6918.cn/gtfscswcjj.html

C#:   Parallel.For
来源：http://hz.chenjidiqi.icu/gtfyyrchxm.html

================================================================================
来源：http://hz.haohaochexian.top/gtqutpskpb.html

P. 常用工具函数
来源：http://hz.jlsjyb.cn/gtpvcrolep.html

================================================================================
来源：http://hz.jqgfzy.top/gtgijufhzq.html

[P01] 生成 UUID
来源：http://hz.yanxiufei.cn/gtxqrrbifa.html

Py:   str(uuid.uuid4())
来源：http://hz.ppjwa.cn/gtrgcwtpov.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yj20258888.top/gtoeosevgd.html

JS:   crypto.randomUUID()
来源：http://hz.kuanghao11.cn/gtavwveiwk.html

TS:   crypto.randomUUID()
来源：http://hz.ybcxt.top/gtktjgjfxi.html

Java: UUID.randomUUID().toString()
来源：http://hz.gotoacloud.top/gtayrpyklu.html

Go:   // 用 github.com/google/uuid
来源：http://hz.shanyushiyangtech.top/gtmakdkuvu.html

Ruby: SecureRandom.uuid
来源：http://hz.zdqjudy.top/gtzwkrsqkq.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.sufxvd.cn/gtyailtfdi.html

[P02] MD5 / SHA256 摘要
来源：http://hz.fengsongda.top/gttnhavfgu.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.zhiwuduotai.top/gtjjhggujb.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.xuanzx.com/gtndvhtigu.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.cqqwz.cn/gtmoselzjs.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.yuanzhike.top/gtdvnerobx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.guannengcc.top/gtdjzwzxck.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.jinyuanbaomall.cn/gthnmivsfq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.fzhhl.top/gtdsoggowa.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.zhixingplan.top/gtestfjqad.html

[P03] 生成短随机字符串
来源：http://hz.hongshengwenyu.top/gtnhdkscpa.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.shzxlz.cn/gtqofgwwqq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.cqqwz.cn/gtnkncvosq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hnqzz.top/gtnmfnsdlf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ivvv.top/gtqxiuojfm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yangfankeji.com/gtuuoltfpt.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.jqgfzy.top/gtgpycuozl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.hfpthk.cn/gtbphcryum.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.birdmap.top/gtgptetpjx.html

[P04] 求长度
来源：http://hz.fzhhl.top/gthslkzdwu.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.shanyushiyangtech.top/gtsbeqwogq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shuidangran.top/gtvrngsfvg.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hammf.cn/gtxrbddbwa.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.sxryk.cn/gtsxutonvn.html

Java: list.size();  map.size();  s.length()
来源：http://hz.yanxiufei.cn/gtmwccxmwg.html

Go:   len(arr);  len(m)
来源：http://hz.quarkkingdee.top/gtagetferr.html

Ruby: x.length;  x.size
来源：http://hz.bjfxy.top/gthgqywzkh.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.zhongyouzk.top/gtetsefzij.html

[P05] 判断两个对象内容是否相等
来源：http://hz.hfpthk.cn/gtfaneqdtv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.gogol.net.cn/gtuftifgmx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.smart0.xyz/gtnvjvqrro.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.shzxlz.cn/gtxurfewmp.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.chenjidiqi.icu/gtsshephxo.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.yueranfly.top/gtyyuptyzf.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.nanxuanxn.top/gttztapyos.html

Ruby: a == b
来源：http://hz.quarkkingdee.top/gtrvxqbjck.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.wangdashe.top/gtimuoskny.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.yj20258.top/gtfcndyfot.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.hywenlv.cn/gtyxfoefjd.html

PHP:  if (empty($x)) {}
来源：http://hz.cucudq.cn/gtsccgfcpy.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.shangyingyoupin.top/gtaiyissym.html

TS:   if (x == null) {}
来源：http://hz.daxiang520.top/gtngikvoot.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.ybcxt.top/gtemtslyuo.html

Go:   if x == nil {}
来源：http://hz.gogol.net.cn/gtcwofimzr.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.nwbrower.top/gttnjwazms.html

C#:   if (x is null) {}
来源：http://hz.shanyushiyangkeji.top/gtyykvswhh.html

[P07] 防抖与节流
来源：http://hz.nanxinkj.top/gtmrarnpzd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.ehwqpu.com/gtqzencqwy.html

PHP:  // 手写时间戳比较
来源：http://hz.shanyushiyangtech.top/gtrbykcskl.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cheryme.top/gttihekbox.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.aizwys.cn/gtsfittngo.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.ppjwa.cn/gtmufmfnmm.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.hnqzz.top/gttswvftmf.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.zhoulong.xyz/gtdqxyxgoy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.zhixingplan.top/gteotimmxf.html

[P08] 处理浮点精度问题
来源：http://hz.9152youxi.cn/gtadnlkhrw.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.ybcxt.top/gtmpcnlyex.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.c1oappe.top/gtpbqhxlpi.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.daria6918.cn/gtpezywtxi.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.shangyingyoupin.top/gtziqvmtos.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.quarkkingdee.top/gtpkiyfeth.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.zdqjudy.top/gthegxraxv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.tanke756.top/gtqxbakimm.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.chenlongwang.top/gtbkspbamn.html

================================================================================
来源：http://hz.smart0.xyz/gtmijbkehj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.hnxiangtu.top/gtmojnkwoe.html

================================================================================
来源：http://hz.zhixingplan.top/gtubhettpv.html

[Q01] 创建表
来源：http://hz.dianchejie.cn/gtfzhaerok.html

CREATE TABLE users (
来源：http://hz.havefunace.top/gtuioyjpjc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hysaishi.cn/gtzlxnnihk.html

name VARCHAR(50) NOT NULL,
来源：http://hz.zdqjudy.top/gtsuqhwzvm.html

email VARCHAR(100) UNIQUE,
来源：http://hz.yuxming.cn/gtqtvvqwhn.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.snrcjt.cn/gtwobmzfpx.html

);
来源：http://hz.sufxvd.cn/gtpkjaufab.html

[Q02] 创建带外键的表
来源：http://hz.chenzaomai.com/gtfeimdsoc.html

CREATE TABLE orders (
来源：http://hz.gzhubu.top/gtekuiccji.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.svipenyu.cn/gtuqcgexts.html

user_id INT NOT NULL,
来源：http://hz.fengsongda.top/gtcyawavxp.html

amount DECIMAL(10, 2),
来源：http://hz.tianlin.xyz/gtzidbkkvn.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.cucudq.cn/gthpaybomk.html

);
来源：http://hz.ppjwa.cn/gtiefqcxmn.html

[Q03] 增加列
来源：http://hz.pycfn.com/gtfequvufr.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.cucudq.cn/gtrddrmdzo.html

[Q04] 修改列类型
来源：http://hz.c1oappe.top/gtqwipcqos.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.c1oappe.top/gtqzlbtduv.html

[Q05] 重命名列
来源：http://hz.sweek.top/gtaqeckflj.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.jlsjyb.cn/gtgckaonna.html

[Q06] 删除列
来源：http://hz.hfpthk.cn/gteaoxmvvp.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.jqgfzy.top/gtgwgshrkh.html

[Q07] 删除表
来源：http://hz.chenjidiqi.icu/gtrfvxwiuw.html

DROP TABLE IF EXISTS orders;
来源：http://hz.jinqigufen.top/gtxsfobqxw.html

[Q08] 创建普通索引
来源：http://hz.zhiwuduotai.top/gtoqtubdys.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jinqigfzy.top/gtyxprijgk.html

[Q09] 创建唯一索引
来源：http://hz.cucudq.cn/gtqpfmacpc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.daria6918.cn/gtbvnilpfu.html

[Q10] 插入单行
来源：http://hz.dianchejie.cn/gtkcijvrgx.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.316326.xyz/gtywnfbcic.html

[Q11] 一次插入多行
来源：http://hz.hnxiangtu.top/gtqmmpncrr.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.ivvv.top/gttumnpccj.html

[Q12] 插入后取自增 ID
来源：http://hz.shzxlz.cn/gtwhfmcveh.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.shanyushiyangtech.top/gtdpeqxary.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.meibo888.top/gtpncgfkxf.html

[Q13] 忽略重复插入
来源：http://hz.316326.xyz/gtyollxdqs.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.cqqwz.cn/gtvwvcuyvj.html

[Q14] 存在则更新（upsert）
来源：http://hz.yueranfly.top/gtccwxeybd.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.gaohongyu789.top/gttdikihsi.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.zhengqikj.top/gtxnejmxmi.html

[Q15] 查询全部
来源：http://hz.0kj1m.cn/gtcyqvqwmq.html

SELECT * FROM users;
来源：http://hz.316326.xyz/gtcmocuarh.html

[Q16] 查询指定列
来源：http://hz.bjfxy.top/gtqtgibxml.html

SELECT id, name FROM users;
来源：http://hz.jinqigfzy.top/gtdeuvewuz.html

[Q17] 条件查询
来源：http://hz.ivvv.top/gtyqdrgrbs.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.xziqi.cn/gthnrptxkk.html

[Q18] 模糊匹配
来源：http://hz.0kj1m.cn/gtxlyikhic.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.0kj1m.cn/gttlbbcqvm.html

[Q19] 范围查询
来源：http://hz.meibo888.top/gtghqsyupt.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.vqdsnc.cn/gtrgdqhihw.html

[Q20] IN 列表
来源：http://hz.hammf.cn/gtpkxjtfmz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yongpay.top/gtaobshrbh.html

[Q21] 空值判断
来源：http://hz.gzhubu.top/gtkpmazqww.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.aizwys.cn/gtglfbctkh.html

[Q22] 排序
来源：http://hz.zhengqikj.top/gtpgtmacrj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.fzhhl.top/gtxhorloow.html

[Q23] 分页
来源：http://hz.shangyingyoupin.top/gtjgdwkvzj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.316326.xyz/gthvcpdext.html

[Q24] 去重
来源：http://hz.jyoumei.cn/gtjntsgeqa.html

SELECT DISTINCT city FROM users;
来源：http://hz.shangyingyoupin.top/gtjracfofw.html

[Q25] 只取前 N 条
来源：http://hz.xylfe.cn/gtsxvtuxjg.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.zdqjudy.top/gthkzelpdi.html

[Q26] 计数
来源：http://hz.guannengcc.top/gtnpqplyff.html

SELECT COUNT(*) FROM users;
来源：http://hz.nanxuanxn.top/gtjmoinwij.html

[Q27] 条件计数
来源：http://hz.ydzc1.top/gtopahwbhg.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.9152youxi.cn/gtvwvfkivx.html

[Q28] 求和与平均
来源：http://hz.shanyushiyangtech.top/gtxrvdnfol.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.svipenyu.cn/gtxpznikvd.html

[Q29] 最大最小值
来源：http://hz.fzhhl.top/gtssdshile.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.gotoacloud.top/gtaepffzbo.html

[Q30] 分组统计
来源：http://hz.jinghuilouyu.cn/gtkvnytech.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.bjfxy.top/gtvnbvbrlg.html

[Q31] 分组后过滤
来源：http://hz.sxryk.cn/gtnsyjqdhu.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.vqdsnc.cn/gttkegifql.html

[Q32] 分组拼接字符串
来源：http://hz.hnxiangtu.top/gtiziplftf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.cqqwz.cn/gtwsoqxyii.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.zdqjudy.top/gtfmqjotam.html


<!-- 参考信息 -->