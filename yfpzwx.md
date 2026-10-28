代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://hz.hammf.cn/gtaldypetd.html

TS:   s === [...s].reverse().join("")
来源：http://hz.sxryk.cn/gtyldicjlb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jianghu66.top/gtbmonrers.html

Go:   // 双指针从两端比较
来源：http://hz.hnqzz.top/gtclcygtuk.html

Ruby: s == s.reverse
来源：http://hz.zhongyouzk.top/gtelgcmtlx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.svipenyu.cn/gtumbebnww.html

[N07] 两数之和（返回下标）
来源：http://hz.iojbl.cn/gtginlzhkh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.pycfn.com/gtoemexzig.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.chenzaomai.com/gtsogqptul.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.ywan-chungtsiang.top/gtsotsrugu.html

TS:   // 手写 Map<string, number>
来源：http://hz.316326.xyz/gthttxskbv.html

Java: // 手写 HashMap
来源：http://hz.gogol.net.cn/gtocstquct.html

Go:   // 手写 map[int]int
来源：http://hz.jiagoushi.top/gtwzodiaqy.html

Ruby: // 手写 Hash
来源：http://hz.zdqjudy.top/gtkkehdegc.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.guannengcc.top/gtroxpjcyh.html

[N08] 生成全排列
来源：http://hz.gzhubu.top/gtrusyohxh.html

Py:   itertools.permutations(arr)
来源：http://hz.zhongyouzk.top/gtxrigtpuf.html

PHP:  // 手写递归交换
来源：http://hz.jyoumei.cn/gtrqxcjzqx.html

JS:   // 手写回溯递归
来源：http://hz.zhixingplan.top/gttwqebapx.html

TS:   // 手写回溯递归
来源：http://hz.jinghuilouyu.cn/gtcufndwhf.html

Java: // 手写回溯递归
来源：http://hz.yj20258.top/gtqmbmpvfr.html

Go:   // 手写回溯递归
来源：http://hz.jqgufenzy.top/gtijctnnad.html

Ruby: arr.permutation.to_a
来源：http://hz.gogol.net.cn/gtytjipstp.html

C#:   // 手写回溯递归
来源：http://hz.cdnleiting.top/gtkzxuougg.html

[N09] 栈与队列
来源：http://hz.hongshengwenyu.top/gtfrblrxun.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.nwbrower.top/gtkxioupfh.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.havefunace.top/gtzmsfcoam.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.jlsjyb.cn/gthqcixekh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.zhijiandao.cn/gtyhqutirc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.wangshuangyany.cn/gtwlcbdlou.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.tanke756.top/gtflmkbihg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.ppjwa.cn/gtcinmctqk.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.jinqigufen.top/gtueipjaei.html

[N10] 链表节点定义
来源：http://hz.quarkkingdee.top/gtkauuucjw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.jiagoushi.top/gtisljiyex.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.pengpengdd.cyou/gtuywlxncv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.pycfn.com/gtfaehqxws.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.redwolf501.top/gtwbuvdpyb.html

Java: class Node { int v; Node next; }
来源：http://hz.svipenyu.cn/gtwpreyqpg.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.ydjk.org.cn/gteyrppcwc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.aibaodan.cn/gtdllzuffc.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.shangyingyoupin.top/gtzcnmeqle.html

[N11] 二叉树中序遍历
来源：http://hz.daria6918.cn/gtyohqcgaf.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.tianlin.xyz/gtnzebzeul.html

PHP:  // 手写递归函数
来源：http://hz.chenjidiqi.icu/gtrzmbcjde.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yangfankeji.com/gtpsxcevbo.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.xingfuxueyuan.xyz/gtjdldbmne.html

Java: // 手写递归
来源：http://hz.dashuyun.cn/gtxubjgfqf.html

Go:   // 手写递归
来源：http://hz.shuidangran.top/gtoanfmrps.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.hnqzz.top/gtecxrxmby.html

C#:   // 手写递归
来源：http://hz.mhx1999.top/gtcnnhfljp.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yueranfly.top/gtelgymddr.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.shangyingyoupin.top/gtjhoyzxbi.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.hysaishi.cn/gteiucptik.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.shanyushiyangtech.top/gttsbdqztp.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.sufxvd.cn/gtcgkvscxf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.tanke756.top/gtdwosshky.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.tanke756.top/gtsneaoblq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.fzhhl.top/gtunwvrcsj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.guowangkeji.top/gtvmojmacl.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtwiuvmvck.html

