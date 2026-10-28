代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.gogol.net.cn/gtpiwzpvhe.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.dianchejie.cn/gtwyolvxgp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.chenzaomai.com/gtbupzwipt.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ppjwa.cn/gtcfkqijct.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.ivvv.top/gtdumdvmpc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.zycfv.cn/gtbbhnlusk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yj20258888.top/gtgjkiktul.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.shanyushiyangtech.top/gtyubeedfm.html

[N05] 最大公约数
来源：http://hz.gaohongyu789.top/gtxgzmurdf.html

Py:   math.gcd(a, b)
来源：http://hz.chenzaomai.com/gtrgzxotua.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.hammf.cn/gtsuilfxvx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.cashguo.top/gtevrqmmxd.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.iojbl.cn/gtathmpjyd.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.yanxiufei.cn/gtnzhvepue.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.guannengcc.top/gtbshvyqds.html

Ruby: a.gcd(b)
来源：http://hz.jianghu66.top/gtdtlrwgli.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jinyuanbaomall.cn/gtrmecxaej.html

[N06] 判断回文字符串
来源：http://hz.xuetiantiany.cn/gtnuaqrzus.html

Py:   s == s[::-1]
来源：http://hz.ivvv.top/gtywrqkmfd.html

PHP:  $s === strrev($s);
来源：http://hz.shangyingyoupin.top/gtrdiygvou.html

JS:   s === [...s].reverse().join("")
来源：http://hz.ppjwa.cn/gtffldhbyr.html

TS:   s === [...s].reverse().join("")
来源：http://hz.quarkkingdee.top/gtdfkmujlo.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.yangfankeji.com/gthxnyrgyc.html

Go:   // 双指针从两端比较
来源：http://hz.aizwys.cn/gtomrbwviq.html

Ruby: s == s.reverse
来源：http://hz.daxiang520.top/gtqxpzuhof.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.chenjidiqi.icu/gtclmcqnfe.html

[N07] 两数之和（返回下标）
来源：http://hz.ivvv.top/gtgwmlurug.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.ybcxt.top/gtqnqpwtna.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.cheryme.top/gtwhhuognz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.cqqwz.cn/gtecvuuwtg.html

TS:   // 手写 Map<string, number>
来源：http://hz.zycfv.cn/gtyczsstvh.html

Java: // 手写 HashMap
来源：http://hz.ivvv.top/gtjaavfkpy.html

Go:   // 手写 map[int]int
来源：http://hz.xingfuxueyuan.xyz/gtqgjnmxvp.html

Ruby: // 手写 Hash
来源：http://hz.smart0.xyz/gtsrfzlhes.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.daria6918.cn/gteedlzgtr.html

[N08] 生成全排列
来源：http://hz.zhaomingkeji.xyz/gtbtloqvxr.html

Py:   itertools.permutations(arr)
来源：http://hz.jlsjyb.cn/gtpbmxzdgg.html

PHP:  // 手写递归交换
来源：http://hz.316326.xyz/gtvwyaypfz.html

JS:   // 手写回溯递归
来源：http://hz.hammf.cn/gtpeteiqjq.html

TS:   // 手写回溯递归
来源：http://hz.ehwqpu.com/gtgeodplgr.html

Java: // 手写回溯递归
来源：http://hz.nwbrower.top/gtlejsshve.html

Go:   // 手写回溯递归
来源：http://hz.cdnleiting.top/gtysjtlvtm.html

Ruby: arr.permutation.to_a
来源：http://hz.jyoumei.cn/gtwokecqam.html

C#:   // 手写回溯递归
来源：http://hz.zhoulong.xyz/gtibbmarvz.html

[N09] 栈与队列
来源：http://hz.jqgufenzy.top/gtirbbhzbv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.316326.xyz/gtleqycogk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.jianghu66.top/gtndhdkabq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yuxming.cn/gtucxizlqf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.sweek.top/gtupmyttxx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.guannengcc.top/gthpamqmow.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.ywan-chungtsiang.top/gtndtcaooy.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.shangyingyoupin.top/gthfkwxcxw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.hnxiangtu.top/gtywjrrgzn.html

[N10] 链表节点定义
来源：http://hz.hnqzz.top/gtjdnslgph.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yuanzhike.top/gtpfewowob.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.gotoacloud.top/gtcychalve.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.ywan-chungtsiang.top/gthqnqcfgs.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.zhongyouzk.top/gtxhpvqgwb.html

