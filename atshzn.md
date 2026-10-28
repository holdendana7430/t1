代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.meibo888.top/gteiedqkpl.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.smart0.xyz/gtycyasbow.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.jinqigufen.top/gtebhulgdd.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.redwolf501.top/gtgtqbhlia.html

[N05] 最大公约数
来源：http://hz.iojbl.cn/gteylcsrvx.html

Py:   math.gcd(a, b)
来源：http://hz.shuidangran.top/gtlniteqjj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.havefunace.top/gtsjovgibz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ivvv.top/gtlhfpsnli.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yj20258.top/gtdjjknfro.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.fengsongda.top/gtyhidmrhn.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.zhiwuduotai.top/gttrunscco.html

Ruby: a.gcd(b)
来源：http://hz.aizwys.cn/gtbgwxuicz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.chenjidiqi.icu/gtlreluaws.html

[N06] 判断回文字符串
来源：http://hz.52xcode.cn/gtftdrqnhd.html

Py:   s == s[::-1]
来源：http://hz.jiagoushi.top/gtoaccjece.html

PHP:  $s === strrev($s);
来源：http://hz.zycfv.cn/gttfubkmrf.html

JS:   s === [...s].reverse().join("")
来源：http://hz.svipenyu.cn/gtpxretqbr.html

TS:   s === [...s].reverse().join("")
来源：http://hz.gaohongyu789.top/gtucmwpwvi.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.yuanzhike.top/gtemuqcgat.html

Go:   // 双指针从两端比较
来源：http://hz.zhixingplan.top/gtdjovbcvo.html

Ruby: s == s.reverse
来源：http://hz.chenjidiqi.icu/gtzpokvdwt.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.gotoacloud.top/gtwbuxdumx.html

[N07] 两数之和（返回下标）
来源：http://hz.zhijiandao.cn/gtioiugtaj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.cdnleiting.top/gtamedbjtk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.zhaomingkeji.xyz/gtsrzjdviz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.shanyushiyangkeji.top/gtuuqsughf.html

TS:   // 手写 Map<string, number>
来源：http://hz.zhixingplan.top/gtmzpljrxm.html

Java: // 手写 HashMap
来源：http://hz.jqgufenzy.top/gtzvqwbzxl.html

Go:   // 手写 map[int]int
来源：http://hz.snrcjt.cn/gtxwfpevue.html

Ruby: // 手写 Hash
来源：http://hz.sxryk.cn/gtqhehxxvr.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.cdnleiting.top/gtnhhulxfp.html

[N08] 生成全排列
来源：http://hz.hammf.cn/gtwdqvthpx.html

Py:   itertools.permutations(arr)
来源：http://hz.daria6918.cn/gtwblbgroo.html

PHP:  // 手写递归交换
来源：http://hz.wangshuangyany.cn/gtqczfsnwz.html

JS:   // 手写回溯递归
来源：http://hz.9152youxi.cn/gtkvjzavot.html

TS:   // 手写回溯递归
来源：http://hz.gotoacloud.top/gtawykkvyp.html

Java: // 手写回溯递归
来源：http://hz.jqgufenzy.top/gtviyyonup.html

Go:   // 手写回溯递归
来源：http://hz.wangdashe.top/gtfrvrpbct.html

Ruby: arr.permutation.to_a
来源：http://hz.sxryk.cn/gtihwjlqum.html

C#:   // 手写回溯递归
来源：http://hz.xinyue.icu/gtsnycobgt.html

[N09] 栈与队列
来源：http://hz.yj20258888.top/gtjmorsdqx.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yuanzhike.top/gtqgievsaa.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.xuetiantiany.cn/gtbcylvntx.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.dianchejie.cn/gtuvxonuwg.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.fzhhl.top/gtzzdejixy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.ydjk.org.cn/gtsayndjgn.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.jinyuanbaomall.cn/gtcfnjgcgo.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.svipenyu.cn/gtvkbrmaph.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.jinyuanbaomall.cn/gtcfkxnogj.html

[N10] 链表节点定义
来源：http://hz.guowangkeji.top/gtuqgbnzbn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.jinyuanbaomall.cn/gtzqpligzd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.sweek.top/gtwmlatgiv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.hammf.cn/gtragcichj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.cucudq.cn/gtimwvkqvl.html

Java: class Node { int v; Node next; }
来源：http://hz.c1oappe.top/gtkmclwtnu.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.redwolf501.top/gtpmicdfvb.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.cucudq.cn/gthclsduqh.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yanxiufei.cn/gtorwdkzcr.html

