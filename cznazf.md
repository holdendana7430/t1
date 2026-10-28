代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.mhx1999.top/gtdbobguuo.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.xziqi.cn/gtlacndfrk.html

TS:   // 手写 Map<string, number>
来源：http://hz.hysaishi.cn/gtphxvixbx.html

Java: // 手写 HashMap
来源：http://hz.jqgfzy.top/gtguvyblyx.html

Go:   // 手写 map[int]int
来源：http://hz.chenlongwang.top/gtvdnzmlkr.html

Ruby: // 手写 Hash
来源：http://hz.chenjidiqi.icu/gtrppjghjt.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jinyuanbaomall.cn/gtefondxeu.html

[N08] 生成全排列
来源：http://hz.havefunace.top/gtrreadgax.html

Py:   itertools.permutations(arr)
来源：http://hz.xingfuxueyuan.xyz/gtlqiawqvq.html

PHP:  // 手写递归交换
来源：http://hz.ehwqpu.com/gtlafwrlwd.html

JS:   // 手写回溯递归
来源：http://hz.zhengqikj.top/gtjuqjwxoe.html

TS:   // 手写回溯递归
来源：http://hz.daria6918.cn/gtsqhvlbqx.html

Java: // 手写回溯递归
来源：http://hz.dianchejie.cn/gtwldwlruq.html

Go:   // 手写回溯递归
来源：http://hz.nwbrower.top/gtkgzrbrxz.html

Ruby: arr.permutation.to_a
来源：http://hz.bjfxy.top/gtuzyfshdh.html

C#:   // 手写回溯递归
来源：http://hz.yonumen.top/gtfkrfynmm.html

[N09] 栈与队列
来源：http://hz.jqgfzy.top/gtwlafzbux.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.nanxinkj.top/gtypskgtgr.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.fzhhl.top/gtfgbzszpg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.aibaodan.cn/gtsikqnnwd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.shanyushiyangtech.top/gtrakxnejd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.316326.xyz/gtebdaegvf.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.birdmap.top/gtbgntsxia.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.52xcode.cn/gtgvkwsupq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.birdmap.top/gtjvmkvqvx.html

[N10] 链表节点定义
来源：http://hz.shanyushiyangkeji.top/gtzkubyrne.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yuanzhike.top/gttfhgaknk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.quarkkingdee.top/gtjpneaclc.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yj20258.top/gtsxbbngmx.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.ehwqpu.com/gtdbhfrxfk.html

Java: class Node { int v; Node next; }
来源：http://hz.xylfe.cn/gtpmfrjcth.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.tian-w.cn/gtrydclgtz.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.jinyuanbaomall.cn/gtujtzilbm.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.hfpthk.cn/gthcwqhvyp.html

[N11] 二叉树中序遍历
来源：http://hz.9152youxi.cn/gtwdisxuwz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.vqdsnc.cn/gtcunhtyvj.html

PHP:  // 手写递归函数
来源：http://hz.xuetiantiany.cn/gtnxydskym.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.birdmap.top/gtntjouiwf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hywenlv.cn/gtfbdujhsj.html

Java: // 手写递归
来源：http://hz.hongshengwenyu.top/gtttrewutv.html

Go:   // 手写递归
来源：http://hz.0kj1m.cn/gtrkevfivc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.gogol.net.cn/gtiwvtiosk.html

C#:   // 手写递归
来源：http://hz.ydjk.org.cn/gtestpnbxg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.zycfv.cn/gteldcgdqn.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.yuxming.cn/gtjnfxizex.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jyoumei.cn/gthhejlydy.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.sufxvd.cn/gtcqrxvaqs.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cheryme.top/gtifvnuhxq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.tianlin.xyz/gtmkiajivp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.xylfe.cn/gtqtrdnfer.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.dashuyun.cn/gtstbqmrgr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.meibo888.top/gtfaoidibv.html

================================================================================
来源：http://hz.jlsjyb.cn/gtmdggbwii.html

O. 并发与异步
来源：http://hz.zhoulong.xyz/gtzonbsqsg.html

================================================================================
来源：http://hz.svipenyu.cn/gtxcuxcpzx.html

[O01] 启动一个线程
来源：http://hz.9152youxi.cn/gtculnajwf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.haohaochexian.top/gthaitlsqw.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.gaohongyu789.top/gtannbvogo.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.zhoulong.xyz/gtaqrbrhed.html

TS:   // 同 JS
来源：http://hz.daria6918.cn/gtcgpukhxd.html