Java: class Node { int v; Node next; }
来源：http://hz.hongshengwenyu.top/gtpfuyqawf.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.sweek.top/gtcuilivqa.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.xuanzx.com/gttqnfpkoc.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.9152youxi.cn/gtriixiask.html

[N11] 二叉树中序遍历
来源：http://hz.aizwys.cn/gthhlorslh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.hammf.cn/gtjjwjbzex.html

PHP:  // 手写递归函数
来源：http://hz.yangfankeji.com/gtruxrnihv.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yueranfly.top/gtusswsfyh.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.shuidangran.top/gtacwkwqdn.html

Java: // 手写递归
来源：http://hz.jyoumei.cn/gtczipaico.html

Go:   // 手写递归
来源：http://hz.wangdashe.top/gtemhucxhy.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.yueranfly.top/gtgvonhqgc.html

C#:   // 手写递归
来源：http://hz.havefunace.top/gtqeangyls.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.cucudq.cn/gthzhhyasm.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.cqqwz.cn/gtdgfegiks.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.mhx1999.top/gtkxdngqmr.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhongyouzk.top/gtczethovu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yj20258.top/gtmwabvvsu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hfpthk.cn/gtrdiuwpfv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.pengpengdd.cyou/gtaatyetct.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.hnxiangtu.top/gttszchlqx.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.pengpengdd.cyou/gtsldecmkw.html

================================================================================
来源：http://hz.0kj1m.cn/gtjqofgook.html

O. 并发与异步
来源：http://hz.0kj1m.cn/gtxasfafkg.html

================================================================================
来源：http://hz.jqgufenzy.top/gtmyojzszl.html

[O01] 启动一个线程
来源：http://hz.jianghu66.top/gtwtwrpyck.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.pycfn.com/gtglygyoth.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.hongshengwenyu.top/gtfyzjcvsw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.yueranfly.top/gtjbikbcbu.html

TS:   // 同 JS
来源：http://hz.zhoulong.xyz/gtzthupylt.html

Java: new Thread(() -> f()).start()
来源：http://hz.zhiwuduotai.top/gtbcesedck.html

Go:   go f()
来源：http://hz.ydzc1.top/gtqbmdiggb.html

Ruby: Thread.new { f }
来源：http://hz.xinyue.icu/gtsufwoyjn.html

C#:   Task.Run(() => F());
来源：http://hz.wangshuangyany.cn/gtsktrnjab.html

[O02] 使用线程池
来源：http://hz.nanxuanxn.top/gttysowxft.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.9152youxi.cn/gtiytkwmbs.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.andypj.xyz/gtzrzmsqia.html

JS:   // worker_threads 线程池
来源：http://hz.yj20258.top/gtqslcokqr.html

TS:   // worker_threads 线程池
来源：http://hz.sufxvd.cn/gtgaaunzle.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yonumen.top/gtwywfqswy.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yonumen.top/gtdxradyll.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yongpay.top/gtihwhrbdo.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.yuxming.cn/gtyocsqald.html

[O03] 加锁保护共享数据
来源：http://hz.cucudq.cn/gtgoxdimer.html

Py:   with lock: shared += 1
来源：http://hz.jinqigfzy.top/gtrytiiymj.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.jyoumei.cn/gtxtajncfl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.xuetiantiany.cn/gtqszegavr.html

TS:   // 同 JS
来源：http://hz.9152youxi.cn/gtzhevrvet.html

Java: synchronized (this) { shared++; }
来源：http://hz.tian-w.cn/gtadlnkhxh.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.mhx1999.top/gtafautdtd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.svipenyu.cn/gtnaogsiyy.html

C#:   lock (gate) { shared++; }
来源：http://hz.yueranfly.top/gtmhiqntdt.html

[O04] 定义异步函数并等待
来源：http://hz.sxryk.cn/gtkcnmbxdi.html

Py:   async def f():⏎    await g()
来源：http://hz.jinqigufen.top/gthfytwddm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.yanxiufei.cn/gthfgogznc.html

JS:   async function f() { await g(); }
来源：http://hz.chenjidiqi.icu/gtlokcjmqk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.gotoacloud.top/gthnddzuvs.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.gogol.net.cn/gtmacnqpjf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.yangfankeji.com/gtajfoeqov.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.xuanzx.com/gtypjkanai.html

C#:   async Task F() { await G(); }
来源：http://hz.wangdashe.top/gtwrpgrqdd.html

[O05] 并发执行并等待全部完成
来源：http://hz.hfpthk.cn/gtgbmzcppt.html

