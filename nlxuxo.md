代发 wailian999

Ruby: s == s.reverse
来源：http://hz.c1oappe.top/gttvlwwiea.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.jqgfzy.top/gttwrtekbs.html

[N07] 两数之和（返回下标）
来源：http://hz.sxryk.cn/gtcenqyauw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.hammf.cn/gtfblhqapg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yvedp.cn/gthbcndkfg.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.0kj1m.cn/gttqabaeyx.html

TS:   // 手写 Map<string, number>
来源：http://hz.jinqigufen.top/gtjegjlamr.html

Java: // 手写 HashMap
来源：http://hz.tanke756.top/gtxhfnvuxv.html

Go:   // 手写 map[int]int
来源：http://hz.haohaochexian.top/gtowuvnonb.html

Ruby: // 手写 Hash
来源：http://hz.0kj1m.cn/gtynqhenyz.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.quarkkingdee.top/gtqgmpzxex.html

[N08] 生成全排列
来源：http://hz.tian-w.cn/gtomhzigpg.html

Py:   itertools.permutations(arr)
来源：http://hz.daria6918.cn/gtdgdjyijw.html

PHP:  // 手写递归交换
来源：http://hz.sysykeji.top/gtmsnlyqkd.html

JS:   // 手写回溯递归
来源：http://hz.nanxinkj.top/gtovikttty.html

TS:   // 手写回溯递归
来源：http://hz.nanxuanxn.top/gtnkpldmio.html

Java: // 手写回溯递归
来源：http://hz.hnxiangtu.top/gtoenxdnbo.html

Go:   // 手写回溯递归
来源：http://hz.yj20258.top/gteumobxih.html

Ruby: arr.permutation.to_a
来源：http://hz.jlsjyb.cn/gtkbvuqbwl.html

C#:   // 手写回溯递归
来源：http://hz.52xcode.cn/gtutmnyjny.html

[N09] 栈与队列
来源：http://hz.zhaomingkeji.xyz/gthcqqvisn.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.c1oappe.top/gtvcobwuwf.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.sxryk.cn/gtulhezene.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.xinyue.icu/gtpoedsgta.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.nanxuanxn.top/gtuawwigxe.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.birdmap.top/gtqjmkcuzx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.jyoumei.cn/gtmvtmotzy.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.wangshuangyany.cn/gtoptxxhzj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.zhaomingkeji.xyz/gtwmimgbig.html

[N10] 链表节点定义
来源：http://hz.zhengqikj.top/gtgbrbxdnl.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.jlsjyb.cn/gtflmsfrrz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.fzhhl.top/gtxkyqqrvc.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.cashguo.top/gtdzuknofk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.smart0.xyz/gtyvnurjub.html

Java: class Node { int v; Node next; }
来源：http://hz.chenjidiqi.icu/gtzswrxzsp.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.pycfn.com/gtrotybjfj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.zdqjudy.top/gtvmtbxscb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.zhongyouzk.top/gthyzstoba.html

[N11] 二叉树中序遍历
来源：http://hz.wangdashe.top/gtgpbacadd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.tanke756.top/gtvjyxpazw.html

PHP:  // 手写递归函数
来源：http://hz.wangdashe.top/gtsbsxeubo.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.chenlongwang.top/gtgstxrkot.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhengqikj.top/gtiddvbhww.html

Java: // 手写递归
来源：http://hz.svipenyu.cn/gtqnttsxjk.html

Go:   // 手写递归
来源：http://hz.zhijiandao.cn/gtgnftejbc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.shzxlz.cn/gtlzxvgzbo.html

C#:   // 手写递归
来源：http://hz.jiagoushi.top/gtmsiwncly.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.zhixingplan.top/gtlybzbnds.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.zhoulong.xyz/gtegwndbfn.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.gotoacloud.top/gtrgwybmiy.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ydzc1.top/gtdstprklu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yuxming.cn/gtftdxceon.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.cqqwz.cn/gtltaglztk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.shuidangran.top/gtcyrgwzqm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.nwbrower.top/gtntakuquf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.shangyingyoupin.top/gtcyyejkxi.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtsaoosmon.html

O. 并发与异步
来源：http://hz.nwbrower.top/gtosmvefpw.html

================================================================================
来源：http://hz.redwolf501.top/gtivfpfapi.html

[O01] 启动一个线程
来源：http://hz.xinyue.icu/gtaoceztuw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.sufxvd.cn/gtgeiixqef.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.aibaodan.cn/gtkdnyyhml.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.meibo888.top/gthzfazepx.html