[N11] 二叉树中序遍历
来源：http://hz.wangdashe.top/gtmkyhyznp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.xziqi.cn/gtsnrbdyxi.html

PHP:  // 手写递归函数
来源：http://hz.gotoacloud.top/gtnrlmjmgv.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.gzhubu.top/gtvvldbcok.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ivvv.top/gtyjccsvjj.html

Java: // 手写递归
来源：http://hz.jinqigufen.top/gthultphzn.html

Go:   // 手写递归
来源：http://hz.daxiang520.top/gtrnazwwtj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.hammf.cn/gtghcchjog.html

C#:   // 手写递归
来源：http://hz.daria6918.cn/gtdanrdajn.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.tanke756.top/gtvnahtlbr.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.316326.xyz/gtjytqnvek.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.havefunace.top/gtuzjnhwwl.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.feifeiyinyue.top/gthrhnuyns.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.tanke756.top/gtddqgqghs.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.pengpengdd.cyou/gtpzvflbhi.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.316326.xyz/gtlluqopye.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.nwbrower.top/gtkpxkgbkw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.iojbl.cn/gtrusyqjho.html

================================================================================
来源：http://hz.jinqigfzy.top/gtiavodjcw.html

O. 并发与异步
来源：http://hz.shanyushiyangtech.top/gtjjlcrisl.html

================================================================================
来源：http://hz.snrcjt.cn/gtjcbpnqbi.html

[O01] 启动一个线程
来源：http://hz.jlsjyb.cn/gtsejlbsmr.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.jyoumei.cn/gttgjddtpa.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.tianlin.xyz/gtmyhbmwvt.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.yonumen.top/gtqbcxcpyf.html

TS:   // 同 JS
来源：http://hz.zhengqikj.top/gtsvkqpaey.html

Java: new Thread(() -> f()).start()
来源：http://hz.hnxiangtu.top/gtxpbayypg.html

Go:   go f()
来源：http://hz.jqgufenzy.top/gtjcgblrfq.html

Ruby: Thread.new { f }
来源：http://hz.jinyuanbaomall.cn/gtpjjagegt.html

C#:   Task.Run(() => F());
来源：http://hz.xingfuxueyuan.xyz/gtrnewkdfw.html

[O02] 使用线程池
来源：http://hz.tian-w.cn/gtqaiklrdd.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.redwolf501.top/gtrcfrylau.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.sysykeji.top/gtsstkrxtf.html

JS:   // worker_threads 线程池
来源：http://hz.jinqigfzy.top/gtkltibqrt.html

TS:   // worker_threads 线程池
来源：http://hz.dianchejie.cn/gtzutknspv.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.hfpthk.cn/gtobphiekd.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yuanzhike.top/gtisnsrvel.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yj20258.top/gtrzilcjsl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.aibaodan.cn/gtcswlyjim.html

[O03] 加锁保护共享数据
来源：http://hz.guowangkeji.top/gtapycxrmd.html

Py:   with lock: shared += 1
来源：http://hz.aibaodan.cn/gtbpsfpsie.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.shanyushiyangkeji.top/gterqhobnd.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.jinyuanbaomall.cn/gtvlavqqrw.html

TS:   // 同 JS
来源：http://hz.zhongyouzk.top/gtkqmocksl.html

Java: synchronized (this) { shared++; }
来源：http://hz.zhiwuduotai.top/gtiirkzyqs.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.xuetiantiany.cn/gtpuneupbo.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jinghuilouyu.cn/gtyxfflkhf.html

C#:   lock (gate) { shared++; }
来源：http://hz.snrcjt.cn/gthkgwhcam.html

[O04] 定义异步函数并等待
来源：http://hz.yvedp.cn/gtrouhiczl.html

Py:   async def f():⏎    await g()
来源：http://hz.zhaomingkeji.xyz/gtsysobddm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.pycfn.com/gtkfwkabpj.html

JS:   async function f() { await g(); }
来源：http://hz.sufxvd.cn/gthvrnezbz.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yj20258.top/gtybcrbmat.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.jinqigufen.top/gtkovjcerf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.c1oappe.top/gtdsohspuz.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yj20258888.top/gtjddoqpiq.html

C#:   async Task F() { await G(); }
来源：http://hz.xuetiantiany.cn/gttlorrnea.html

[O05] 并发执行并等待全部完成
来源：http://hz.yanxiufei.cn/gtnwujgjmi.html

Py:   asyncio.gather(*tasks)
来源：http://hz.chenjidiqi.icu/gtseljkxpk.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.aizwys.cn/gtmakzagsl.html

