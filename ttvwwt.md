代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://hz.chenjidiqi.icu/gtdnybhepl.html

TS:   s === [...s].reverse().join("")
来源：http://hz.tianlin.xyz/gtpxcidjoy.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.hongshengwenyu.top/gtmrftwgtw.html

Go:   // 双指针从两端比较
来源：http://hz.xuetiantiany.cn/gthbxnodtj.html

Ruby: s == s.reverse
来源：http://hz.aibaodan.cn/gtestncpxj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.hfpthk.cn/gtadlhqnzi.html

[N07] 两数之和（返回下标）
来源：http://hz.hnxiangtu.top/gtemdkvtbq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.gotoacloud.top/gtalynktpo.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.cqqwz.cn/gtzvakkocp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.hnqzz.top/gtxphrecuu.html

TS:   // 手写 Map<string, number>
来源：http://hz.svipenyu.cn/gtnaxqbrca.html

Java: // 手写 HashMap
来源：http://hz.ppjwa.cn/gtiusgkkog.html

Go:   // 手写 map[int]int
来源：http://hz.jiagoushi.top/gtyykhsimq.html

Ruby: // 手写 Hash
来源：http://hz.jqgufenzy.top/gtklhfunqv.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.zhoulong.xyz/gtvblocuwh.html

[N08] 生成全排列
来源：http://hz.xuanzx.com/gthqmummrk.html

Py:   itertools.permutations(arr)
来源：http://hz.xuetiantiany.cn/gtlokbqzhd.html

PHP:  // 手写递归交换
来源：http://hz.chenzaomai.com/gtdsiibdfx.html

JS:   // 手写回溯递归
来源：http://hz.yonumen.top/gtdngzlqra.html

TS:   // 手写回溯递归
来源：http://hz.yuxming.cn/gtdresvkug.html

Java: // 手写回溯递归
来源：http://hz.zhengqikj.top/gtesetvbtk.html

Go:   // 手写回溯递归
来源：http://hz.nanxinkj.top/gtprovbrgf.html

Ruby: arr.permutation.to_a
来源：http://hz.quarkkingdee.top/gtbcgttxds.html

C#:   // 手写回溯递归
来源：http://hz.gzhubu.top/gtdogcbrel.html

[N09] 栈与队列
来源：http://hz.daxiang520.top/gtutcexcqs.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.guannengcc.top/gtlbflhgwp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.zdqjudy.top/gtchgtczom.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.snrcjt.cn/gtstbmrvdr.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.feifeiyinyue.top/gtfawiahfa.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yonumen.top/gtmvdadgxb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.0kj1m.cn/gtsrjrfzwp.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.dianchejie.cn/gttzkbznav.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.tanke756.top/gtdskiiuaa.html

[N10] 链表节点定义
来源：http://hz.tianlin.xyz/gttftawkfw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.xziqi.cn/gtrjtordzq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.yueranfly.top/gtginujhoh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.sxryk.cn/gtizgxhjph.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.hongshengwenyu.top/gtrxurkahq.html

Java: class Node { int v; Node next; }
来源：http://hz.zhongyouzk.top/gtksbzsyvj.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.yueranfly.top/gtcmfnspgk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.cdnleiting.top/gtdhtvttev.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.shanyushiyangtech.top/gtyiewbplm.html

[N11] 二叉树中序遍历
来源：http://hz.jiagoushi.top/gtajmiiqdo.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.gzhubu.top/gtxuiwlwlo.html

PHP:  // 手写递归函数
来源：http://hz.tianlin.xyz/gtnrxnmlid.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.pycfn.com/gtwsxiunsz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hnqzz.top/gtrtspwsnl.html

Java: // 手写递归
来源：http://hz.sxryk.cn/gtoebvxqti.html

Go:   // 手写递归
来源：http://hz.guowangkeji.top/gtdzcgasoq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.jiagoushi.top/gthnoshbnj.html

C#:   // 手写递归
来源：http://hz.jqgfzy.top/gtavmvsapz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.chenlongwang.top/gtkytacync.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.jlsjyb.cn/gthihbqyky.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.ywan-chungtsiang.top/gtdrzxdhpl.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yongpay.top/gtdwdrhupt.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jqgfzy.top/gtllccgvzl.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ybcxt.top/gtvdhguyyj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.ydzc1.top/gtkyxhbgdo.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.hnqzz.top/gttfzrzrze.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yanxiufei.cn/gttdnuzcrc.html

================================================================================
来源：http://hz.cucudq.cn/gtrudnapvu.html