TS:   // 同 JS
来源：http://hz.redwolf501.top/gtjkdonyqe.html

Java: new Thread(() -> f()).start()
来源：http://hz.9152youxi.cn/gtonblmttd.html

Go:   go f()
来源：http://hz.sufxvd.cn/gtypwenrdt.html

Ruby: Thread.new { f }
来源：http://hz.dianchejie.cn/gtrayhkacq.html

C#:   Task.Run(() => F());
来源：http://hz.aizwys.cn/gtwdtgbrij.html

[O02] 使用线程池
来源：http://hz.daria6918.cn/gtcaxenaie.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.zhaomingkeji.xyz/gtlgngekot.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.tian-w.cn/gtfdxhtedb.html

JS:   // worker_threads 线程池
来源：http://hz.dashuyun.cn/gtjeqxdkhc.html

TS:   // worker_threads 线程池
来源：http://hz.xingfuxueyuan.xyz/gtakcrgppj.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yongpay.top/gtkuilaksg.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yangfankeji.com/gtztvnlcwy.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.shzxlz.cn/gtjagdsljg.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.shzxlz.cn/gtzvfftbvb.html

[O03] 加锁保护共享数据
来源：http://hz.birdmap.top/gtmvmxbwam.html

Py:   with lock: shared += 1
来源：http://hz.iojbl.cn/gtloqtxula.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.shzxlz.cn/gtdykgprga.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.yonumen.top/gtxejnpajs.html

TS:   // 同 JS
来源：http://hz.zhengqikj.top/gtjgfiwzcs.html

Java: synchronized (this) { shared++; }
来源：http://hz.sufxvd.cn/gtrbfhvhbm.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.nwbrower.top/gtdzjwocza.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.sweek.top/gtlunlpuvk.html

C#:   lock (gate) { shared++; }
来源：http://hz.cdnleiting.top/gtfzkjakwh.html

[O04] 定义异步函数并等待
来源：http://hz.hongshengwenyu.top/gtuyukfubk.html

Py:   async def f():⏎    await g()
来源：http://hz.sweek.top/gtoshyrwgf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.haohaochexian.top/gtspzhpbta.html

JS:   async function f() { await g(); }
来源：http://hz.cashguo.top/gtfaphvcre.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.cqqwz.cn/gtwraojwyw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.gaohongyu789.top/gtrlqcdzut.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.zhaomingkeji.xyz/gteysggoii.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.zhoulong.xyz/gtkyhxlggb.html

C#:   async Task F() { await G(); }
来源：http://hz.dashuyun.cn/gtqkduqzht.html

[O05] 并发执行并等待全部完成
来源：http://hz.zhengqikj.top/gtwmnzippl.html

Py:   asyncio.gather(*tasks)
来源：http://hz.shangyingyoupin.top/gtjtbnavfm.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.cashguo.top/gtjjkhrvuy.html

JS:   await Promise.all(tasks)
来源：http://hz.zhengqikj.top/gtltmzgahk.html

TS:   await Promise.all(tasks)
来源：http://hz.feifeiyinyue.top/gtvrrdbvdj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.0kj1m.cn/gtofdfpotx.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.feifeiyinyue.top/gtgqxuxsov.html

Ruby: threads.map(&:join)
来源：http://hz.jinghuilouyu.cn/gteccsqbal.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.jinqigfzy.top/gtsyuhqwef.html

[O06] 使用进程池
来源：http://hz.xylfe.cn/gtoilrkubo.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.xingfuxueyuan.xyz/gtncreixes.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.mhx1999.top/gtilkktxiz.html

JS:   // child_process / cluster 模块
来源：http://hz.jinghuilouyu.cn/gtmdhrqzzo.html

TS:   // child_process / cluster 模块
来源：http://hz.aizwys.cn/gttasllymq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.shanyushiyangkeji.top/gtbvyuvnli.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.hfpthk.cn/gtrlgofkza.html

Ruby: // fork 块
来源：http://hz.meibo888.top/gtswxkdleq.html

C#:   Parallel.For
来源：http://hz.nanxuanxn.top/gtzycvgjdw.html

================================================================================
来源：http://hz.jiagoushi.top/gtearchkls.html

P. 常用工具函数
来源：http://hz.cqqwz.cn/gtgccjeesr.html

================================================================================
来源：http://hz.nanxuanxn.top/gtoacdldqz.html

[P01] 生成 UUID
来源：http://hz.zycfv.cn/gturtthmxw.html