Java: new Thread(() -> f()).start()
来源：http://hz.xuanzx.com/gthbxwavmu.html

Go:   go f()
来源：http://hz.yangfankeji.com/gtxstlgfnk.html

Ruby: Thread.new { f }
来源：http://hz.xinyue.icu/gthdetanaf.html

C#:   Task.Run(() => F());
来源：http://hz.meibo888.top/gtdfkafrav.html

[O02] 使用线程池
来源：http://hz.jqgfzy.top/gteznlydyq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.tanke756.top/gtlpsgtbta.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.zdqjudy.top/gtqcbawkuf.html

JS:   // worker_threads 线程池
来源：http://hz.fengsongda.top/gtvhiqlgju.html

TS:   // worker_threads 线程池
来源：http://hz.xuanzx.com/gtgzphdqgw.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yj20258.top/gtvgnizsjb.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.jianghu66.top/gtwurulvfx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yonumen.top/gtwrdepvmq.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.svipenyu.cn/gttvyepdwj.html

[O03] 加锁保护共享数据
来源：http://hz.hongshengwenyu.top/gtrpedccdq.html

Py:   with lock: shared += 1
来源：http://hz.shanyushiyangkeji.top/gtyyloxsyv.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.ehwqpu.com/gtuvglzppg.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.nanxinkj.top/gtzijuwsda.html

TS:   // 同 JS
来源：http://hz.tianlin.xyz/gtyifwqiau.html

Java: synchronized (this) { shared++; }
来源：http://hz.tian-w.cn/gtvicocryq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.ppjwa.cn/gtslgnhhqw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.yanxiufei.cn/gtwfyquyas.html

C#:   lock (gate) { shared++; }
来源：http://hz.yj20258888.top/gtzekvnykp.html

[O04] 定义异步函数并等待
来源：http://hz.yuanzhike.top/gtugqdpugg.html

Py:   async def f():⏎    await g()
来源：http://hz.hammf.cn/gtitjzqwwr.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.sxryk.cn/gtdqcgxdwf.html

JS:   async function f() { await g(); }
来源：http://hz.xylfe.cn/gtgqcvoujy.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.gaohongyu789.top/gtftxxexms.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.ybcxt.top/gtdqtltljm.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.iojbl.cn/gtotljtwna.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yongpay.top/gtkzxvxlxf.html

C#:   async Task F() { await G(); }
来源：http://hz.quarkkingdee.top/gtrqspyjyz.html

[O05] 并发执行并等待全部完成
来源：http://hz.hfpthk.cn/gtidpexdlk.html

Py:   asyncio.gather(*tasks)
来源：http://hz.yongpay.top/gtgjkbbbsc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.dianchejie.cn/gtjwanmhqb.html

JS:   await Promise.all(tasks)
来源：http://hz.pycfn.com/gtixjpxagr.html

TS:   await Promise.all(tasks)
来源：http://hz.gotoacloud.top/gtvxlhieny.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.andypj.xyz/gticafhtbw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.sufxvd.cn/gtgknhdmzp.html

Ruby: threads.map(&:join)
来源：http://hz.hnxiangtu.top/gtfwtdjjpv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.jqgfzy.top/gtgadjhzuy.html

[O06] 使用进程池
来源：http://hz.yueranfly.top/gtmirbsudc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.ydzc1.top/gtcqdznfht.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.sufxvd.cn/gtyczdmnvh.html

JS:   // child_process / cluster 模块
来源：http://hz.fzhhl.top/gtzbfnhche.html

TS:   // child_process / cluster 模块
来源：http://hz.yonumen.top/gtgwbwscte.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.ivvv.top/gtsshygbfg.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.haohaochexian.top/gtqlglhcbj.html

Ruby: // fork 块
来源：http://hz.xziqi.cn/gtjakjstdv.html

C#:   Parallel.For
来源：http://hz.fzhhl.top/gtxaqvfmas.html

================================================================================
来源：http://hz.ivvv.top/gtqaelreen.html

P. 常用工具函数
来源：http://hz.pycfn.com/gtnzvyodxf.html

================================================================================
来源：http://hz.gotoacloud.top/gtxkujxeoy.html

[P01] 生成 UUID
来源：http://hz.xziqi.cn/gteetqngfy.html

Py:   str(uuid.uuid4())
来源：http://hz.jqgfzy.top/gtgrsbzkyh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.gogol.net.cn/gteqhentnq.html

JS:   crypto.randomUUID()
来源：http://hz.316326.xyz/gtrrktwzko.html

