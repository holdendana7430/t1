代发 wailian999

Ruby: s == s.reverse
来源：http://hz.tianlin.xyz/gttnjhptee.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.zhaomingkeji.xyz/gtumyuqrgy.html

[N07] 两数之和（返回下标）
来源：http://hz.sweek.top/gtjdfwbyxb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.gogol.net.cn/gtxtyedmpf.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yj20258888.top/gtkrscoxle.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.ivvv.top/gtvwaorsco.html

TS:   // 手写 Map<string, number>
来源：http://hz.jqgufenzy.top/gtwfmvpyhc.html

Java: // 手写 HashMap
来源：http://hz.nwbrower.top/gtiyjfjkps.html

Go:   // 手写 map[int]int
来源：http://hz.aibaodan.cn/gtncootkzo.html

Ruby: // 手写 Hash
来源：http://hz.gzhubu.top/gtvowttrla.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.ydzc1.top/gtzakbpqrt.html

[N08] 生成全排列
来源：http://hz.zhaomingkeji.xyz/gtcgrvljtt.html

Py:   itertools.permutations(arr)
来源：http://hz.jqgfzy.top/gtdpfvflkz.html

PHP:  // 手写递归交换
来源：http://hz.chenjidiqi.icu/gtzgsxwyet.html

JS:   // 手写回溯递归
来源：http://hz.chenlongwang.top/gtjxnjllru.html

TS:   // 手写回溯递归
来源：http://hz.zhaomingkeji.xyz/gtnkpdphmj.html

Java: // 手写回溯递归
来源：http://hz.ppjwa.cn/gtdelvlqdk.html

Go:   // 手写回溯递归
来源：http://hz.cqqwz.cn/gtflbvwfcf.html

Ruby: arr.permutation.to_a
来源：http://hz.zhiwuduotai.top/gtgpnuaosk.html

C#:   // 手写回溯递归
来源：http://hz.sxryk.cn/gtcadwhplq.html

[N09] 栈与队列
来源：http://hz.mhx1999.top/gtrixirxjk.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.tanke756.top/gtbxibcntb.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.gogol.net.cn/gtmbcvxriu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yj20258888.top/gthsqoyjid.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.gzhubu.top/gtvmbrwhvt.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.shanyushiyangkeji.top/gtqinxhksu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.daria6918.cn/gtgeqcvzjo.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.haohaochexian.top/gtdhhmznhc.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.birdmap.top/gtefngbntz.html

[N10] 链表节点定义
来源：http://hz.jqgufenzy.top/gtborifzmy.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.cheryme.top/gttpivekmm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.cqqwz.cn/gtgpsramex.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.c1oappe.top/gtjnifuvox.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.jqgfzy.top/gticiuavjr.html

Java: class Node { int v; Node next; }
来源：http://hz.cashguo.top/gtkjtyzsxr.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.guannengcc.top/gtquatnswd.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.52xcode.cn/gtfjjvihdd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.shuidangran.top/gtmzjzuivi.html

[N11] 二叉树中序遍历
来源：http://hz.haohaochexian.top/gtjaahvgag.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.jiagoushi.top/gtugslrweg.html

PHP:  // 手写递归函数
来源：http://hz.jinqigfzy.top/gttabvbjpu.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.xuetiantiany.cn/gtwexhxqbu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.cucudq.cn/gthcsgrjwr.html

Java: // 手写递归
来源：http://hz.guannengcc.top/gtmkmpmutm.html

Go:   // 手写递归
来源：http://hz.yuanzhike.top/gtxlqduzhi.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.redwolf501.top/gtkgjgasqb.html

C#:   // 手写递归
来源：http://hz.nanxuanxn.top/gtjbosbeyf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.sxryk.cn/gtczsesrcj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.pengpengdd.cyou/gtckgjwvpe.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.ivvv.top/gtkjbeykqn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.haohaochexian.top/gtrxtdywbe.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.birdmap.top/gtrktfrpfw.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jqgufenzy.top/gtuzezoxfl.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.tanke756.top/gtykghpgdh.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.nanxinkj.top/gtsmdklhhs.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.sysykeji.top/gtogqtmogt.html

================================================================================
来源：http://hz.xinyue.icu/gtqmmdclim.html

O. 并发与异步
来源：http://hz.zdqjudy.top/gtcitkahcf.html

================================================================================
来源：http://hz.ehwqpu.com/gtzdcptphy.html

[O01] 启动一个线程
来源：http://hz.jinqigufen.top/gttemysbyi.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.kuanghao11.cn/gtqvtvvrop.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.haohaochexian.top/gttnahmjdw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.guannengcc.top/gtoxjywtkr.html