O. 并发与异步
来源：http://hz.yuanzhike.top/gtsxqqantn.html

================================================================================
来源：http://hz.hnqzz.top/gtqtomfprh.html

[O01] 启动一个线程
来源：http://hz.ybcxt.top/gtlgiacsog.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.tanke756.top/gtyxqazzkf.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.shangyingyoupin.top/gtoxvossvd.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.xuanzx.com/gtnjnuiore.html

TS:   // 同 JS
来源：http://hz.ywan-chungtsiang.top/gtkgegvmbq.html

Java: new Thread(() -> f()).start()
来源：http://hz.zdqjudy.top/gtrdmybvgr.html

Go:   go f()
来源：http://hz.pengpengdd.cyou/gtgltumbze.html

Ruby: Thread.new { f }
来源：http://hz.guowangkeji.top/gtmlvwuxrz.html

C#:   Task.Run(() => F());
来源：http://hz.chenzaomai.com/gtshcfdjav.html

[O02] 使用线程池
来源：http://hz.sufxvd.cn/gtgvhbibdp.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.0kj1m.cn/gtraarxxuy.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.sysykeji.top/gtnuydstxb.html

JS:   // worker_threads 线程池
来源：http://hz.mhx1999.top/gtbqqookho.html

TS:   // worker_threads 线程池
来源：http://hz.cdnleiting.top/gtlssukdcp.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.jyoumei.cn/gtyfsdhdie.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.sweek.top/gtxuoxqxup.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.jinyuanbaomall.cn/gtulntchir.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.gotoacloud.top/gtmtbjpopt.html

[O03] 加锁保护共享数据
来源：http://hz.cucudq.cn/gtzxswbrrd.html

Py:   with lock: shared += 1
来源：http://hz.guannengcc.top/gtakinucpz.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.9152youxi.cn/gttmgojazn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.jinghuilouyu.cn/gtvuetdyth.html

TS:   // 同 JS
来源：http://hz.tianlin.xyz/gtauikzexp.html

Java: synchronized (this) { shared++; }
来源：http://hz.0kj1m.cn/gtsewyoygf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.fzhhl.top/gtitqfgljw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.cucudq.cn/gtilawcusl.html

C#:   lock (gate) { shared++; }
来源：http://hz.tianlin.xyz/gtnbibqbbe.html

[O04] 定义异步函数并等待
来源：http://hz.jinghuilouyu.cn/gtmkaxwhas.html

Py:   async def f():⏎    await g()
来源：http://hz.hnxiangtu.top/gttbtpyxjz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.xziqi.cn/gtkbuaugif.html

JS:   async function f() { await g(); }
来源：http://hz.wangshuangyany.cn/gttvrxyqrj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.shangyingyoupin.top/gtuhvdjxuq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.shuidangran.top/gtutqsorqi.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.shuidangran.top/gtlenjwxjb.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yj202588.top/gtaimvzdco.html

C#:   async Task F() { await G(); }
来源：http://hz.ehwqpu.com/gtzikzkkfg.html

[O05] 并发执行并等待全部完成
来源：http://hz.hnqzz.top/gthspaqiwz.html

Py:   asyncio.gather(*tasks)
来源：http://hz.iojbl.cn/gtymqcwqzv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.ppjwa.cn/gtylapwhpn.html

JS:   await Promise.all(tasks)
来源：http://hz.jyoumei.cn/gtrhcowkog.html

TS:   await Promise.all(tasks)
来源：http://hz.316326.xyz/gtzludgebl.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.xziqi.cn/gtpjgctirp.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.ehwqpu.com/gtrqvjkpev.html

Ruby: threads.map(&:join)
来源：http://hz.meibo888.top/gtuunxwiuv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yonumen.top/gtvktbcrqr.html

[O06] 使用进程池
来源：http://hz.yanxiufei.cn/gtphpculfa.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.nanxinkj.top/gtvvrlzygu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.wangshuangyany.cn/gtdwrrukjl.html

JS:   // child_process / cluster 模块
来源：http://hz.zhaomingkeji.xyz/gttkmsfqnm.html

TS:   // child_process / cluster 模块
来源：http://hz.wangdashe.top/gtliveksjy.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jianghu66.top/gtvlefguey.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.ydjk.org.cn/gtlzxtlcvw.html

Ruby: // fork 块
来源：http://hz.shangyingyoupin.top/gthkutxqyr.html

C#:   Parallel.For
来源：http://hz.xuanzx.com/gtokxqklib.html

================================================================================
来源：http://hz.ppjwa.cn/gtuasieqav.html