TS:   crypto.randomUUID()
来源：http://hz.yuanzhike.top/gtzjdagjyt.html

Java: UUID.randomUUID().toString()
来源：http://hz.feifeiyinyue.top/gtzdhacmip.html

Go:   // 用 github.com/google/uuid
来源：http://hz.nanxuanxn.top/gttatkzhfb.html

Ruby: SecureRandom.uuid
来源：http://hz.zhiwuduotai.top/gtmkibwtwv.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.yj202588.top/gthrdkbrcj.html

[P02] MD5 / SHA256 摘要
来源：http://hz.hysaishi.cn/gtedriyoea.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.chenjidiqi.icu/gtiegcjhnp.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.sysykeji.top/gtvuivnmma.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.ppjwa.cn/gtcabklbex.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.yangfankeji.com/gtzfulkqdm.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.jinqigfzy.top/gtunnrnqfs.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.316326.xyz/gtauktkdug.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.zhoulong.xyz/gtjpncznqj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.svipenyu.cn/gtczjtnvii.html

[P03] 生成短随机字符串
来源：http://hz.hnxiangtu.top/gtbiaplicv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jqgufenzy.top/gtebzzqgbl.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.wangdashe.top/gtgvfvhlej.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hnqzz.top/gtddajtndy.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.nanxinkj.top/gtquxsbcih.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.0kj1m.cn/gtxocqrqbt.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.wangshuangyany.cn/gtrwwhlaop.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jiagoushi.top/gtfschwbqs.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.fzhhl.top/gtuhzjthjn.html

[P04] 求长度
来源：http://hz.0kj1m.cn/gtbgjkwyrz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.andypj.xyz/gtadvtlgls.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.gzhubu.top/gtlubgyaav.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.tanke756.top/gtqgjghogk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zycfv.cn/gthmoxvznv.html

Java: list.size();  map.size();  s.length()
来源：http://hz.wangshuangyany.cn/gthmfhbbeo.html

Go:   len(arr);  len(m)
来源：http://hz.snrcjt.cn/gtetwpsovt.html

Ruby: x.length;  x.size
来源：http://hz.sufxvd.cn/gtedixoktg.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.ydjk.org.cn/gtlxcvlpls.html

[P05] 判断两个对象内容是否相等
来源：http://hz.zhengqikj.top/gtaulngtwi.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.hfpthk.cn/gtwzugonrv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.c1oappe.top/gtotegkkpa.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.sufxvd.cn/gtinurpocv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.xinyue.icu/gtmewibcyr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.0kj1m.cn/gtykrajrgu.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.bjfxy.top/gtzknefthe.html

Ruby: a == b
来源：http://hz.yueranfly.top/gtccixveuo.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.pycfn.com/gtlrrtujsp.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.52xcode.cn/gtefbckyzc.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.chenzaomai.com/gtpmomfyfk.html

PHP:  if (empty($x)) {}
来源：http://hz.ydjk.org.cn/gtjpjojdny.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.tian-w.cn/gtbdqyvcjm.html

TS:   if (x == null) {}
来源：http://hz.yj20258.top/gtglawzlbq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.hammf.cn/gtvbzamlwk.html

Go:   if x == nil {}
来源：http://hz.9152youxi.cn/gtjcgtwjcv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jianghu66.top/gtiiyrbnhl.html

C#:   if (x is null) {}
来源：http://hz.ydjk.org.cn/gthymbccwr.html

[P07] 防抖与节流
来源：http://hz.hysaishi.cn/gtveaiacxw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yj20258.top/gtvurajcsr.html

PHP:  // 手写时间戳比较
来源：http://hz.sufxvd.cn/gtnxjiehtt.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.snrcjt.cn/gtbiwhzrxn.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.sufxvd.cn/gtfmnanann.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.hammf.cn/gtwuepukvo.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.wangdashe.top/gtjuuuinaw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.shanyushiyangtech.top/gtbcolwvqj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.9152youxi.cn/gtlwpegirc.html

[P08] 处理浮点精度问题
来源：http://hz.ywan-chungtsiang.top/gtqxddqgdu.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.yuxming.cn/gtrpczpvjz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.zhixingplan.top/gtuumtdjyt.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.tianlin.xyz/gtixzufqhn.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.pengpengdd.cyou/gtopomflaf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.quarkkingdee.top/gtstssthmp.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.jinghuilouyu.cn/gtsvgtomhn.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.yanxiufei.cn/gtwddfpfyv.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.jinyuanbaomall.cn/gthywllqip.html