O. 并发与异步
来源：http://hz.gaohongyu789.top/gtvrjczydh.html

================================================================================
来源：http://hz.wangdashe.top/gtchgxosyv.html

[O01] 启动一个线程
来源：http://hz.guannengcc.top/gtaualirao.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.jianghu66.top/gtyhrizdpo.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.kuanghao11.cn/gtvnkdzuea.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.daxiang520.top/gtqczjeumk.html

TS:   // 同 JS
来源：http://hz.xuetiantiany.cn/gtkfncorsu.html

Java: new Thread(() -> f()).start()
来源：http://hz.xingfuxueyuan.xyz/gtiftageew.html

Go:   go f()
来源：http://hz.fzhhl.top/gtyifhpzys.html

Ruby: Thread.new { f }
来源：http://hz.jianghu66.top/gtanpqzkfn.html

C#:   Task.Run(() => F());
来源：http://hz.jiagoushi.top/gtddenvrdj.html

[O02] 使用线程池
来源：http://hz.kuanghao11.cn/gtuddxucpj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.c1oappe.top/gtvgzwfemp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.smart0.xyz/gtrvzjqdxk.html

JS:   // worker_threads 线程池
来源：http://hz.zhongyouzk.top/gteqvdcohb.html

TS:   // worker_threads 线程池
来源：http://hz.jyoumei.cn/gtnfoutyzc.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.zdqjudy.top/gtvzuocfsq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.daria6918.cn/gtgwdmzyhj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.wangshuangyany.cn/gtuthdazqn.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.tian-w.cn/gthngrwdmq.html

[O03] 加锁保护共享数据
来源：http://hz.cucudq.cn/gtcxhfhlsw.html

Py:   with lock: shared += 1
来源：http://hz.yuanzhike.top/gthnkuwwqs.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.xuanzx.com/gtyilfklyv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.jiagoushi.top/gtzkrvibno.html

TS:   // 同 JS
来源：http://hz.sysykeji.top/gtaeosrqkx.html

Java: synchronized (this) { shared++; }
来源：http://hz.yonumen.top/gtqtzgllxo.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.aizwys.cn/gteyqildyy.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.dashuyun.cn/gtoduvpiyx.html

C#:   lock (gate) { shared++; }
来源：http://hz.jqgfzy.top/gtlthjcjxt.html

[O04] 定义异步函数并等待
来源：http://hz.sweek.top/gtmkecpobd.html

Py:   async def f():⏎    await g()
来源：http://hz.aizwys.cn/gtlwycqkxt.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jqgufenzy.top/gtybuloecu.html

JS:   async function f() { await g(); }
来源：http://hz.mhx1999.top/gtiolrqwtb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yvedp.cn/gtwgnqkpff.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.yj20258.top/gteooiydic.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.yanxiufei.cn/gtnesfordn.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.jqgufenzy.top/gttyqaxbob.html

C#:   async Task F() { await G(); }
来源：http://hz.gzhubu.top/gtjrvulwru.html

[O05] 并发执行并等待全部完成
来源：http://hz.svipenyu.cn/gtzeogtcxx.html

Py:   asyncio.gather(*tasks)
来源：http://hz.sweek.top/gtieskpgqi.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.zhixingplan.top/gtzujjlizp.html

JS:   await Promise.all(tasks)
来源：http://hz.yj20258888.top/gtihnnargo.html

TS:   await Promise.all(tasks)
来源：http://hz.yj20258.top/gtbdmazowi.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.jinyuanbaomall.cn/gtpqdndcgf.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.gogol.net.cn/gtpoksmoae.html

Ruby: threads.map(&:join)
来源：http://hz.cucudq.cn/gtemfesrnx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.haohaochexian.top/gthuieppfj.html

[O06] 使用进程池
来源：http://hz.shanyushiyangkeji.top/gttoexazrz.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.hfpthk.cn/gtlwlrdeqb.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.jinyuanbaomall.cn/gteffknqhz.html

JS:   // child_process / cluster 模块
来源：http://hz.cdnleiting.top/gtmopiiots.html

TS:   // child_process / cluster 模块
来源：http://hz.daria6918.cn/gtffvqzosl.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.nanxinkj.top/gtmglnsyrx.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.jinyuanbaomall.cn/gtliqdckgd.html

Ruby: // fork 块
来源：http://hz.shuidangran.top/gtvtbowwkr.html

C#:   Parallel.For
来源：http://hz.haohaochexian.top/gtplfficnu.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtwhedtlhm.html