P. 常用工具函数
来源：http://hz.cheryme.top/gtjdcutecz.html

================================================================================
来源：http://hz.redwolf501.top/gtwhfbwumt.html

[P01] 生成 UUID
来源：http://hz.chenlongwang.top/gtieffegvu.html

Py:   str(uuid.uuid4())
来源：http://hz.iojbl.cn/gtvoxogsis.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.dashuyun.cn/gtaxbixeli.html

JS:   crypto.randomUUID()
来源：http://hz.fzhhl.top/gtmzzqsiip.html

TS:   crypto.randomUUID()
来源：http://hz.pengpengdd.cyou/gtezpgyigb.html

Java: UUID.randomUUID().toString()
来源：http://hz.sufxvd.cn/gtqzdkcfjy.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yj20258.top/gtepgkezpx.html

Ruby: SecureRandom.uuid
来源：http://hz.xinyue.icu/gtpjzwzjzb.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.feifeiyinyue.top/gtjpzimyeo.html

[P02] MD5 / SHA256 摘要
来源：http://hz.andypj.xyz/gtfqigihpk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.xingfuxueyuan.xyz/gtfwvjgxnr.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.zhaomingkeji.xyz/gtlhbbkhzj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.gaohongyu789.top/gthsowjhjc.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.pengpengdd.cyou/gtdobzfagw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.hywenlv.cn/gtswsiekjd.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.yvedp.cn/gtsdaasrlm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.chenjidiqi.icu/gtxiflevqk.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.tian-w.cn/gtcgctzgkc.html

[P03] 生成短随机字符串
来源：http://hz.gaohongyu789.top/gtrnqqcfhm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.xuetiantiany.cn/gtdrwqouua.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.hammf.cn/gtjbhucpea.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.pycfn.com/gtcfyzuaue.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.cqqwz.cn/gtsedpzsuc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yonumen.top/gtruhvnopc.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.jinqigfzy.top/gtjvskokca.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jqgufenzy.top/gtehxbiuux.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.ivvv.top/gtvdovqcmz.html

[P04] 求长度
来源：http://hz.sxryk.cn/gtbxcitqfl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.nanxinkj.top/gtvbfueijw.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.gotoacloud.top/gtowtuqqfe.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hywenlv.cn/gtttnkkmbv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.shuidangran.top/gtursppxdz.html

Java: list.size();  map.size();  s.length()
来源：http://hz.havefunace.top/gtrqdlnjfv.html

Go:   len(arr);  len(m)
来源：http://hz.vqdsnc.cn/gtmogtixww.html

Ruby: x.length;  x.size
来源：http://hz.cdnleiting.top/gtibuvomkx.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.xuetiantiany.cn/gtuuwrbknf.html

[P05] 判断两个对象内容是否相等
来源：http://hz.pycfn.com/gtjrnqqido.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.hysaishi.cn/gtleiiabxw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.zdqjudy.top/gtkgbxnstu.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.mhx1999.top/gtlyilsrui.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.cdnleiting.top/gtkoohebou.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.zhijiandao.cn/gtuknakzud.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.zhengqikj.top/gtkhwjwnzo.html

Ruby: a == b
来源：http://hz.fengsongda.top/gtfijhznnt.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.iojbl.cn/gtxuzyarhu.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.zhongyouzk.top/gtltzqvwoy.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.hnqzz.top/gtxvysxqod.html

PHP:  if (empty($x)) {}
来源：http://hz.jlsjyb.cn/gtfhyefoir.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.ehwqpu.com/gtveuipdvw.html

TS:   if (x == null) {}
来源：http://hz.zhoulong.xyz/gtkjfyeejq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.xuetiantiany.cn/gtzxfuxfbh.html

Go:   if x == nil {}
来源：http://hz.ppjwa.cn/gtghhdciol.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.haohaochexian.top/gtxgrgqpjx.html

C#:   if (x is null) {}
来源：http://hz.yj20258888.top/gtbbbopvdb.html

[P07] 防抖与节流
来源：http://hz.xingfuxueyuan.xyz/gtvmmhmwvk.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.sweek.top/gttoqeifdp.html

PHP:  // 手写时间戳比较
来源：http://hz.hfpthk.cn/gthwkgmzyc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hnqzz.top/gtxohicpqi.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hongshengwenyu.top/gttztrgjkb.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.kuanghao11.cn/gtoexdsjww.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.xuetiantiany.cn/gtytuqmweg.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.wangdashe.top/gthnqupeen.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.aibaodan.cn/gtpjsmvtqr.html

