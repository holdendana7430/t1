代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://hz.xingfuxueyuan.xyz/gtzghjbysc.html

TS:   s === [...s].reverse().join("")
来源：http://hz.shzxlz.cn/gtmdzxjswc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.chenzaomai.com/gtzeajdrmu.html

Go:   // 双指针从两端比较
来源：http://hz.0kj1m.cn/gtysjkgktd.html

Ruby: s == s.reverse
来源：http://hz.svipenyu.cn/gtohlacdso.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.ywan-chungtsiang.top/gtdvxmrmut.html

[N07] 两数之和（返回下标）
来源：http://hz.jinqigufen.top/gthqufumcl.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.gaohongyu789.top/gtmgxfytwd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.bjfxy.top/gtvjoddtmc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.feifeiyinyue.top/gtsuvrqyiy.html

TS:   // 手写 Map<string, number>
来源：http://hz.feifeiyinyue.top/gtepmgxcej.html

Java: // 手写 HashMap
来源：http://hz.zhongyouzk.top/gtoxwsvsft.html

Go:   // 手写 map[int]int
来源：http://hz.cqqwz.cn/gtplxijhny.html

Ruby: // 手写 Hash
来源：http://hz.zhiwuduotai.top/gtjmanyscw.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yj20258.top/gtezopbung.html

[N08] 生成全排列
来源：http://hz.hongshengwenyu.top/gtfxwreqwp.html

Py:   itertools.permutations(arr)
来源：http://hz.ivvv.top/gthpgsekvm.html

PHP:  // 手写递归交换
来源：http://hz.gaohongyu789.top/gtdeqqyduf.html

JS:   // 手写回溯递归
来源：http://hz.ywan-chungtsiang.top/gtsinzqkqc.html

TS:   // 手写回溯递归
来源：http://hz.0kj1m.cn/gtzdogqohu.html

Java: // 手写回溯递归
来源：http://hz.jinghuilouyu.cn/gtozgumdhs.html

Go:   // 手写回溯递归
来源：http://hz.guannengcc.top/gtgzdodkvz.html

Ruby: arr.permutation.to_a
来源：http://hz.jinyuanbaomall.cn/gtnpmgkllc.html

C#:   // 手写回溯递归
来源：http://hz.chenzaomai.com/gtwhjuhcpp.html

[N09] 栈与队列
来源：http://hz.jlsjyb.cn/gtcyighvgi.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.ybcxt.top/gttcnjhkcq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.chenjidiqi.icu/gtwwtfarig.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.wangdashe.top/gtartahhwl.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yj20258.top/gtoozmrhcz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yanxiufei.cn/gtllvrbckj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.aizwys.cn/gtvikvysvi.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.jqgufenzy.top/gtiavoolyp.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yuanzhike.top/gtlzjtqhkq.html

[N10] 链表节点定义
来源：http://hz.xinyue.icu/gtgrjxmojz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.zhoulong.xyz/gtdhmlvsmy.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.xingfuxueyuan.xyz/gtoibjrnmc.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.mhx1999.top/gtsbcxkdaj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.yj20258.top/gtuefvkwyh.html

Java: class Node { int v; Node next; }
来源：http://hz.jiagoushi.top/gtzgxmuhoa.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.zhaomingkeji.xyz/gtqaylhohc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.sweek.top/gtwbuhutje.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.cdnleiting.top/gtznhhawwd.html

[N11] 二叉树中序遍历
来源：http://hz.316326.xyz/gttblpcici.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.ybcxt.top/gttjasycxz.html

PHP:  // 手写递归函数
来源：http://hz.nwbrower.top/gtiabfmqab.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.tianlin.xyz/gtrppgulkf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yanxiufei.cn/gtlpmvklwl.html

Java: // 手写递归
来源：http://hz.hysaishi.cn/gtlghczayw.html

Go:   // 手写递归
来源：http://hz.yj20258888.top/gtepsibgku.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.iojbl.cn/gtbvhxtjee.html

C#:   // 手写递归
来源：http://hz.bjfxy.top/gtjaipaple.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.zhiwuduotai.top/gtesfxjvhx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.xylfe.cn/gtsgeemkcd.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.wangshuangyany.cn/gtmwawuapn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yj20258888.top/gtxuufknzv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.nanxuanxn.top/gtnirfbksk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yj202588.top/gtguhxxkhe.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.svipenyu.cn/gtqvbogvkp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.jinghuilouyu.cn/gtpkuvxmjz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yj20258888.top/gtyzdzadfu.html