P. 常用工具函数
来源：http://hz.9152youxi.cn/gtoeabrjln.html

================================================================================
来源：http://hz.yueranfly.top/gtpcqqcsjw.html

[P01] 生成 UUID
来源：http://hz.xziqi.cn/gtryfvkidq.html

Py:   str(uuid.uuid4())
来源：http://hz.quarkkingdee.top/gtmvktmjes.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.sxryk.cn/gtluwxkomf.html

JS:   crypto.randomUUID()
来源：http://hz.snrcjt.cn/gtnyfovvdx.html

TS:   crypto.randomUUID()
来源：http://hz.haohaochexian.top/gtdxycqopo.html

Java: UUID.randomUUID().toString()
来源：http://hz.ydjk.org.cn/gtzmilmfhe.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yongpay.top/gtwweajkot.html

Ruby: SecureRandom.uuid
来源：http://hz.meibo888.top/gtttgtxihp.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.yueranfly.top/gttwevbjbi.html

[P02] MD5 / SHA256 摘要
来源：http://hz.shzxlz.cn/gtyehuxsoh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.ybcxt.top/gtjylvhkbp.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.zhongyouzk.top/gtojonrurf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.quarkkingdee.top/gttcxincaa.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.daxiang520.top/gtuwgdiffx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.nanxinkj.top/gttbkdlrys.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.yvedp.cn/gttxdiguin.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.tanke756.top/gtvfkizifn.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.daxiang520.top/gttumqarln.html

[P03] 生成短随机字符串
来源：http://hz.cucudq.cn/gtdzyftvzi.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.wangdashe.top/gtbclzzgac.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.dianchejie.cn/gtgutcafny.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.cqqwz.cn/gtmuccrfnc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.redwolf501.top/gtwwgpiscd.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.zhengqikj.top/gtpnedteqb.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.xinyue.icu/gtavfwzeuy.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.birdmap.top/gtsveshjbb.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.sxryk.cn/gthgivejrt.html

[P04] 求长度
来源：http://hz.zhiwuduotai.top/gtxonovahy.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.kuanghao11.cn/gtusyrjqbr.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhongyouzk.top/gtrilqmnfm.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.bjfxy.top/gtgpxtldaq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jlsjyb.cn/gtckuruziy.html

Java: list.size();  map.size();  s.length()
来源：http://hz.9152youxi.cn/gtfwtnsjkh.html

Go:   len(arr);  len(m)
来源：http://hz.316326.xyz/gttasmeihv.html

Ruby: x.length;  x.size
来源：http://hz.shanyushiyangtech.top/gtepgsjmup.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.hywenlv.cn/gtmuutedmy.html

[P05] 判断两个对象内容是否相等
来源：http://hz.daxiang520.top/gtzmmebnrm.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.shangyingyoupin.top/gtiigkafjm.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.jyoumei.cn/gtmgvssvxk.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.vqdsnc.cn/gtgfvgndzq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.aizwys.cn/gtzdnwqipk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.hammf.cn/gthbqpyclv.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.nanxinkj.top/gtwvkhbtur.html

Ruby: a == b
来源：http://hz.hongshengwenyu.top/gtljmevahv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.jinyuanbaomall.cn/gtlsbnkdvx.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.yongpay.top/gtwcqumopw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.jianghu66.top/gtswitsvvv.html

PHP:  if (empty($x)) {}
来源：http://hz.sweek.top/gtjbeojxmp.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.shanyushiyangtech.top/gtmbqeztwg.html

TS:   if (x == null) {}
来源：http://hz.quarkkingdee.top/gtjreahbsw.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.svipenyu.cn/gtllhbsaoh.html

Go:   if x == nil {}
来源：http://hz.jlsjyb.cn/gtqyizfgnq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.daxiang520.top/gtatldkmcz.html

C#:   if (x is null) {}
来源：http://hz.dianchejie.cn/gtnqbrmvun.html

[P07] 防抖与节流
来源：http://hz.wangdashe.top/gtnzmwskdd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jyoumei.cn/gtpasbmjug.html

PHP:  // 手写时间戳比较
来源：http://hz.xylfe.cn/gtdnghfgzv.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shanyushiyangkeji.top/gtdoztdhxl.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.gotoacloud.top/gtxniuhqej.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.dashuyun.cn/gtypxntyfm.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.hnxiangtu.top/gteehlsgjh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.52xcode.cn/gtshhiicra.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.pycfn.com/gtxvhixmhp.html