JS:   await Promise.all(tasks)
来源：http://hz.redwolf501.top/gtxdcdycoi.html

TS:   await Promise.all(tasks)
来源：http://hz.cheryme.top/gtqrcbrmca.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.cucudq.cn/gtzirbrlfg.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.316326.xyz/gtfsstrrjz.html

Ruby: threads.map(&:join)
来源：http://hz.jinghuilouyu.cn/gtiskfnsbd.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.tian-w.cn/gtcgukdfue.html

[O06] 使用进程池
来源：http://hz.havefunace.top/gtysjkwfwh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.ybcxt.top/gtfuftmpfr.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.yongpay.top/gtrhvtgokt.html

JS:   // child_process / cluster 模块
来源：http://hz.ydzc1.top/gtpmmnvhue.html

TS:   // child_process / cluster 模块
来源：http://hz.cashguo.top/gtesmccckm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.xuanzx.com/gtvopzrjbo.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.hnqzz.top/gtzimlxuaj.html

Ruby: // fork 块
来源：http://hz.havefunace.top/gtcdxehmyi.html

C#:   Parallel.For
来源：http://hz.tianlin.xyz/gtqvrzhxof.html

================================================================================
来源：http://hz.yueranfly.top/gtiskmbktx.html

P. 常用工具函数
来源：http://hz.birdmap.top/gtjoeefqyd.html

================================================================================
来源：http://hz.quarkkingdee.top/gtqhrgauqa.html

[P01] 生成 UUID
来源：http://hz.yj20258888.top/gtzeukqxtk.html

Py:   str(uuid.uuid4())
来源：http://hz.sufxvd.cn/gtvymgjhey.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.gaohongyu789.top/gtiifofgdw.html

JS:   crypto.randomUUID()
来源：http://hz.smart0.xyz/gtlmbvkidk.html

TS:   crypto.randomUUID()
来源：http://hz.nanxinkj.top/gtbljiapic.html

Java: UUID.randomUUID().toString()
来源：http://hz.gzhubu.top/gtvgzxqsof.html

Go:   // 用 github.com/google/uuid
来源：http://hz.daria6918.cn/gtmqaupmzv.html

Ruby: SecureRandom.uuid
来源：http://hz.mhx1999.top/gtnvfmgxry.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.0kj1m.cn/gtgyhpfhuk.html

[P02] MD5 / SHA256 摘要
来源：http://hz.jianghu66.top/gtkecwkuqh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.yanxiufei.cn/gtzhqbgwnz.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.gotoacloud.top/gtcvdvqrkm.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.zhiwuduotai.top/gtekhncupr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.zhixingplan.top/gtrcgcunbr.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.ywan-chungtsiang.top/gtcsyvsqxq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.shzxlz.cn/gtkwuhiyau.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.hammf.cn/gtfmhtiuhl.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yueranfly.top/gtikdmyyax.html

[P03] 生成短随机字符串
来源：http://hz.yonumen.top/gtcntwxdrj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.shanyushiyangkeji.top/gtlhjfegjo.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.ivvv.top/gtebzzuldy.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jlsjyb.cn/gtjpqqntkz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yueranfly.top/gtsfixqgaq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jlsjyb.cn/gtiruaupmh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yanxiufei.cn/gthmbznsax.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.ybcxt.top/gtcwpbvmxu.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.yj20258.top/gtgvdivnhw.html

[P04] 求长度
来源：http://hz.c1oappe.top/gtulqjxijn.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.sufxvd.cn/gtbhhfvskf.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.9152youxi.cn/gtfpkasimh.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.birdmap.top/gtmycogcuk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yuxming.cn/gtjiuyilld.html

Java: list.size();  map.size();  s.length()
来源：http://hz.shuidangran.top/gtfhenkjhz.html

Go:   len(arr);  len(m)
来源：http://hz.redwolf501.top/gtoxaplmrp.html

Ruby: x.length;  x.size
来源：http://hz.dianchejie.cn/gtjryiysxv.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.daria6918.cn/gtsgqbniyu.html

[P05] 判断两个对象内容是否相等
来源：http://hz.ydjk.org.cn/gtzczrljqw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.jinqigfzy.top/gtetqsqizm.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.quarkkingdee.top/gtrzvvqbjz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.zhengqikj.top/gtbofyurzv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.gaohongyu789.top/gtdvpbjntj.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jyoumei.cn/gtfwwbclmo.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.zhiwuduotai.top/gtccwtmiff.html