================================================================================
来源：http://hz.iojbl.cn/gtdwryrnir.html

O. 并发与异步
来源：http://hz.hammf.cn/gtdvkxzauj.html

================================================================================
来源：http://hz.hnqzz.top/gterlnovax.html

[O01] 启动一个线程
来源：http://hz.shuidangran.top/gtztmcpoyp.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.zhaomingkeji.xyz/gtfxyngioz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.nanxinkj.top/gtrxhwzzbr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.zhaomingkeji.xyz/gtgcsrhaio.html

TS:   // 同 JS
来源：http://hz.jinqigufen.top/gtjkzarmrq.html

Java: new Thread(() -> f()).start()
来源：http://hz.wangdashe.top/gtuqjqxced.html

Go:   go f()
来源：http://hz.sweek.top/gtmbzmykii.html

Ruby: Thread.new { f }
来源：http://hz.yangfankeji.com/gtppmfyovx.html

C#:   Task.Run(() => F());
来源：http://hz.jinghuilouyu.cn/gtmddnudwy.html

[O02] 使用线程池
来源：http://hz.hywenlv.cn/gtsgzfljcc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.hongshengwenyu.top/gtqobtekjd.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.meibo888.top/gttrgjzsqi.html

JS:   // worker_threads 线程池
来源：http://hz.yvedp.cn/gtuckgukfv.html

TS:   // worker_threads 线程池
来源：http://hz.jinghuilouyu.cn/gtymryfmbs.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.jyoumei.cn/gtbmmudohc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.cqqwz.cn/gtmjthukbi.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.c1oappe.top/gtqyrppszv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.yuxming.cn/gtxnctyczr.html

[O03] 加锁保护共享数据
来源：http://hz.jinghuilouyu.cn/gttpfwxsup.html

Py:   with lock: shared += 1
来源：http://hz.gzhubu.top/gtgpkpagxu.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.hongshengwenyu.top/gtzxdwcmik.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.sweek.top/gtbiwejfxs.html

TS:   // 同 JS
来源：http://hz.yj20258888.top/gtjesatahx.html

Java: synchronized (this) { shared++; }
来源：http://hz.zhaomingkeji.xyz/gtuktbajsl.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.tian-w.cn/gtfrfslhji.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.svipenyu.cn/gtdghknerv.html

C#:   lock (gate) { shared++; }
来源：http://hz.wangdashe.top/gtijvzawgb.html

[O04] 定义异步函数并等待
来源：http://hz.gotoacloud.top/gtxzjbjfpy.html

Py:   async def f():⏎    await g()
来源：http://hz.xingfuxueyuan.xyz/gtexkkdeyb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.guowangkeji.top/gtymvnijkp.html

JS:   async function f() { await g(); }
来源：http://hz.jyoumei.cn/gtnrcqjmut.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.shuidangran.top/gtmavbhdip.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.ivvv.top/gtynntniso.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.cheryme.top/gtloqdsvmm.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.andypj.xyz/gtinxcqycl.html

C#:   async Task F() { await G(); }
来源：http://hz.aizwys.cn/gtiqedjyfh.html

[O05] 并发执行并等待全部完成
来源：http://hz.sufxvd.cn/gtxdufzdpi.html

Py:   asyncio.gather(*tasks)
来源：http://hz.ppjwa.cn/gthfucxjuo.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.smart0.xyz/gttultnnec.html

JS:   await Promise.all(tasks)
来源：http://hz.nwbrower.top/gtaiyiexqd.html

TS:   await Promise.all(tasks)
来源：http://hz.wangshuangyany.cn/gtvnsydwzp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.zdqjudy.top/gtrnwgwabi.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.xziqi.cn/gtyrrinlem.html

Ruby: threads.map(&:join)
来源：http://hz.iojbl.cn/gtvdkhcseu.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yuxming.cn/gtzkgxqamr.html

[O06] 使用进程池
来源：http://hz.hnxiangtu.top/gtdmsnqsfn.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.chenlongwang.top/gttyctztxq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.nanxinkj.top/gtmefkztqi.html

JS:   // child_process / cluster 模块
来源：http://hz.pycfn.com/gtpryskbzd.html

TS:   // child_process / cluster 模块
来源：http://hz.ybcxt.top/gtzkmgdrof.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yuanzhike.top/gtoqtesaiu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.aibaodan.cn/gtqesoaoea.html

Ruby: // fork 块
来源：http://hz.hfpthk.cn/gtplwtdggs.html

C#:   Parallel.For
来源：http://hz.haohaochexian.top/gtpdwcshet.html