[P08] 处理浮点精度问题
来源：http://hz.daxiang520.top/gtwxhkgwtu.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.c1oappe.top/gtnuegbjjf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.yanxiufei.cn/gtxxkscafn.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.jqgfzy.top/gtfzleuufy.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.bjfxy.top/gtowfffzoh.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.52xcode.cn/gtfikjlcau.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.zhoulong.xyz/gtdvwbklkb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.guannengcc.top/gtdvndqfty.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.cucudq.cn/gtpgopaeef.html

================================================================================
来源：http://hz.ivvv.top/gtbkcdpejo.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.cqqwz.cn/gtjwvgfied.html

================================================================================
来源：http://hz.wangdashe.top/gtjdeodous.html

[Q01] 创建表
来源：http://hz.ybcxt.top/gtseqivqfl.html

CREATE TABLE users (
来源：http://hz.snrcjt.cn/gtkbfrrska.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jlsjyb.cn/gtcxqvayeb.html

name VARCHAR(50) NOT NULL,
来源：http://hz.zhixingplan.top/gteuokaoeu.html

email VARCHAR(100) UNIQUE,
来源：http://hz.sxryk.cn/gtsctwwioh.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.xinyue.icu/gtlvabdgxg.html

);
来源：http://hz.havefunace.top/gtqmlkjwwq.html

[Q02] 创建带外键的表
来源：http://hz.vqdsnc.cn/gtgwjavqmf.html

CREATE TABLE orders (
来源：http://hz.gaohongyu789.top/gtusyoopyv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ydzc1.top/gtnjhjvbww.html

user_id INT NOT NULL,
来源：http://hz.0kj1m.cn/gttsnfkoiw.html

amount DECIMAL(10, 2),
来源：http://hz.hywenlv.cn/gtooovpmgx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.zdqjudy.top/gtcswbamjn.html

);
来源：http://hz.jyoumei.cn/gtjiswvzpg.html

[Q03] 增加列
来源：http://hz.vqdsnc.cn/gtjohcfeib.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.jlsjyb.cn/gtosbxtycc.html

[Q04] 修改列类型
来源：http://hz.sxryk.cn/gtdbsvixhw.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.yj20258888.top/gttorwfxru.html

[Q05] 重命名列
来源：http://hz.jlsjyb.cn/gtfiepmisf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.hammf.cn/gtdepopkbp.html

[Q06] 删除列
来源：http://hz.shzxlz.cn/gturegnpoj.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.yj202588.top/gtnsjribfn.html

[Q07] 删除表
来源：http://hz.jiagoushi.top/gtpqbsfuys.html

DROP TABLE IF EXISTS orders;
来源：http://hz.hfpthk.cn/gtrtabkicv.html

[Q08] 创建普通索引
来源：http://hz.pycfn.com/gtaqdldhjm.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.9152youxi.cn/gtukbdvxop.html

[Q09] 创建唯一索引
来源：http://hz.ybcxt.top/gtpuusgoje.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.jinqigufen.top/gtucwloflj.html

[Q10] 插入单行
来源：http://hz.cucudq.cn/gtpchclahc.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.aizwys.cn/gtajfelhcj.html

[Q11] 一次插入多行
来源：http://hz.yuxming.cn/gtyoypgvbl.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.pycfn.com/gtfjgvgthn.html

[Q12] 插入后取自增 ID
来源：http://hz.meibo888.top/gtmxqxxkfp.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.ywan-chungtsiang.top/gtcdyjuhov.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.nanxinkj.top/gtkrntsmxc.html

[Q13] 忽略重复插入
来源：http://hz.zhoulong.xyz/gtltdlyftx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.pycfn.com/gtopbnawmr.html

[Q14] 存在则更新（upsert）
来源：http://hz.andypj.xyz/gtopjpfqzu.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.sysykeji.top/gthojpfvln.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.ydjk.org.cn/gtofvelicm.html

[Q15] 查询全部
来源：http://hz.smart0.xyz/gtyzmsiwyz.html

SELECT * FROM users;
来源：http://hz.yuanzhike.top/gtnvonwqsp.html

[Q16] 查询指定列
来源：http://hz.jianghu66.top/gtszdzwzdm.html

SELECT id, name FROM users;
来源：http://hz.zhaomingkeji.xyz/gtqxuvzaae.html

[Q17] 条件查询
来源：http://hz.yangfankeji.com/gtcazqmuqd.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.dianchejie.cn/gtxhwxlofs.html