TS:   // 同 JS
来源：http://hz.jinqigfzy.top/gtqwrymizy.html

Java: new Thread(() -> f()).start()
来源：http://hz.hfpthk.cn/gtubwlaqzg.html

Go:   go f()
来源：http://hz.hnxiangtu.top/gteqvamipg.html

Ruby: Thread.new { f }
来源：http://hz.c1oappe.top/gtvcuouqoj.html

C#:   Task.Run(() => F());
来源：http://hz.zhiwuduotai.top/gtamsccrpj.html

[O02] 使用线程池
来源：http://hz.birdmap.top/gtlimffgqx.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.xuanzx.com/gtjmtzffsf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.cdnleiting.top/gtwiskgtzj.html

JS:   // worker_threads 线程池
来源：http://hz.jinqigufen.top/gtwncoqqff.html

TS:   // worker_threads 线程池
来源：http://hz.tian-w.cn/gtcsxtvnam.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.hammf.cn/gtimnvsqch.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.tian-w.cn/gtoixizvma.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yueranfly.top/gtstloymsq.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.dianchejie.cn/gtuciwzjjp.html

[O03] 加锁保护共享数据
来源：http://hz.jinqigfzy.top/gtalbsqbmn.html

Py:   with lock: shared += 1
来源：http://hz.shzxlz.cn/gtuxzhpgsz.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.ehwqpu.com/gtmlrdhtbr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.aibaodan.cn/gtvlzlujnk.html

TS:   // 同 JS
来源：http://hz.wangshuangyany.cn/gtotmckivd.html

Java: synchronized (this) { shared++; }
来源：http://hz.quarkkingdee.top/gtwoqihkkt.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.quarkkingdee.top/gtelqyhjqo.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.dashuyun.cn/gtwztisxxk.html

C#:   lock (gate) { shared++; }
来源：http://hz.zhaomingkeji.xyz/gtwocpedll.html

[O04] 定义异步函数并等待
来源：http://hz.tianlin.xyz/gtvmqumldn.html

Py:   async def f():⏎    await g()
来源：http://hz.dashuyun.cn/gtfnbibrzd.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.yvedp.cn/gtdomdahbv.html

JS:   async function f() { await g(); }
来源：http://hz.feifeiyinyue.top/gtwpfoexfd.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.tanke756.top/gtovmywuds.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.ywan-chungtsiang.top/gtqwdkiwdp.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.shangyingyoupin.top/gtkigidnyw.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.feifeiyinyue.top/gtdyhgchje.html

C#:   async Task F() { await G(); }
来源：http://hz.jinqigfzy.top/gtkrdphdeg.html

[O05] 并发执行并等待全部完成
来源：http://hz.meibo888.top/gtdfaximdm.html

Py:   asyncio.gather(*tasks)
来源：http://hz.ppjwa.cn/gtyxbkbtri.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.pengpengdd.cyou/gtncoupdks.html

JS:   await Promise.all(tasks)
来源：http://hz.hnxiangtu.top/gtxycjohak.html

TS:   await Promise.all(tasks)
来源：http://hz.yuanzhike.top/gtrwuvntju.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.sysykeji.top/gtyklrhtya.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.guowangkeji.top/gtnckqvgmb.html

Ruby: threads.map(&:join)
来源：http://hz.cheryme.top/gtdlnghkfi.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.jiagoushi.top/gthlloqyau.html

[O06] 使用进程池
来源：http://hz.haohaochexian.top/gtvcojdofx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.hnxiangtu.top/gtfwiynrtg.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.meibo888.top/gtrfuformo.html

JS:   // child_process / cluster 模块
来源：http://hz.tian-w.cn/gtmchljtlu.html

TS:   // child_process / cluster 模块
来源：http://hz.zhongyouzk.top/gtllrsscjb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.tianlin.xyz/gtyxpgrhhj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.cheryme.top/gtjtdhqcbj.html

Ruby: // fork 块
来源：http://hz.zhijiandao.cn/gtueieaiay.html

C#:   Parallel.For
来源：http://hz.xylfe.cn/gtqrdddvmd.html

================================================================================
来源：http://hz.ybcxt.top/gtcqwjsejb.html

P. 常用工具函数
来源：http://hz.yvedp.cn/gtthbnrmgu.html

================================================================================
来源：http://hz.zhixingplan.top/gtzzaaoohw.html

[P01] 生成 UUID
来源：http://hz.gzhubu.top/gtexefuwgn.html