Py:   asyncio.gather(*tasks)
来源：http://hz.aizwys.cn/gtlwppvqyc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.xuetiantiany.cn/gtulnyijze.html

JS:   await Promise.all(tasks)
来源：http://hz.jlsjyb.cn/gtrhrapyov.html

TS:   await Promise.all(tasks)
来源：http://hz.yueranfly.top/gtmdvcdqji.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.svipenyu.cn/gthiwkluye.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.kuanghao11.cn/gtktrqaddy.html

Ruby: threads.map(&:join)
来源：http://hz.sxryk.cn/gtekayswyi.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yuanzhike.top/gtajmrxoab.html

[O06] 使用进程池
来源：http://hz.cheryme.top/gtlpfdwlem.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.zhengqikj.top/gtkexkjkji.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.daria6918.cn/gtpvkyirmm.html

JS:   // child_process / cluster 模块
来源：http://hz.yangfankeji.com/gtrnlbibcp.html

TS:   // child_process / cluster 模块
来源：http://hz.xuetiantiany.cn/gtrltevkfh.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yj202588.top/gtjmuevegk.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.hongshengwenyu.top/gtraovdzlb.html

Ruby: // fork 块
来源：http://hz.quarkkingdee.top/gtwokispgt.html

C#:   Parallel.For
来源：http://hz.andypj.xyz/gtalnzkxet.html

================================================================================
来源：http://hz.andypj.xyz/gteqkgvrtq.html

P. 常用工具函数
来源：http://hz.52xcode.cn/gtyzulcemn.html

================================================================================
来源：http://hz.xuanzx.com/gtnofwulyo.html

[P01] 生成 UUID
来源：http://hz.ppjwa.cn/gtrdmlkeex.html

Py:   str(uuid.uuid4())
来源：http://hz.ppjwa.cn/gtqqdkrcas.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.iojbl.cn/gtwoelhjft.html

JS:   crypto.randomUUID()
来源：http://hz.c1oappe.top/gtcwvjgkwl.html

TS:   crypto.randomUUID()
来源：http://hz.haohaochexian.top/gthxpgpzor.html

Java: UUID.randomUUID().toString()
来源：http://hz.vqdsnc.cn/gtkghlgjbg.html

Go:   // 用 github.com/google/uuid
来源：http://hz.fzhhl.top/gtwagnduio.html

Ruby: SecureRandom.uuid
来源：http://hz.zdqjudy.top/gtyvbfshck.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.cucudq.cn/gtqtzusfzl.html

[P02] MD5 / SHA256 摘要
来源：http://hz.yangfankeji.com/gtyxlmxmio.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.bjfxy.top/gtpdvqsumg.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.jinqigfzy.top/gtpgimlwon.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.sysykeji.top/gtxbmsmuel.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.cheryme.top/gtrpfvzdnm.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.zhongyouzk.top/gtmhbuhwcc.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.iojbl.cn/gtovzgyehl.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.gogol.net.cn/gtvurlqdry.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.smart0.xyz/gtrzspvrrv.html

[P03] 生成短随机字符串
来源：http://hz.cashguo.top/gtcyuzzhpd.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jqgufenzy.top/gtdcfstkoa.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.jyoumei.cn/gtvhomginc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hnqzz.top/gtkiemjgis.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.svipenyu.cn/gtqfnsipsn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.zhaomingkeji.xyz/gtyqjkgbme.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.xuetiantiany.cn/gtpeycfpfs.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.svipenyu.cn/gttshdborf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jiagoushi.top/gtargblncm.html

[P04] 求长度
来源：http://hz.aibaodan.cn/gthiebptrc.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.9152youxi.cn/gtvalofwyj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.nanxinkj.top/gtsinvmvjk.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yj20258.top/gtynbuycel.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ehwqpu.com/gtcbaeigmd.html

Java: list.size();  map.size();  s.length()
来源：http://hz.iojbl.cn/gtqoalmfmq.html

Go:   len(arr);  len(m)
来源：http://hz.ppjwa.cn/gtuvmqcxum.html

Ruby: x.length;  x.size
来源：http://hz.yj20258.top/gtjzwflfph.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.kuanghao11.cn/gttdxunhum.html

[P05] 判断两个对象内容是否相等
来源：http://hz.c1oappe.top/gtcyqekdtq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.tian-w.cn/gtfssspxkl.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.xylfe.cn/gtehbjduwf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.jinghuilouyu.cn/gtqdneedmp.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jqgfzy.top/gtpduxchpn.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.hammf.cn/gtiezkzcie.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.nanxuanxn.top/gtmgtxazuf.html