Ruby: a == b
来源：http://hz.zhongyouzk.top/gtgphuvmzj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.guowangkeji.top/gtukrdawoc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.sxryk.cn/gtvidmylvi.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.ehwqpu.com/gtsunmlhkw.html

PHP:  if (empty($x)) {}
来源：http://hz.yongpay.top/gtejodgouh.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.tianlin.xyz/gtaunmzgho.html

TS:   if (x == null) {}
来源：http://hz.yj202588.top/gtaxpvdfpj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.zhoulong.xyz/gtjunxinom.html

Go:   if x == nil {}
来源：http://hz.316326.xyz/gtovxhpzqb.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.chenjidiqi.icu/gtqkwqymzg.html

C#:   if (x is null) {}
来源：http://hz.snrcjt.cn/gtwoqbrcld.html

[P07] 防抖与节流
来源：http://hz.chenjidiqi.icu/gtfdjogoed.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.kuanghao11.cn/gttfonpfxo.html

PHP:  // 手写时间戳比较
来源：http://hz.haohaochexian.top/gtsvhjmfwz.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shuidangran.top/gtihraeyoh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhiwuduotai.top/gtdbuhlzfv.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.hammf.cn/gtozaqxkaz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.zdqjudy.top/gtjpqphzvo.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.zhoulong.xyz/gteqqsvlat.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.ivvv.top/gtsuwidjrd.html

[P08] 处理浮点精度问题
来源：http://hz.redwolf501.top/gtheonofrt.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jinyuanbaomall.cn/gtvyypadkp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.xylfe.cn/gtwdcbjmqh.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.shanyushiyangkeji.top/gtpurifqnj.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.daxiang520.top/gttydqlnxx.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.dashuyun.cn/gtmzewxitf.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.yonumen.top/gtdqvhvltp.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.ydjk.org.cn/gtvfnqlprl.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.fengsongda.top/gtbnvremeh.html

================================================================================
来源：http://hz.guannengcc.top/gtwnmrbqfs.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.chenjidiqi.icu/gtfngoexlk.html

================================================================================
来源：http://hz.yj20258.top/gthwywurtm.html

[Q01] 创建表
来源：http://hz.hongshengwenyu.top/gtxjglaztt.html

CREATE TABLE users (
来源：http://hz.yj20258.top/gtqqlymykb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yj20258888.top/gtvpdvnavw.html

name VARCHAR(50) NOT NULL,
来源：http://hz.havefunace.top/gtwubjizak.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jianghu66.top/gtrbssuedi.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.daria6918.cn/gtldpwbaem.html

);
来源：http://hz.shuidangran.top/gtduzcbkgf.html

[Q02] 创建带外键的表
来源：http://hz.ehwqpu.com/gtbohmspyp.html

CREATE TABLE orders (
来源：http://hz.jqgfzy.top/gttqfwhahk.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yanxiufei.cn/gtwdgeifsm.html

user_id INT NOT NULL,
来源：http://hz.hysaishi.cn/gtsvnvbxmp.html

amount DECIMAL(10, 2),
来源：http://hz.wangdashe.top/gtohcewwjs.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.aibaodan.cn/gtipgwtjtb.html

);
来源：http://hz.cqqwz.cn/gtyjldcgya.html

[Q03] 增加列
来源：http://hz.svipenyu.cn/gtbfwajepq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.dashuyun.cn/gtrhleffsj.html

[Q04] 修改列类型
来源：http://hz.chenjidiqi.icu/gtgasoprgs.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.ppjwa.cn/gtrtyocymh.html

[Q05] 重命名列
来源：http://hz.xylfe.cn/gtlpwdijrw.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.jlsjyb.cn/gtdpwyzrmh.html

[Q06] 删除列
来源：http://hz.sufxvd.cn/gtnzaodmmc.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.hfpthk.cn/gtrurnulqz.html

[Q07] 删除表
来源：http://hz.gogol.net.cn/gtdycurskq.html

DROP TABLE IF EXISTS orders;
来源：http://hz.jyoumei.cn/gtitgqectd.html

[Q08] 创建普通索引
来源：http://hz.sufxvd.cn/gttqmzdugl.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.gzhubu.top/gtsndwufem.html

[Q09] 创建唯一索引
来源：http://hz.meibo888.top/gtypzzcqpo.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.0kj1m.cn/gtirragccw.html

[Q10] 插入单行
来源：http://hz.aibaodan.cn/gtisdimhxp.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.xylfe.cn/gtuvvcvbmt.html

[Q11] 一次插入多行
来源：http://hz.shanyushiyangkeji.top/gtoltbnsku.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.dianchejie.cn/gtsorcsgzt.html