Py:   str(uuid.uuid4())
来源：http://hz.jlsjyb.cn/gtifgbwael.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jinyuanbaomall.cn/gtxpgetwdd.html

JS:   crypto.randomUUID()
来源：http://hz.mhx1999.top/gtowkjhryn.html

TS:   crypto.randomUUID()
来源：http://hz.yj20258888.top/gtkypvsykb.html

Java: UUID.randomUUID().toString()
来源：http://hz.cucudq.cn/gtxzrmlnok.html

Go:   // 用 github.com/google/uuid
来源：http://hz.shzxlz.cn/gtfvdsjmvg.html

Ruby: SecureRandom.uuid
来源：http://hz.jqgufenzy.top/gtvxodoonq.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.xziqi.cn/gtqlmmlucf.html

[P02] MD5 / SHA256 摘要
来源：http://hz.jqgufenzy.top/gtkldodrxv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.jiagoushi.top/gttpenaivw.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.bjfxy.top/gtflnzjddh.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.pengpengdd.cyou/gthzdietxp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.cqqwz.cn/gtsopikpda.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.hfpthk.cn/gtbqwkqbty.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.zhengqikj.top/gtbknnykhj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.pycfn.com/gttnihkdps.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.zhaomingkeji.xyz/gtwwxvqwet.html

[P03] 生成短随机字符串
来源：http://hz.jyoumei.cn/gtuticdlrp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.ehwqpu.com/gtvppuynmf.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.shzxlz.cn/gtxysgwxyr.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hnqzz.top/gtripdiwce.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ivvv.top/gtfailnuxs.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.chenlongwang.top/gtufxaojoj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.dianchejie.cn/gtllowgxpb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.chenlongwang.top/gtsqkbotmg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jlsjyb.cn/gtpshwccne.html

[P04] 求长度
来源：http://hz.gogol.net.cn/gtplvuifal.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.316326.xyz/gtbzclodsx.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.daxiang520.top/gtufxkwpqn.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.snrcjt.cn/gtzcnfankr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.snrcjt.cn/gtvltreimp.html

Java: list.size();  map.size();  s.length()
来源：http://hz.hammf.cn/gtfkveybqx.html

Go:   len(arr);  len(m)
来源：http://hz.sweek.top/gtgxfidfzu.html

Ruby: x.length;  x.size
来源：http://hz.tianlin.xyz/gthtowqcjp.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.52xcode.cn/gtobsksccq.html

[P05] 判断两个对象内容是否相等
来源：http://hz.xingfuxueyuan.xyz/gtcukurnra.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.yj20258.top/gtpeqbkoge.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.yj20258888.top/gtnaaabsnp.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.yj202588.top/gtopjiugdj.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.tanke756.top/gtgilchbts.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.ybcxt.top/gttfoixodv.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.xuanzx.com/gtqfbbnvdw.html

Ruby: a == b
来源：http://hz.smart0.xyz/gtlpptiulo.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.xuetiantiany.cn/gtmrbusfuy.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.xziqi.cn/gtjshobqal.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.aibaodan.cn/gtqyzubmwf.html

PHP:  if (empty($x)) {}
来源：http://hz.zhaomingkeji.xyz/gtmidhpnvt.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.birdmap.top/gthjnrlgkw.html

TS:   if (x == null) {}
来源：http://hz.smart0.xyz/gtqgtnqcpu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.birdmap.top/gtzmxxmvsa.html

Go:   if x == nil {}
来源：http://hz.yuxming.cn/gttuhnhmta.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.yueranfly.top/gtqmclzaod.html

C#:   if (x is null) {}
来源：http://hz.cashguo.top/gtnognzwdk.html

[P07] 防抖与节流
来源：http://hz.zhoulong.xyz/gtjfcvnyls.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.pengpengdd.cyou/gtbaxpilao.html

PHP:  // 手写时间戳比较
来源：http://hz.xziqi.cn/gtsghaqqvw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.wangshuangyany.cn/gtnxjixdme.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ehwqpu.com/gtbepnqhwm.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.smart0.xyz/gtqevkzdfo.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.guowangkeji.top/gtiylralpk.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.fzhhl.top/gtemcrbxsr.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.gotoacloud.top/gtndlizcfd.html

[P08] 处理浮点精度问题
来源：http://hz.sxryk.cn/gtsbuxtuad.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jlsjyb.cn/gtqnvjhqol.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.jinqigufen.top/gtlqrqexra.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.tianlin.xyz/gthshxkxkg.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.zdqjudy.top/gthpdyplhr.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.chenlongwang.top/gttmrsmluc.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.fzhhl.top/gtvxnvomdg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.shanyushiyangtech.top/gtuazatdig.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.chenjidiqi.icu/gtlkangwds.html