[P08] 处理浮点精度问题
来源：http://hz.ehwqpu.com/gttsftykcz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.xingfuxueyuan.xyz/gtcgaqgxse.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.jqgufenzy.top/gtnryxqwjq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.zycfv.cn/gtrztubacd.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.xinyue.icu/gtkiyszawv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yongpay.top/gtogxjwgrq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.wangshuangyany.cn/gtgotorcsk.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.0kj1m.cn/gteedhbwxv.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.hnxiangtu.top/gtsreyvtsp.html

================================================================================
来源：http://hz.snrcjt.cn/gtpfkibtrl.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.xuanzx.com/gtlnocpcgg.html

================================================================================
来源：http://hz.nanxinkj.top/gtardugmfk.html

[Q01] 创建表
来源：http://hz.zhengqikj.top/gtmurqwodp.html

CREATE TABLE users (
来源：http://hz.chenlongwang.top/gtrflkoyui.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hongshengwenyu.top/gtvijgftbl.html

name VARCHAR(50) NOT NULL,
来源：http://hz.jinyuanbaomall.cn/gtjvvlelxz.html

email VARCHAR(100) UNIQUE,
来源：http://hz.birdmap.top/gtoiqkodcs.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.ydzc1.top/gtsqlhbhbs.html

);
来源：http://hz.wangshuangyany.cn/gtpqgewmuj.html

[Q02] 创建带外键的表
来源：http://hz.zycfv.cn/gtblqbcrgs.html

CREATE TABLE orders (
来源：http://hz.redwolf501.top/gtejzoqdnl.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.guannengcc.top/gtnqfxyqcv.html

user_id INT NOT NULL,
来源：http://hz.gogol.net.cn/gtjyeaqvyg.html

amount DECIMAL(10, 2),
来源：http://hz.snrcjt.cn/gtpmbeuzcr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.shzxlz.cn/gtrgicaaiq.html

);
来源：http://hz.sxryk.cn/gtglhwzwnz.html

[Q03] 增加列
来源：http://hz.zhengqikj.top/gteuwfoypo.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.zhengqikj.top/gtbndrbegd.html

[Q04] 修改列类型
来源：http://hz.yj20258.top/gttqhvnkoi.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.chenzaomai.com/gtkxpprcef.html

[Q05] 重命名列
来源：http://hz.ywan-chungtsiang.top/gtgnomhdmj.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.hysaishi.cn/gtubwqeyfk.html

[Q06] 删除列
来源：http://hz.shuidangran.top/gtrrqdydbt.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.sweek.top/gthdgbulkp.html

[Q07] 删除表
来源：http://hz.cucudq.cn/gtjmxcgoxl.html

DROP TABLE IF EXISTS orders;
来源：http://hz.jianghu66.top/gtxvxdpulx.html

[Q08] 创建普通索引
来源：http://hz.wangdashe.top/gtslsbhbxl.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.0kj1m.cn/gtszzclvqa.html

[Q09] 创建唯一索引
来源：http://hz.jinqigfzy.top/gtafcmldjr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.yueranfly.top/gtknzmgiby.html

[Q10] 插入单行
来源：http://hz.chenzaomai.com/gtlmytyikd.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.chenjidiqi.icu/gtxlhwybtj.html

[Q11] 一次插入多行
来源：http://hz.dianchejie.cn/gtwoyuiegs.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.tian-w.cn/gtavtjihyx.html

[Q12] 插入后取自增 ID
来源：http://hz.jinqigufen.top/gtaxfkfyrw.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.sweek.top/gtcddkptmn.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.kuanghao11.cn/gtftamdkps.html

[Q13] 忽略重复插入
来源：http://hz.gaohongyu789.top/gtbbgrfbij.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.hnqzz.top/gtqdnvpprk.html

[Q14] 存在则更新（upsert）
来源：http://hz.dianchejie.cn/gtnapvsyue.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.yanxiufei.cn/gtirfqyqnm.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.jyoumei.cn/gtumojorpq.html

[Q15] 查询全部
来源：http://hz.nwbrower.top/gtmsaicxrd.html

SELECT * FROM users;
来源：http://hz.nanxuanxn.top/gtgehxgqcc.html

[Q16] 查询指定列
来源：http://hz.yanxiufei.cn/gtxliswpnv.html

SELECT id, name FROM users;
来源：http://hz.bjfxy.top/gtkwiwgivs.html

[Q17] 条件查询
来源：http://hz.aibaodan.cn/gtqmxhkrxb.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.yueranfly.top/gtywcjhvef.html