================================================================================
来源：http://hz.jiagoushi.top/gteozmnzxk.html

P. 常用工具函数
来源：http://hz.mhx1999.top/gtoysvkntw.html

================================================================================
来源：http://hz.vqdsnc.cn/gtdodszxbp.html

[P01] 生成 UUID
来源：http://hz.yvedp.cn/gtbazyyrms.html

Py:   str(uuid.uuid4())
来源：http://hz.chenzaomai.com/gtkjtnmgqe.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jlsjyb.cn/gtmvubqobw.html

JS:   crypto.randomUUID()
来源：http://hz.zhengqikj.top/gtvwgasarq.html

TS:   crypto.randomUUID()
来源：http://hz.aizwys.cn/gtorytzzgp.html

Java: UUID.randomUUID().toString()
来源：http://hz.316326.xyz/gthryjazuk.html

Go:   // 用 github.com/google/uuid
来源：http://hz.guannengcc.top/gtddyjjunc.html

Ruby: SecureRandom.uuid
来源：http://hz.jinghuilouyu.cn/gtuckaifhs.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.redwolf501.top/gtxwaatthz.html

[P02] MD5 / SHA256 摘要
来源：http://hz.shuidangran.top/gtyfmzcjvm.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.iojbl.cn/gtcegavzmn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.xinyue.icu/gtbuapmgvh.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.fzhhl.top/gtizrfcxph.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.kuanghao11.cn/gtavhopuyz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.zhoulong.xyz/gtalhekqyp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.ehwqpu.com/gtifdictai.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.zhongyouzk.top/gthhrmoogd.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.ivvv.top/gtdiggukuw.html

[P03] 生成短随机字符串
来源：http://hz.zhoulong.xyz/gtynmmzaia.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.hnqzz.top/gtdcybddin.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.jianghu66.top/gtmhlxlnng.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xingfuxueyuan.xyz/gtvitvmidg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xuetiantiany.cn/gtxdvusbtb.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.snrcjt.cn/gtctyujqhi.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.guannengcc.top/gtbiplpkhi.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jinqigufen.top/gtafqkezdc.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.havefunace.top/gtgubnfyms.html

[P04] 求长度
来源：http://hz.tian-w.cn/gtpschvclo.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.svipenyu.cn/gtvednwsqt.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zycfv.cn/gtlngkjqna.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yonumen.top/gtxndtxqkx.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.gogol.net.cn/gtprdaoxfb.html

Java: list.size();  map.size();  s.length()
来源：http://hz.xuetiantiany.cn/gtczxwuzpk.html

Go:   len(arr);  len(m)
来源：http://hz.yueranfly.top/gtbjcgrpxq.html

Ruby: x.length;  x.size
来源：http://hz.yuxming.cn/gtcsqwreaf.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.chenjidiqi.icu/gtxbhmgjfy.html

[P05] 判断两个对象内容是否相等
来源：http://hz.ehwqpu.com/gthgcvnvhr.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.fzhhl.top/gtcfjiayqt.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.cdnleiting.top/gtywhoiaib.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.hysaishi.cn/gttbzihjqo.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.xingfuxueyuan.xyz/gtiazboxzl.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.wangshuangyany.cn/gtadehukkk.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.guannengcc.top/gtwefshboi.html

Ruby: a == b
来源：http://hz.dashuyun.cn/gtvaxpcfmu.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.kuanghao11.cn/gttjustvdx.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.cdnleiting.top/gtivlsktqh.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.iojbl.cn/gtfflopnvs.html

PHP:  if (empty($x)) {}
来源：http://hz.ybcxt.top/gtmmjkxzuq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.fzhhl.top/gtosbqzllr.html

TS:   if (x == null) {}
来源：http://hz.yangfankeji.com/gtjcaozyhd.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.shuidangran.top/gtwdczosnu.html

Go:   if x == nil {}
来源：http://hz.9152youxi.cn/gtzqqvenpc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.shuidangran.top/gtqoxgdrux.html

C#:   if (x is null) {}
来源：http://hz.ybcxt.top/gtgmcxrgii.html

[P07] 防抖与节流
来源：http://hz.daria6918.cn/gtkykeysxt.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.aibaodan.cn/gtahodgoxr.html

PHP:  // 手写时间戳比较
来源：http://hz.cqqwz.cn/gttdyrbnvb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.gogol.net.cn/gtbuqvpzcr.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jinqigufen.top/gtfgswpnny.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.xingfuxueyuan.xyz/gtuzekncib.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.jiagoushi.top/gtgtijaksn.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yongpay.top/gthnlhnamy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.hammf.cn/gtuyafffrl.html