================================================================================
来源：http://hz.gogol.net.cn/gtlldiotjz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.jinqigfzy.top/gtpvgspvim.html

================================================================================
来源：http://hz.zhengqikj.top/gtgvfqfyyj.html

[Q01] 创建表
来源：http://hz.sxryk.cn/gtfnlcwhqj.html

CREATE TABLE users (
来源：http://hz.bjfxy.top/gtetjyczrg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ehwqpu.com/gtijaqvdep.html

name VARCHAR(50) NOT NULL,
来源：http://hz.shzxlz.cn/gtobryvmiu.html

email VARCHAR(100) UNIQUE,
来源：http://hz.yj20258888.top/gtchsswnot.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.pengpengdd.cyou/gtqtcwtjyb.html

);
来源：http://hz.gaohongyu789.top/gttdrfadpg.html

[Q02] 创建带外键的表
来源：http://hz.tian-w.cn/gtvfvmhtbl.html

CREATE TABLE orders (
来源：http://hz.ydjk.org.cn/gtbyjxgqly.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hywenlv.cn/gtcjgyaypp.html

user_id INT NOT NULL,
来源：http://hz.daxiang520.top/gtwarqewkr.html

amount DECIMAL(10, 2),
来源：http://hz.birdmap.top/gtfmngnwps.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.cucudq.cn/gtcbejvgsp.html

);
来源：http://hz.daxiang520.top/gtnfhoywsy.html

[Q03] 增加列
来源：http://hz.9152youxi.cn/gtgegmyxws.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.hammf.cn/gtyfgqctqb.html

[Q04] 修改列类型
来源：http://hz.dianchejie.cn/gtemogyhwy.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.gotoacloud.top/gtaomqecyg.html

[Q05] 重命名列
来源：http://hz.316326.xyz/gtwmfomjrj.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.jinqigfzy.top/gtijaikjtk.html

[Q06] 删除列
来源：http://hz.havefunace.top/gtzcpytopp.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.wangshuangyany.cn/gttgqmpzhn.html

[Q07] 删除表
来源：http://hz.ybcxt.top/gthkdxnhii.html

DROP TABLE IF EXISTS orders;
来源：http://hz.sysykeji.top/gtzwkmhejm.html

[Q08] 创建普通索引
来源：http://hz.redwolf501.top/gtsmpgvyyz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.zhixingplan.top/gtwujyfvvp.html

[Q09] 创建唯一索引
来源：http://hz.zhijiandao.cn/gtqgdolptd.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.dashuyun.cn/gtbwniobxd.html

[Q10] 插入单行
来源：http://hz.yj202588.top/gtarxpcvxe.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.birdmap.top/gttrirsmlt.html

[Q11] 一次插入多行
来源：http://hz.jiagoushi.top/gtqgbrjinp.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.hongshengwenyu.top/gtypmqbdev.html

[Q12] 插入后取自增 ID
来源：http://hz.hnxiangtu.top/gtoiiutgwx.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.c1oappe.top/gtwfsdqdts.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.havefunace.top/gtirjzwlai.html

[Q13] 忽略重复插入
来源：http://hz.hnqzz.top/gtpykrrlkz.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.xylfe.cn/gtwxeiadvl.html

[Q14] 存在则更新（upsert）
来源：http://hz.tanke756.top/gtuvjzxsrz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.havefunace.top/gtmamlapwa.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.gogol.net.cn/gtuaywbcdx.html

[Q15] 查询全部
来源：http://hz.xingfuxueyuan.xyz/gtqdvpssvo.html

SELECT * FROM users;
来源：http://hz.zhoulong.xyz/gtpjaxhomv.html

[Q16] 查询指定列
来源：http://hz.xuanzx.com/gtleachkum.html

SELECT id, name FROM users;
来源：http://hz.daria6918.cn/gtelignslg.html

[Q17] 条件查询
来源：http://hz.sysykeji.top/gtfaqvmvun.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.daria6918.cn/gttoeusqde.html

[Q18] 模糊匹配
来源：http://hz.haohaochexian.top/gtlfnzezdu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.xingfuxueyuan.xyz/gtmhzjdctc.html

[Q19] 范围查询
来源：http://hz.ydjk.org.cn/gtviaokbhd.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.zhongyouzk.top/gtlrjykkee.html

[Q20] IN 列表
来源：http://hz.quarkkingdee.top/gtlexcrafi.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.sweek.top/gtasufjsmz.html

[Q21] 空值判断
来源：http://hz.hywenlv.cn/gtgosvqwny.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.quarkkingdee.top/gtirgsqhew.html