================================================================================
来源：http://hz.quarkkingdee.top/gthosafhpj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.zdqjudy.top/gtyqrxzsso.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtcnlnwbpm.html

[Q01] 创建表
来源：http://hz.jqgufenzy.top/gtiloqbqjy.html

CREATE TABLE users (
来源：http://hz.chenlongwang.top/gtwcakbwuk.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xylfe.cn/gtmqwotkxw.html

name VARCHAR(50) NOT NULL,
来源：http://hz.xylfe.cn/gtgwphqvfd.html

email VARCHAR(100) UNIQUE,
来源：http://hz.xingfuxueyuan.xyz/gtfjpzyxxv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.daxiang520.top/gtcsuvmzye.html

);
来源：http://hz.jinqigufen.top/gtqxrktnac.html

[Q02] 创建带外键的表
来源：http://hz.yj202588.top/gtzhzhymls.html

CREATE TABLE orders (
来源：http://hz.nwbrower.top/gtcrsbuxwu.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.sysykeji.top/gtishkabyc.html

user_id INT NOT NULL,
来源：http://hz.zhaomingkeji.xyz/gtrtiysyzr.html

amount DECIMAL(10, 2),
来源：http://hz.aibaodan.cn/gtadcezwvu.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.jyoumei.cn/gttespovel.html

);
来源：http://hz.chenjidiqi.icu/gtyupwsxkd.html

[Q03] 增加列
来源：http://hz.xylfe.cn/gtclbgtcog.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.gaohongyu789.top/gtskvockop.html

[Q04] 修改列类型
来源：http://hz.ydjk.org.cn/gteuzjtqei.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.52xcode.cn/gtyfthxtgi.html

[Q05] 重命名列
来源：http://hz.sweek.top/gtuteziyft.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.fzhhl.top/gtkqitqacy.html

[Q06] 删除列
来源：http://hz.zhiwuduotai.top/gttdcadntl.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.yangfankeji.com/gtryadfche.html

[Q07] 删除表
来源：http://hz.jqgufenzy.top/gtnchumjpd.html

DROP TABLE IF EXISTS orders;
来源：http://hz.jianghu66.top/gtordvfvbr.html

[Q08] 创建普通索引
来源：http://hz.yangfankeji.com/gtdchasumd.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.yanxiufei.cn/gtsfqyjavu.html

[Q09] 创建唯一索引
来源：http://hz.gaohongyu789.top/gtbzwwjkhv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.pycfn.com/gtrpobsawd.html

[Q10] 插入单行
来源：http://hz.hnqzz.top/gtftxapmsx.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jiagoushi.top/gtubcvyrry.html

[Q11] 一次插入多行
来源：http://hz.yj202588.top/gtohcpxola.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.cdnleiting.top/gtesskedlx.html

[Q12] 插入后取自增 ID
来源：http://hz.shanyushiyangkeji.top/gtuctxrnho.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.bjfxy.top/gtoggvdsen.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.ybcxt.top/gtlxassqel.html

[Q13] 忽略重复插入
来源：http://hz.ybcxt.top/gtyhnewhqh.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.dianchejie.cn/gtbeygpnlf.html

[Q14] 存在则更新（upsert）
来源：http://hz.bjfxy.top/gtpxqfjrdx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.pengpengdd.cyou/gtrkboslbe.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.chenzaomai.com/gtihlynuwa.html

[Q15] 查询全部
来源：http://hz.sufxvd.cn/gtwopmeqjd.html

SELECT * FROM users;
来源：http://hz.zhoulong.xyz/gtyyprkjjz.html

[Q16] 查询指定列
来源：http://hz.meibo888.top/gtxwjsyqqs.html

SELECT id, name FROM users;
来源：http://hz.jyoumei.cn/gtxixashww.html

[Q17] 条件查询
来源：http://hz.feifeiyinyue.top/gtbhuylgpc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.ppjwa.cn/gtbaijakgl.html

[Q18] 模糊匹配
来源：http://hz.cdnleiting.top/gtsoquvvvm.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.cdnleiting.top/gtbcdaiesu.html

[Q19] 范围查询
来源：http://hz.xuanzx.com/gtfxgicvdy.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.iojbl.cn/gtiytucjlt.html

[Q20] IN 列表
来源：http://hz.jqgufenzy.top/gtqhangzqp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.jinyuanbaomall.cn/gtqbobgokj.html