[P08] 处理浮点精度问题
来源：http://hz.ehwqpu.com/gtrpnexqni.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.52xcode.cn/gtifosmemh.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.cashguo.top/gtpxwghfau.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.svipenyu.cn/gtdivroaod.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.jinghuilouyu.cn/gteerpfojs.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.zycfv.cn/gtbocwdgnq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.yangfankeji.com/gtfnyfbkqy.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.andypj.xyz/gtwhummzql.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.guannengcc.top/gtznyvpeib.html

================================================================================
来源：http://hz.cdnleiting.top/gtpovwisao.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.ydjk.org.cn/gtbphzqnop.html

================================================================================
来源：http://hz.xinyue.icu/gthrwrjwsk.html

[Q01] 创建表
来源：http://hz.jqgufenzy.top/gthbdcarbm.html

CREATE TABLE users (
来源：http://hz.jqgfzy.top/gtnnjphdkk.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yj20258.top/gtxrkeetdr.html

name VARCHAR(50) NOT NULL,
来源：http://hz.yonumen.top/gtwfdbxbhh.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jinyuanbaomall.cn/gtvdokyspb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.hnxiangtu.top/gtvzdinuvh.html

);
来源：http://hz.dashuyun.cn/gtujhleths.html

[Q02] 创建带外键的表
来源：http://hz.cdnleiting.top/gtfurnqfqn.html

CREATE TABLE orders (
来源：http://hz.birdmap.top/gtuifixjzs.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.tanke756.top/gtpijdpddy.html

user_id INT NOT NULL,
来源：http://hz.feifeiyinyue.top/gtvwxsscby.html

amount DECIMAL(10, 2),
来源：http://hz.cheryme.top/gtkplwdsut.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.xylfe.cn/gtyddnkaus.html

);
来源：http://hz.aizwys.cn/gtwmyrcqiq.html

[Q03] 增加列
来源：http://hz.chenlongwang.top/gttsavjzrt.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.jinqigfzy.top/gtoxsnnznv.html

[Q04] 修改列类型
来源：http://hz.sweek.top/gttnsktsyn.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.nanxuanxn.top/gtknpajqaj.html

[Q05] 重命名列
来源：http://hz.nanxinkj.top/gteovdiqfs.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.jinqigufen.top/gtunkdjbex.html

[Q06] 删除列
来源：http://hz.shangyingyoupin.top/gtdxtqybus.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.xinyue.icu/gtpsjkpkjq.html

[Q07] 删除表
来源：http://hz.yongpay.top/gtwqbrcrqe.html

DROP TABLE IF EXISTS orders;
来源：http://hz.zhengqikj.top/gtanfzpzak.html

[Q08] 创建普通索引
来源：http://hz.yuanzhike.top/gtyqhnkpmu.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.fengsongda.top/gtoqpksjvk.html

[Q09] 创建唯一索引
来源：http://hz.yj20258.top/gtanswqseo.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.ywan-chungtsiang.top/gtrorkitau.html

[Q10] 插入单行
来源：http://hz.52xcode.cn/gtskeezhei.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.tianlin.xyz/gtzrdpgmel.html

[Q11] 一次插入多行
来源：http://hz.gotoacloud.top/gttbevhdcc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.hnxiangtu.top/gterykbitz.html

[Q12] 插入后取自增 ID
来源：http://hz.zhengqikj.top/gttmdsxoos.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.chenzaomai.com/gtvbebtcmr.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.nanxinkj.top/gtfybbhqkx.html

[Q13] 忽略重复插入
来源：http://hz.guannengcc.top/gtojgtosns.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jqgufenzy.top/gtkninykjr.html

[Q14] 存在则更新（upsert）
来源：http://hz.yangfankeji.com/gtropzvcza.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.jqgufenzy.top/gttbfiyium.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.ydjk.org.cn/gtutcbckpt.html

[Q15] 查询全部
来源：http://hz.zhiwuduotai.top/gtwvhejuvh.html

SELECT * FROM users;
来源：http://hz.jlsjyb.cn/gtsjkyrxgm.html

[Q16] 查询指定列
来源：http://hz.sweek.top/gtmrxzpyce.html

SELECT id, name FROM users;
来源：http://hz.yueranfly.top/gtjhbbnlix.html

[Q17] 条件查询
来源：http://hz.tian-w.cn/gtbunwtycu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.tian-w.cn/gtgcnluurs.html