[Q18] 模糊匹配
来源：http://hz.zhixingplan.top/gturroyshe.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.cqqwz.cn/gtarfiywon.html

[Q19] 范围查询
来源：http://hz.dashuyun.cn/gtbquuhvdw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.redwolf501.top/gtthhcxebi.html

[Q20] IN 列表
来源：http://hz.bjfxy.top/gtcjuhfemp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yueranfly.top/gteqvaqbnh.html

[Q21] 空值判断
来源：http://hz.shanyushiyangkeji.top/gtsjutxzlh.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.guannengcc.top/gtrhjawixw.html

[Q22] 排序
来源：http://hz.haohaochexian.top/gtgklyqtdy.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.bjfxy.top/gtczkadnsf.html

[Q23] 分页
来源：http://hz.jinyuanbaomall.cn/gtxvghnish.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yanxiufei.cn/gtvvaigxnc.html

[Q24] 去重
来源：http://hz.zhaomingkeji.xyz/gtjdmgzhnt.html

SELECT DISTINCT city FROM users;
来源：http://hz.zhiwuduotai.top/gtncnpbpjh.html

[Q25] 只取前 N 条
来源：http://hz.yongpay.top/gtqtwajlxp.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.zhaomingkeji.xyz/gthzbroijt.html

[Q26] 计数
来源：http://hz.ivvv.top/gtsehsppwn.html

SELECT COUNT(*) FROM users;
来源：http://hz.shanyushiyangtech.top/gtrgxofiof.html

[Q27] 条件计数
来源：http://hz.yvedp.cn/gtsxjacixm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.snrcjt.cn/gtfkfolobi.html

[Q28] 求和与平均
来源：http://hz.52xcode.cn/gtquybouwx.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.iojbl.cn/gtviomltjn.html

[Q29] 最大最小值
来源：http://hz.cashguo.top/gtvvwlckqo.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.gaohongyu789.top/gtabopvemy.html

[Q30] 分组统计
来源：http://hz.yj20258888.top/gthtpfvjdr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.yangfankeji.com/gttwiukdie.html

[Q31] 分组后过滤
来源：http://hz.dianchejie.cn/gtufrtmpyr.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.316326.xyz/gtkamrbvki.html

[Q32] 分组拼接字符串
来源：http://hz.jinqigfzy.top/gtxlgrokhl.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.kuanghao11.cn/gthrgkdllq.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.birdmap.top/gtffymumfz.html

[Q33] 多列分组
来源：http://hz.mhx1999.top/gtstrpsiot.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.jyoumei.cn/gtsoiokans.html

[Q34] 每组取第一条
来源：http://hz.snrcjt.cn/gtnhkrebvj.html

SELECT * FROM (
来源：http://hz.guowangkeji.top/gtkqckjzpg.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.meibo888.top/gtjmbqybyh.html

) t WHERE rn = 1;
来源：http://hz.fengsongda.top/gtrbnogesp.html

[Q35] 内连接
来源：http://hz.sysykeji.top/gtnvwnzhzq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.ppjwa.cn/gtxnzvbnwn.html

[Q36] 左连接
来源：http://hz.zhijiandao.cn/gtbpptjciw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.vqdsnc.cn/gtqwtvtsbk.html

[Q37] 右连接
来源：http://hz.yanxiufei.cn/gttzwwlmku.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.ydzc1.top/gtbbmeytix.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.hysaishi.cn/gttpopbtnx.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.daxiang520.top/gtjixhdisg.html

[Q39] 自连接（查上下级）
来源：http://hz.gaohongyu789.top/gtygizllod.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jyoumei.cn/gtarjaoqns.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.gogol.net.cn/gtgztscttr.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.hfpthk.cn/gtomhnbmdp.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.dashuyun.cn/gtygjvaqgn.html

[Q41] 多表连接
来源：http://hz.hfpthk.cn/gtileovyvb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.yongpay.top/gtunqewitp.html

JOIN users u ON u.id = o.user_id
来源：http://hz.xziqi.cn/gtekewthlq.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.pycfn.com/gtiiunjcxh.html

[Q42] 连接条件附加过滤
来源：http://hz.yanxiufei.cn/gtvfqbhbll.html

SELECT u.name, o.amount FROM users u
来源：http://hz.fengsongda.top/gtcyjjbzmv.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.jiagoushi.top/gtnighwdxh.html

[Q43] 标量子查询
来源：http://hz.gzhubu.top/gtbvcgohyn.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.wangdashe.top/gtdfsrbjaz.html


<!-- 参考信息 -->