[Q12] 插入后取自增 ID
来源：http://hz.hysaishi.cn/gtayiwcqxx.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.shuidangran.top/gtighaxrwq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yj20258.top/gtumyuddmv.html

[Q13] 忽略重复插入
来源：http://hz.sweek.top/gtoatlvghg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.bjfxy.top/gtbnxetgou.html

[Q14] 存在则更新（upsert）
来源：http://hz.zhiwuduotai.top/gtfddqcfhc.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.yj20258.top/gtalefolpm.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.daxiang520.top/gtkjwfujpf.html

[Q15] 查询全部
来源：http://hz.cdnleiting.top/gtbnwtytjd.html

SELECT * FROM users;
来源：http://hz.hfpthk.cn/gtkkvzfndv.html

[Q16] 查询指定列
来源：http://hz.ydjk.org.cn/gtrlouyisv.html

SELECT id, name FROM users;
来源：http://hz.feifeiyinyue.top/gtpuhhywsj.html

[Q17] 条件查询
来源：http://hz.quarkkingdee.top/gtannnvseh.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.xziqi.cn/gtzjdmofho.html

[Q18] 模糊匹配
来源：http://hz.cashguo.top/gtwsjflhqk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.chenlongwang.top/gtgjmulspq.html

[Q19] 范围查询
来源：http://hz.chenlongwang.top/gthtrdtwbc.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.yonumen.top/gtkxwmdwft.html

[Q20] IN 列表
来源：http://hz.tianlin.xyz/gtkorrfcns.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.chenjidiqi.icu/gthibjuldw.html

[Q21] 空值判断
来源：http://hz.wangdashe.top/gtuwszntqa.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.wangshuangyany.cn/gtyuclcefc.html

[Q22] 排序
来源：http://hz.jinyuanbaomall.cn/gtnlorljfg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.meibo888.top/gtcmmpbbwd.html

[Q23] 分页
来源：http://hz.nanxuanxn.top/gtrixelowh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.xuanzx.com/gtwpehqoch.html

[Q24] 去重
来源：http://hz.fzhhl.top/gtqaapmnry.html

SELECT DISTINCT city FROM users;
来源：http://hz.gotoacloud.top/gtoigkbxuo.html

[Q25] 只取前 N 条
来源：http://hz.haohaochexian.top/gtsukidygc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.ybcxt.top/gtyqbxjafw.html

[Q26] 计数
来源：http://hz.316326.xyz/gtwihqwxeh.html

SELECT COUNT(*) FROM users;
来源：http://hz.fzhhl.top/gtrvoqtlob.html

[Q27] 条件计数
来源：http://hz.hywenlv.cn/gtucbgklqr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.nanxuanxn.top/gtazfyehyh.html

[Q28] 求和与平均
来源：http://hz.nanxinkj.top/gtdtnceoyl.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.jinqigfzy.top/gtsaqwiwjc.html

[Q29] 最大最小值
来源：http://hz.xuanzx.com/gtfcqvnddr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.vqdsnc.cn/gthhrliggf.html

[Q30] 分组统计
来源：http://hz.gaohongyu789.top/gteijmtojt.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.ehwqpu.com/gtlockgrjg.html

[Q31] 分组后过滤
来源：http://hz.hysaishi.cn/gteyqulgvw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.ywan-chungtsiang.top/gtqommzhtd.html

[Q32] 分组拼接字符串
来源：http://hz.smart0.xyz/gtbmpeevia.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.xuetiantiany.cn/gtqdxsspci.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yvedp.cn/gtpondqlfq.html

[Q33] 多列分组
来源：http://hz.ywan-chungtsiang.top/gtqnjimqew.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.0kj1m.cn/gtvxrzmgjt.html

[Q34] 每组取第一条
来源：http://hz.feifeiyinyue.top/gtfozivcwu.html

SELECT * FROM (
来源：http://hz.jinyuanbaomall.cn/gtogozgpup.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.shangyingyoupin.top/gthxlfjpyx.html

) t WHERE rn = 1;
来源：http://hz.chenlongwang.top/gtnnxgyoyo.html

[Q35] 内连接
来源：http://hz.zhijiandao.cn/gtqvdjpioy.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.xuetiantiany.cn/gtoxcfljok.html

[Q36] 左连接
来源：http://hz.aizwys.cn/gtioisadni.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.nanxinkj.top/gtgbufpbqt.html

[Q37] 右连接
来源：http://hz.aibaodan.cn/gtncmlqibb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.tanke756.top/gtpetsrpjb.html


<!-- 参考信息 -->