Py:   str(uuid.uuid4())
来源：http://hz.birdmap.top/gtrcxcgzbk.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.iojbl.cn/gtyqtijruw.html

JS:   crypto.randomUUID()
来源：http://hz.snrcjt.cn/gtabkcjzcp.html

TS:   crypto.randomUUID()
来源：http://hz.vqdsnc.cn/gtqbeogucv.html

Java: UUID.randomUUID().toString()
来源：http://hz.zycfv.cn/gtsnfroyai.html

Go:   // 用 github.com/google/uuid
来源：http://hz.pycfn.com/gtqnpwyipz.html

Ruby: SecureRandom.uuid
来源：http://hz.yanxiufei.cn/gtsrqdhcos.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.cheryme.top/gtbernanjj.html

[P02] MD5 / SHA256 摘要
来源：http://hz.yueranfly.top/gtyvpowlfz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.xylfe.cn/gteshrokjm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.wangshuangyany.cn/gtdmdkiiwo.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.kuanghao11.cn/gtmzhuuvjz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.shangyingyoupin.top/gtvwzzlzol.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.tanke756.top/gtgopcyiet.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.hfpthk.cn/gtkfexafak.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.c1oappe.top/gtxpikurnu.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.zycfv.cn/gtdtatlqta.html

[P03] 生成短随机字符串
来源：http://hz.yongpay.top/gtcoqkbcfl.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.shuidangran.top/gthkcbeklh.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.redwolf501.top/gtaaurheld.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.cheryme.top/gtwrejcvny.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hfpthk.cn/gtezxzjmjl.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.shangyingyoupin.top/gtrohquotx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.ydjk.org.cn/gtrmaoxfhw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.yvedp.cn/gtvknetueu.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.chenlongwang.top/gtsnufaewu.html

[P04] 求长度
来源：http://hz.yj20258.top/gtjeyainck.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.jinqigufen.top/gtlysfmhbx.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.cucudq.cn/gtweijfeds.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.cheryme.top/gtmegrnwtw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yj202588.top/gtfkqkttwo.html

Java: list.size();  map.size();  s.length()
来源：http://hz.bjfxy.top/gtvvnjhblj.html

Go:   len(arr);  len(m)
来源：http://hz.kuanghao11.cn/gtojauiktj.html

Ruby: x.length;  x.size
来源：http://hz.gotoacloud.top/gtmczzjrms.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.gzhubu.top/gtvpjwexfk.html

[P05] 判断两个对象内容是否相等
来源：http://hz.chenlongwang.top/gthsmtywjm.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.daria6918.cn/gtbfohffkr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.meibo888.top/gtwdwdwsla.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.yj20258.top/gtgeokayms.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jinyuanbaomall.cn/gtcvcbvumm.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.cqqwz.cn/gtxlqumcma.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.ivvv.top/gtbvpaeexk.html

Ruby: a == b
来源：http://hz.ydjk.org.cn/gtpysmlecu.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.cheryme.top/gttmkzdwky.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.shanyushiyangtech.top/gtgsebpydm.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.sufxvd.cn/gtvmmhvehw.html

PHP:  if (empty($x)) {}
来源：http://hz.gaohongyu789.top/gtitgixdel.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.yangfankeji.com/gtemtvhivh.html

TS:   if (x == null) {}
来源：http://hz.cucudq.cn/gtgapewstr.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.fengsongda.top/gtobnsldkb.html

Go:   if x == nil {}
来源：http://hz.zhixingplan.top/gtbqixeceg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.hywenlv.cn/gtirvkbkmt.html

C#:   if (x is null) {}
来源：http://hz.dashuyun.cn/gtdxbipohu.html

[P07] 防抖与节流
来源：http://hz.redwolf501.top/gtxhxjmrxd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.cdnleiting.top/gtrsldjwtw.html

PHP:  // 手写时间戳比较
来源：http://hz.gzhubu.top/gtbrbzwcjo.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.gaohongyu789.top/gthcfvssqj.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yuanzhike.top/gtrjpqbitm.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.cqqwz.cn/gtshyjzqke.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.yuanzhike.top/gtztqfingl.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.0kj1m.cn/gtinrhfhpw.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.zhoulong.xyz/gtarhnzuyt.html

[P08] 处理浮点精度问题
来源：http://hz.9152youxi.cn/gtryafozcx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.shanyushiyangkeji.top/gtxojnmvxu.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.zycfv.cn/gtrhehzxii.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.jianghu66.top/gtxjzchgsm.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.jyoumei.cn/gtyrxmvstz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.shangyingyoupin.top/gtblmvgctd.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.jinqigfzy.top/gtehpezbmc.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.yuxming.cn/gtmbqwyzvj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.yanxiufei.cn/gtnyhcxtep.html