[Q18] 模糊匹配
来源：http://hz.wangshuangyany.cn/gtmmkkbmri.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.52xcode.cn/gtjxpngxea.html

[Q19] 范围查询
来源：http://hz.ybcxt.top/gtxcexybkx.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.ybcxt.top/gtqsykuffb.html

[Q20] IN 列表
来源：http://hz.sxryk.cn/gtfgqvyyow.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.xziqi.cn/gtfyghkpnu.html

[Q21] 空值判断
来源：http://hz.yuxming.cn/gtlfgqcqxc.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.xziqi.cn/gtzzybqxhz.html

[Q22] 排序
来源：http://hz.fengsongda.top/gtcmnvhemj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.shuidangran.top/gtoyroghsl.html

[Q23] 分页
来源：http://hz.chenjidiqi.icu/gtcohjizaf.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.kuanghao11.cn/gtubtapnut.html

[Q24] 去重
来源：http://hz.sxryk.cn/gtxswpipum.html

SELECT DISTINCT city FROM users;
来源：http://hz.yueranfly.top/gtkqqdokvw.html

[Q25] 只取前 N 条
来源：http://hz.redwolf501.top/gtdqxnckif.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.ydzc1.top/gtcvrpexxl.html

[Q26] 计数
来源：http://hz.andypj.xyz/gtvbliorkx.html

SELECT COUNT(*) FROM users;
来源：http://hz.yangfankeji.com/gtlzbhrqvv.html

[Q27] 条件计数
来源：http://hz.yj20258.top/gtxrsvogte.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.daria6918.cn/gtnyjvqibn.html

[Q28] 求和与平均
来源：http://hz.gogol.net.cn/gtpwcmiyhq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.ydzc1.top/gtuhlpotmi.html

[Q29] 最大最小值
来源：http://hz.zycfv.cn/gtnnnstpzn.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.tianlin.xyz/gteimlsphw.html

[Q30] 分组统计
来源：http://hz.aizwys.cn/gtikpzntxv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.hfpthk.cn/gtpuvcljmj.html

[Q31] 分组后过滤
来源：http://hz.birdmap.top/gtxkhjslzc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.zdqjudy.top/gtugjcnedb.html

[Q32] 分组拼接字符串
来源：http://hz.hywenlv.cn/gtulclupoa.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.birdmap.top/gtfbgeabwi.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.tanke756.top/gtesizltaw.html

[Q33] 多列分组
来源：http://hz.jqgufenzy.top/gtvyzazzcs.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yuanzhike.top/gtyauckyqj.html

[Q34] 每组取第一条
来源：http://hz.aizwys.cn/gtpjdxytqt.html

SELECT * FROM (
来源：http://hz.xinyue.icu/gtvbvjntvb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.zhixingplan.top/gtchtojrbz.html

) t WHERE rn = 1;
来源：http://hz.xziqi.cn/gtuombbghg.html

[Q35] 内连接
来源：http://hz.dashuyun.cn/gtwsdeionn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.ywan-chungtsiang.top/gtprmmzett.html

[Q36] 左连接
来源：http://hz.9152youxi.cn/gtondlnyad.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.316326.xyz/gtbqdspzgd.html

[Q37] 右连接
来源：http://hz.ivvv.top/gtzhnxwxsq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.zhixingplan.top/gtzdnaomax.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.chenzaomai.com/gtaokcswkt.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.yuxming.cn/gtazatdmwp.html

[Q39] 自连接（查上下级）
来源：http://hz.zhixingplan.top/gtvivmrrvs.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jinghuilouyu.cn/gtcqofjffo.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.ppjwa.cn/gtckxpcdtp.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.sweek.top/gtwlbuutxs.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.yonumen.top/gtocsxtuis.html

[Q41] 多表连接
来源：http://hz.yanxiufei.cn/gtuufgegjz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.xylfe.cn/gtrkhgnwfq.html

JOIN users u ON u.id = o.user_id
来源：http://hz.jyoumei.cn/gtmarcttxw.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.xylfe.cn/gtwuiayoqa.html

[Q42] 连接条件附加过滤
来源：http://hz.zhongyouzk.top/gtepyjsqfl.html

SELECT u.name, o.amount FROM users u
来源：http://hz.nanxinkj.top/gtbwebzgia.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.tianlin.xyz/gtbucghxju.html

[Q43] 标量子查询
来源：http://hz.jiagoushi.top/gtkzdsmuch.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.nwbrower.top/gtvvmpedbg.html


<!-- 参考信息 -->