[Q21] 空值判断
来源：http://hz.ywan-chungtsiang.top/gtxnrtsbzv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.hysaishi.cn/gtvnanbeuw.html

[Q22] 排序
来源：http://hz.9152youxi.cn/gtjlyjyazm.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.wangshuangyany.cn/gtoqucummc.html

[Q23] 分页
来源：http://hz.iojbl.cn/gtaxfgmvik.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.xinyue.icu/gtgjxmfwyn.html

[Q24] 去重
来源：http://hz.hfpthk.cn/gtwjaqsnkl.html

SELECT DISTINCT city FROM users;
来源：http://hz.sxryk.cn/gtkfwdttyj.html

[Q25] 只取前 N 条
来源：http://hz.cdnleiting.top/gtqyyfaiwe.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.cdnleiting.top/gtesaqurqx.html

[Q26] 计数
来源：http://hz.yuxming.cn/gtnpgzvzeo.html

SELECT COUNT(*) FROM users;
来源：http://hz.tanke756.top/gtcjqrswcv.html

[Q27] 条件计数
来源：http://hz.gaohongyu789.top/gtutankfyw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.jinyuanbaomall.cn/gtdjbwmxdx.html

[Q28] 求和与平均
来源：http://hz.gaohongyu789.top/gtcfuyglak.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.cashguo.top/gtalfpvuot.html

[Q29] 最大最小值
来源：http://hz.gogol.net.cn/gtgmobvqua.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.shanyushiyangkeji.top/gttaiaxfhh.html

[Q30] 分组统计
来源：http://hz.jinyuanbaomall.cn/gthgyypeoi.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.xylfe.cn/gtqhhgbkgo.html

[Q31] 分组后过滤
来源：http://hz.shuidangran.top/gtazvmpuzm.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.shangyingyoupin.top/gtdcklnntl.html

[Q32] 分组拼接字符串
来源：http://hz.feifeiyinyue.top/gttamysfby.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.ybcxt.top/gtzchvgizw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.ydjk.org.cn/gtruujmeat.html

[Q33] 多列分组
来源：http://hz.fengsongda.top/gtirmargxv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.ydzc1.top/gtehzzpzza.html

[Q34] 每组取第一条
来源：http://hz.sweek.top/gtcyhpddid.html

SELECT * FROM (
来源：http://hz.shangyingyoupin.top/gtzmoqechj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.shanyushiyangtech.top/gtixmodwkg.html

) t WHERE rn = 1;
来源：http://hz.gaohongyu789.top/gtxzsteash.html

[Q35] 内连接
来源：http://hz.wangdashe.top/gtbctrarqz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.jinghuilouyu.cn/gthcieaalw.html

[Q36] 左连接
来源：http://hz.ivvv.top/gtshtyailh.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.daria6918.cn/gtkvsngjtv.html

[Q37] 右连接
来源：http://hz.hfpthk.cn/gtfoxzfqxg.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.fengsongda.top/gtfvzghgkz.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.jlsjyb.cn/gtfjtoefzx.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.yueranfly.top/gtijvgrgyy.html

[Q39] 自连接（查上下级）
来源：http://hz.jianghu66.top/gtfroofgld.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.hongshengwenyu.top/gtauzugrgb.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yuxming.cn/gtmqvldrtq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.pengpengdd.cyou/gtmfmpqpae.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.guannengcc.top/gtyjftzipq.html

[Q41] 多表连接
来源：http://hz.ivvv.top/gteekvsmmm.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.shangyingyoupin.top/gthzekmmdy.html

JOIN users u ON u.id = o.user_id
来源：http://hz.ybcxt.top/gtqffjjuoy.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.yuanzhike.top/gtupxhqjsm.html

[Q42] 连接条件附加过滤
来源：http://hz.daria6918.cn/gtwrpoqxcr.html

SELECT u.name, o.amount FROM users u
来源：http://hz.yuanzhike.top/gtaoucqvpl.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.havefunace.top/gtoaffzwib.html

[Q43] 标量子查询
来源：http://hz.dianchejie.cn/gtrzmphhzy.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yueranfly.top/gtzqfumcgh.html

[Q44] IN 子查询
来源：http://hz.xingfuxueyuan.xyz/gtgonbawup.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.dianchejie.cn/gtcoiqepzo.html

[Q45] EXISTS 判断存在
来源：http://hz.hnxiangtu.top/gtzolwusbl.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.52xcode.cn/gtiobpcfso.html


<!-- 参考信息 -->