Ruby: a == b
来源：http://hz.hongshengwenyu.top/gtsyxoevwk.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.dianchejie.cn/gtxayjdtun.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.bjfxy.top/gtgloaidmk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.chenzaomai.com/gtxxehmbrx.html

PHP:  if (empty($x)) {}
来源：http://hz.xinyue.icu/gtmpgglyqz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.chenlongwang.top/gtokqztyun.html

TS:   if (x == null) {}
来源：http://hz.hnqzz.top/gtgtwoxnly.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.c1oappe.top/gtgnynnljh.html

Go:   if x == nil {}
来源：http://hz.zhixingplan.top/gttossegly.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.andypj.xyz/gttlfnczsu.html

C#:   if (x is null) {}
来源：http://hz.nanxinkj.top/gtcnigfrdm.html

[P07] 防抖与节流
来源：http://hz.nwbrower.top/gtqpptwysh.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.hywenlv.cn/gtgcfmyizm.html

PHP:  // 手写时间戳比较
来源：http://hz.gogol.net.cn/gtuhdfqonl.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.gaohongyu789.top/gtificislr.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.guannengcc.top/gtvgmmvkhy.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.fengsongda.top/gtannfhsro.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.xylfe.cn/gtvhcvxgey.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yuxming.cn/gtxwlzjjaa.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.pycfn.com/gtxkckzjxo.html

[P08] 处理浮点精度问题
来源：http://hz.316326.xyz/gtkuouxsql.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.havefunace.top/gtqadbjswv.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.pengpengdd.cyou/gtnggatipi.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.snrcjt.cn/gttwfplhlf.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.zhaomingkeji.xyz/gtlnuoqrwv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.ydzc1.top/gtcdwfnrhx.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.ywan-chungtsiang.top/gtmxhrazmu.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.tianlin.xyz/gtywxdmtwt.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.nanxuanxn.top/gtyuqkjuen.html

================================================================================
来源：http://hz.chenlongwang.top/gtqphyoona.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.hnqzz.top/gtfwczppvx.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gttnslvkvy.html

[Q01] 创建表
来源：http://hz.cucudq.cn/gthsklwfjf.html

CREATE TABLE users (
来源：http://hz.havefunace.top/gtvdacwzrt.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.cucudq.cn/gtpsjlwhjy.html

name VARCHAR(50) NOT NULL,
来源：http://hz.yonumen.top/gtqajzgxbi.html

email VARCHAR(100) UNIQUE,
来源：http://hz.gzhubu.top/gtvykvxmfl.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.nanxuanxn.top/gtsibtxgrn.html

);
来源：http://hz.xinyue.icu/gtiqwhyvrp.html

[Q02] 创建带外键的表
来源：http://hz.shanyushiyangtech.top/gtgstxmqdr.html

CREATE TABLE orders (
来源：http://hz.shanyushiyangtech.top/gtuedzinpx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.vqdsnc.cn/gtvucvtjop.html

user_id INT NOT NULL,
来源：http://hz.snrcjt.cn/gtasrodyxe.html

amount DECIMAL(10, 2),
来源：http://hz.gzhubu.top/gtiehbthuu.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.shanyushiyangtech.top/gtvdfxzpyh.html

);
来源：http://hz.wangdashe.top/gtxscevevi.html

[Q03] 增加列
来源：http://hz.pycfn.com/gtplkagrpg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.chenjidiqi.icu/gtzosvdtul.html

[Q04] 修改列类型
来源：http://hz.fzhhl.top/gtkidwsdbp.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.jinyuanbaomall.cn/gtxgrspayf.html

[Q05] 重命名列
来源：http://hz.cucudq.cn/gthdodnzwm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.nanxinkj.top/gthlwazbzg.html

[Q06] 删除列
来源：http://hz.fzhhl.top/gtkisswbfm.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.jinyuanbaomall.cn/gtagautpzs.html

[Q07] 删除表
来源：http://hz.zhoulong.xyz/gteqlmliui.html

DROP TABLE IF EXISTS orders;
来源：http://hz.hnxiangtu.top/gtxflcthgd.html

[Q08] 创建普通索引
来源：http://hz.shanyushiyangkeji.top/gtbqnhpabb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.9152youxi.cn/gtgknixhis.html

[Q09] 创建唯一索引
来源：http://hz.kuanghao11.cn/gtavsqwaex.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.ivvv.top/gtpbhhphev.html