================================================================================
来源：http://hz.smart0.xyz/gtdijvzukg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.jiagoushi.top/gtxblxbulb.html

================================================================================
来源：http://hz.ppjwa.cn/gtwjhenuor.html

[Q01] 创建表
来源：http://hz.ivvv.top/gtkjvyrwkq.html

CREATE TABLE users (
来源：http://hz.ehwqpu.com/gtlqfiiehq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xuetiantiany.cn/gtmkuvcyfo.html

name VARCHAR(50) NOT NULL,
来源：http://hz.zhiwuduotai.top/gtjowjctxp.html

email VARCHAR(100) UNIQUE,
来源：http://hz.hywenlv.cn/gtjupjlkce.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.gzhubu.top/gtxftzuzlp.html

);
来源：http://hz.aizwys.cn/gtndybenrv.html

[Q02] 创建带外键的表
来源：http://hz.jiagoushi.top/gtbskdextk.html

CREATE TABLE orders (
来源：http://hz.pycfn.com/gtyhojtzye.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ydjk.org.cn/gtmhppxciu.html

user_id INT NOT NULL,
来源：http://hz.iojbl.cn/gtvehovuvs.html

amount DECIMAL(10, 2),
来源：http://hz.pycfn.com/gtxjwgucjb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.hammf.cn/gtvmrtzgnq.html

);
来源：http://hz.pycfn.com/gtznyuslwu.html

[Q03] 增加列
来源：http://hz.tianlin.xyz/gtrexholyt.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.dianchejie.cn/gtuemybgly.html

[Q04] 修改列类型
来源：http://hz.ehwqpu.com/gtvhqmmrrd.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.feifeiyinyue.top/gtxezkucea.html

[Q05] 重命名列
来源：http://hz.xylfe.cn/gtyyeywlfo.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.xuetiantiany.cn/gtfrrpszuq.html

[Q06] 删除列
来源：http://hz.shanyushiyangkeji.top/gticbaabwp.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.jinyuanbaomall.cn/gtzwrhqpse.html

[Q07] 删除表
来源：http://hz.jyoumei.cn/gtydqweiwv.html

DROP TABLE IF EXISTS orders;
来源：http://hz.xuetiantiany.cn/gtvdfjjvxd.html

[Q08] 创建普通索引
来源：http://hz.havefunace.top/gtekgyqmrf.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.shanyushiyangkeji.top/gtxkwzzdwj.html

[Q09] 创建唯一索引
来源：http://hz.jlsjyb.cn/gtukvygfeu.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.hongshengwenyu.top/gtylbtklqd.html

[Q10] 插入单行
来源：http://hz.xinyue.icu/gthofwoerr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jinqigufen.top/gttrqunrcv.html

[Q11] 一次插入多行
来源：http://hz.zhixingplan.top/gtuecmdfmt.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.zycfv.cn/gtqpxrkzzs.html

[Q12] 插入后取自增 ID
来源：http://hz.meibo888.top/gtmxfrjthf.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.jqgfzy.top/gtzyhnvmnk.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.cashguo.top/gtzgealjyv.html

[Q13] 忽略重复插入
来源：http://hz.wangdashe.top/gtqsmedlhm.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.zhongyouzk.top/gtqdasrdtq.html

[Q14] 存在则更新（upsert）
来源：http://hz.xziqi.cn/gtlgyyhxmi.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.316326.xyz/gtmwsuucxn.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.yj20258888.top/gtleyjvkhs.html

[Q15] 查询全部
来源：http://hz.ppjwa.cn/gtwxnqvkix.html

SELECT * FROM users;
来源：http://hz.yangfankeji.com/gtluecsyhe.html

[Q16] 查询指定列
来源：http://hz.ydzc1.top/gtpscvgqzu.html

SELECT id, name FROM users;
来源：http://hz.xuanzx.com/gtpubvigle.html

[Q17] 条件查询
来源：http://hz.cashguo.top/gtarpenxqq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.svipenyu.cn/gtffgugxag.html

[Q18] 模糊匹配
来源：http://hz.shzxlz.cn/gtoqoflqgk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.chenjidiqi.icu/gtlxeophpv.html

[Q19] 范围查询
来源：http://hz.316326.xyz/gtouetlevg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.vqdsnc.cn/gtyyjsjdxl.html

[Q20] IN 列表
来源：http://hz.meibo888.top/gtmyzeudyt.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yanxiufei.cn/gtzgmkykgx.html