[Q18] 模糊匹配
来源：http://hz.pycfn.com/gtpugmxamz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.guowangkeji.top/gthsbnmpqn.html

[Q19] 范围查询
来源：http://hz.cqqwz.cn/gtwiqnuzqq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.jinyuanbaomall.cn/gtrwylcpnr.html

[Q20] IN 列表
来源：http://hz.cqqwz.cn/gtzlfcyroq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.jianghu66.top/gtlznareus.html

[Q21] 空值判断
来源：http://hz.hywenlv.cn/gtufpvziqs.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.bjfxy.top/gtgjdjarey.html

[Q22] 排序
来源：http://hz.yuanzhike.top/gtxtujssmw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.yj20258.top/gtqkwulqlu.html

[Q23] 分页
来源：http://hz.redwolf501.top/gtkpkeoecm.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.xuanzx.com/gtsrsscfgs.html

[Q24] 去重
来源：http://hz.zdqjudy.top/gtbxfxvsqw.html

SELECT DISTINCT city FROM users;
来源：http://hz.meibo888.top/gtxfvzzbae.html

[Q25] 只取前 N 条
来源：http://hz.aizwys.cn/gtqdfurdjf.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.ppjwa.cn/gtbgmrajuv.html

[Q26] 计数
来源：http://hz.yj20258888.top/gtlimhgdur.html

SELECT COUNT(*) FROM users;
来源：http://hz.hysaishi.cn/gtbuyddarq.html

[Q27] 条件计数
来源：http://hz.jinyuanbaomall.cn/gtutgxmiid.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.mhx1999.top/gtjdonznbo.html

[Q28] 求和与平均
来源：http://hz.bjfxy.top/gtfcxfxxyc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.haohaochexian.top/gtngboarva.html

[Q29] 最大最小值
来源：http://hz.daxiang520.top/gtubbxumjw.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.ivvv.top/gtxjuqmylc.html

[Q30] 分组统计
来源：http://hz.birdmap.top/gtdnivtnpj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.redwolf501.top/gtblhtuoqs.html

[Q31] 分组后过滤
来源：http://hz.chenlongwang.top/gtqicrpizs.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.sweek.top/gtiwhkdffs.html

[Q32] 分组拼接字符串
来源：http://hz.jinyuanbaomall.cn/gtwmykzujl.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.ywan-chungtsiang.top/gtipxpygtd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.wangshuangyany.cn/gtjugjkzgu.html

[Q33] 多列分组
来源：http://hz.ybcxt.top/gtsuafcbsa.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.redwolf501.top/gtjlrczgsq.html

[Q34] 每组取第一条
来源：http://hz.jyoumei.cn/gthlhqdgtv.html

SELECT * FROM (
来源：http://hz.hongshengwenyu.top/gtzmjuamql.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.cdnleiting.top/gteurhuxtf.html

) t WHERE rn = 1;
来源：http://hz.birdmap.top/gtrlchhqhk.html

[Q35] 内连接
来源：http://hz.jinqigufen.top/gtlqyjlwjd.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.guowangkeji.top/gtsqgnoydm.html

[Q36] 左连接
来源：http://hz.sufxvd.cn/gtgrvxogpl.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhiwuduotai.top/gtgubrbpai.html

[Q37] 右连接
来源：http://hz.pycfn.com/gttrjyyqmr.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jianghu66.top/gtobppqfxo.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.wangdashe.top/gtjhjpoodw.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.fzhhl.top/gtehkcvrfo.html

[Q39] 自连接（查上下级）
来源：http://hz.jyoumei.cn/gtheemcctu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.pengpengdd.cyou/gtdksjkvog.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.zhaomingkeji.xyz/gtltpwttpo.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.ehwqpu.com/gtrlagzhfi.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.jyoumei.cn/gtphjxemac.html

[Q41] 多表连接
来源：http://hz.shangyingyoupin.top/gtdbhxcboi.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.ydzc1.top/gtptutscfp.html

JOIN users u ON u.id = o.user_id
来源：http://hz.yj20258888.top/gtplhnidnh.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.zhengqikj.top/gtvabnhzil.html

[Q42] 连接条件附加过滤
来源：http://hz.ybcxt.top/gtelqhbrok.html

SELECT u.name, o.amount FROM users u
来源：http://hz.xuanzx.com/gtwpjxixkt.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.sxryk.cn/gtvuoeysxu.html

[Q43] 标量子查询
来源：http://hz.jinyuanbaomall.cn/gtwbtfpwcv.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yuxming.cn/gtnhkkbpsx.html


<!-- 参考信息 -->