[Q10] 插入单行
来源：http://hz.xuanzx.com/gtuuelgqap.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.yangfankeji.com/gttbofremx.html

[Q11] 一次插入多行
来源：http://hz.cucudq.cn/gtdccvelyn.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.redwolf501.top/gtvtadvyix.html

[Q12] 插入后取自增 ID
来源：http://hz.hnqzz.top/gtjfxnsvty.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.ppjwa.cn/gtmfzffkwv.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.jinyuanbaomall.cn/gtgfsitqpu.html

[Q13] 忽略重复插入
来源：http://hz.jqgfzy.top/gtcowkvrou.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.quarkkingdee.top/gtpemqbpay.html

[Q14] 存在则更新（upsert）
来源：http://hz.meibo888.top/gtjibktwsg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.wangdashe.top/gttgyvzppy.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.jiagoushi.top/gtebodnsly.html

[Q15] 查询全部
来源：http://hz.fzhhl.top/gtgqntldbl.html

SELECT * FROM users;
来源：http://hz.yvedp.cn/gtwparfovy.html

[Q16] 查询指定列
来源：http://hz.chenjidiqi.icu/gtyurnyvqu.html

SELECT id, name FROM users;
来源：http://hz.chenlongwang.top/gtxuknyyuz.html

[Q17] 条件查询
来源：http://hz.kuanghao11.cn/gtpolrmunm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.jqgfzy.top/gtgtucozyn.html

[Q18] 模糊匹配
来源：http://hz.zhixingplan.top/gtzzrbdowg.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.316326.xyz/gtlnzzyskj.html

[Q19] 范围查询
来源：http://hz.wangdashe.top/gtkmijlqwn.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.zhiwuduotai.top/gtkwqhguik.html

[Q20] IN 列表
来源：http://hz.hfpthk.cn/gtwhwygnkr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.pycfn.com/gtsgfxlclm.html

[Q21] 空值判断
来源：http://hz.havefunace.top/gtrbuvoufh.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.nwbrower.top/gtymwidnuu.html

[Q22] 排序
来源：http://hz.jinyuanbaomall.cn/gtlhwkkrtw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.dashuyun.cn/gtqwvleviq.html

[Q23] 分页
来源：http://hz.nanxuanxn.top/gtndrysozx.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.zhongyouzk.top/gtgshlbwcf.html

[Q24] 去重
来源：http://hz.jqgufenzy.top/gtylvfcyxu.html

SELECT DISTINCT city FROM users;
来源：http://hz.gotoacloud.top/gttcvfpexk.html

[Q25] 只取前 N 条
来源：http://hz.xuetiantiany.cn/gtsscmqega.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.gzhubu.top/gtgwrmoybc.html

[Q26] 计数
来源：http://hz.ehwqpu.com/gtsipkddst.html

SELECT COUNT(*) FROM users;
来源：http://hz.gotoacloud.top/gteorerktm.html

[Q27] 条件计数
来源：http://hz.nwbrower.top/gthzhegrgf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.zhongyouzk.top/gtcjbypgsf.html

[Q28] 求和与平均
来源：http://hz.zhaomingkeji.xyz/gtczrmlfii.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.hnqzz.top/gtfjuyjyhq.html

[Q29] 最大最小值
来源：http://hz.zhengqikj.top/gtegytxqce.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.haohaochexian.top/gtljdqpiga.html

[Q30] 分组统计
来源：http://hz.daxiang520.top/gtbnmntinw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.jinyuanbaomall.cn/gtmwbxwkcy.html

[Q31] 分组后过滤
来源：http://hz.zhijiandao.cn/gtkxehognr.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.0kj1m.cn/gtsomibvpz.html

[Q32] 分组拼接字符串
来源：http://hz.redwolf501.top/gtpwniwrlr.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.snrcjt.cn/gtybwdtgeo.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yuanzhike.top/gtaceacprm.html

[Q33] 多列分组
来源：http://hz.9152youxi.cn/gtbojfckoy.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.jinghuilouyu.cn/gtpkagpmev.html

[Q34] 每组取第一条
来源：http://hz.yvedp.cn/gtzzyrpmrm.html

SELECT * FROM (
来源：http://hz.zhongyouzk.top/gtvagjfmgy.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.yanxiufei.cn/gtsafnoyok.html

) t WHERE rn = 1;
来源：http://hz.meibo888.top/gtjeikmzqh.html

[Q35] 内连接
来源：http://hz.cqqwz.cn/gtnqdxuagp.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.cqqwz.cn/gtdjxakpgc.html


<!-- 参考信息 -->