[Q21] 空值判断
来源：http://hz.sxryk.cn/gtmjypreqt.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.hnqzz.top/gtmvjpuchj.html

[Q22] 排序
来源：http://hz.zhiwuduotai.top/gtohjjrujs.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.cheryme.top/gtwpfugpvc.html

[Q23] 分页
来源：http://hz.9152youxi.cn/gtrxhgjuoh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.ehwqpu.com/gtbystuzeb.html

[Q24] 去重
来源：http://hz.zhengqikj.top/gtwlydtyxg.html

SELECT DISTINCT city FROM users;
来源：http://hz.daxiang520.top/gtrmteyatp.html

[Q25] 只取前 N 条
来源：http://hz.cashguo.top/gtluqwbarw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.hnxiangtu.top/gtrkhhcxhw.html

[Q26] 计数
来源：http://hz.aibaodan.cn/gtaabkmwed.html

SELECT COUNT(*) FROM users;
来源：http://hz.gaohongyu789.top/gttcpuzlob.html

[Q27] 条件计数
来源：http://hz.tian-w.cn/gttpnyvule.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.zhengqikj.top/gtulcigaex.html

[Q28] 求和与平均
来源：http://hz.jiagoushi.top/gthbshdwpz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.nanxinkj.top/gttbxrvwwg.html

[Q29] 最大最小值
来源：http://hz.yuanzhike.top/gtxrsdiztj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.iojbl.cn/gtunoirpts.html

[Q30] 分组统计
来源：http://hz.zhengqikj.top/gtewpnxpgp.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.hnqzz.top/gtnklwnebw.html

[Q31] 分组后过滤
来源：http://hz.aizwys.cn/gtpdacajlq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.meibo888.top/gtjdfcdbql.html

[Q32] 分组拼接字符串
来源：http://hz.jianghu66.top/gtemmervzb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.quarkkingdee.top/gtvjrzbkwx.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.xylfe.cn/gtafcizwbj.html

[Q33] 多列分组
来源：http://hz.hfpthk.cn/gtjmyzklcx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.c1oappe.top/gtyohhmbkz.html

[Q34] 每组取第一条
来源：http://hz.wangdashe.top/gtoajxglsb.html

SELECT * FROM (
来源：http://hz.jlsjyb.cn/gtanhcdmhk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jqgufenzy.top/gtsevpsbpd.html

) t WHERE rn = 1;
来源：http://hz.yonumen.top/gtvovncxcm.html

[Q35] 内连接
来源：http://hz.shanyushiyangkeji.top/gtcmrpjvql.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.sysykeji.top/gtaaipdojo.html

[Q36] 左连接
来源：http://hz.pengpengdd.cyou/gtogbdzwby.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.xingfuxueyuan.xyz/gtvyuebsdr.html

[Q37] 右连接
来源：http://hz.hongshengwenyu.top/gteetmksaa.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.xingfuxueyuan.xyz/gtsxqbfvvy.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.kuanghao11.cn/gtspoxpcoo.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.52xcode.cn/gtsxfjlcnl.html

[Q39] 自连接（查上下级）
来源：http://hz.jqgfzy.top/gtrvmdexqh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.shzxlz.cn/gthizddlee.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.xinyue.icu/gttcomsyks.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.fzhhl.top/gtnsmwjgdu.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.shanyushiyangtech.top/gttyvtqnol.html

[Q41] 多表连接
来源：http://hz.dashuyun.cn/gtvvtcabjq.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.redwolf501.top/gtlpctykjx.html

JOIN users u ON u.id = o.user_id
来源：http://hz.chenjidiqi.icu/gtkxffpvve.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.xingfuxueyuan.xyz/gtpkhgxuko.html

[Q42] 连接条件附加过滤
来源：http://hz.wangshuangyany.cn/gtghpvctqj.html

SELECT u.name, o.amount FROM users u
来源：http://hz.jianghu66.top/gtrnigyohe.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.chenzaomai.com/gtwohoawde.html

[Q43] 标量子查询
来源：http://hz.quarkkingdee.top/gtvpmpdfrr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.aibaodan.cn/gtxkijhrpq.html

[Q44] IN 子查询
来源：http://hz.chenlongwang.top/gtjlxcaeoc.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.zhaomingkeji.xyz/gtxkdodcnz.html

[Q45] EXISTS 判断存在
来源：http://hz.redwolf501.top/gtmnenfvem.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yj202588.top/gttdwqvmwg.html


<!-- 参考信息 -->