[Q22] 排序
来源：http://hz.yuanzhike.top/gthmzditxz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.haohaochexian.top/gtainnpcui.html

[Q23] 分页
来源：http://hz.vqdsnc.cn/gtxbipxivc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.daxiang520.top/gtakwspwmn.html

[Q24] 去重
来源：http://hz.cqqwz.cn/gtjhriypka.html

SELECT DISTINCT city FROM users;
来源：http://hz.0kj1m.cn/gtjwncktfd.html

[Q25] 只取前 N 条
来源：http://hz.nanxinkj.top/gtfolwbbhu.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.shzxlz.cn/gtevffaebr.html

[Q26] 计数
来源：http://hz.316326.xyz/gtopygiwks.html

SELECT COUNT(*) FROM users;
来源：http://hz.andypj.xyz/gtegfxaghq.html

[Q27] 条件计数
来源：http://hz.xziqi.cn/gtvtpljemd.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.sxryk.cn/gtqrlqegug.html

[Q28] 求和与平均
来源：http://hz.havefunace.top/gtktzwvegh.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.jianghu66.top/gtfmkvjyqe.html

[Q29] 最大最小值
来源：http://hz.jiagoushi.top/gtnghtmylc.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.pengpengdd.cyou/gtbkxoqcai.html

[Q30] 分组统计
来源：http://hz.hfpthk.cn/gtjbhnhbot.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.fengsongda.top/gtlcwvvxgx.html

[Q31] 分组后过滤
来源：http://hz.xuetiantiany.cn/gthrrxlqnf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.sufxvd.cn/gtkzmzszsw.html

[Q32] 分组拼接字符串
来源：http://hz.shzxlz.cn/gtekaiepob.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.iojbl.cn/gtmxeowdxf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yonumen.top/gtcbnbrcit.html

[Q33] 多列分组
来源：http://hz.hywenlv.cn/gtvxwpsfow.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.316326.xyz/gtzurtbark.html

[Q34] 每组取第一条
来源：http://hz.yueranfly.top/gtnxjewkpu.html

SELECT * FROM (
来源：http://hz.hysaishi.cn/gtlagxlmvm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jiagoushi.top/gtwpcwrlzz.html

) t WHERE rn = 1;
来源：http://hz.zycfv.cn/gtvorrflew.html

[Q35] 内连接
来源：http://hz.svipenyu.cn/gtfmrsawlc.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.yj20258.top/gtrcpppapa.html

[Q36] 左连接
来源：http://hz.tanke756.top/gtekbsoioz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.hnqzz.top/gtrjzjxcbs.html

[Q37] 右连接
来源：http://hz.sufxvd.cn/gtxjiaczqp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.yj202588.top/gtjiozduas.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.wangdashe.top/gtxgmgutpj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.redwolf501.top/gtxxocgkav.html

[Q39] 自连接（查上下级）
来源：http://hz.shangyingyoupin.top/gtxccgpika.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.yangfankeji.com/gthvtauoyg.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.jinghuilouyu.cn/gtcrhhotbf.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.zhixingplan.top/gthpeozxce.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.havefunace.top/gthmfmcwtd.html

[Q41] 多表连接
来源：http://hz.cdnleiting.top/gtiblegigf.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.9152youxi.cn/gtuaknppee.html

JOIN users u ON u.id = o.user_id
来源：http://hz.gzhubu.top/gthgkavmlx.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.dashuyun.cn/gtwpjhrccw.html

[Q42] 连接条件附加过滤
来源：http://hz.snrcjt.cn/gtyuqxlgua.html

SELECT u.name, o.amount FROM users u
来源：http://hz.xingfuxueyuan.xyz/gtpyjudosi.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.zhaomingkeji.xyz/gtksnfbudh.html

[Q43] 标量子查询
来源：http://hz.tanke756.top/gtirfvrwgg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yanxiufei.cn/gtebhdrmms.html

[Q44] IN 子查询
来源：http://hz.sysykeji.top/gthrjebbaj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.yueranfly.top/gtajljdmhk.html

[Q45] EXISTS 判断存在
来源：http://hz.yj20258888.top/gtppigtdom.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jlsjyb.cn/gtgjopquhw.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.svipenyu.cn/gtnnzylsgm.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hnqzz.top/gtrwhlvtwv.html

[Q47] 与平均值比较
来源：http://hz.zdqjudy.top/gtpnivzbdw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.cdnleiting.top/gtwcedtzxb.html


<!-- 参考信息 -->