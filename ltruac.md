代发 wailian999

Go:   // 手写 map[int]int
来源：http://hz.cdnleiting.top/gtbxsxquni.html

Ruby: // 手写 Hash
来源：http://hz.yonumen.top/gtonzeuzrg.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jyoumei.cn/gttlhymzsp.html

[N08] 生成全排列
来源：http://hz.andypj.xyz/gtlpuidxcd.html

Py:   itertools.permutations(arr)
来源：http://hz.fzhhl.top/gtqogfuasu.html

PHP:  // 手写递归交换
来源：http://hz.yuxming.cn/gtgjngcufy.html

JS:   // 手写回溯递归
来源：http://hz.jqgfzy.top/gtxwzserdu.html

TS:   // 手写回溯递归
来源：http://hz.hnqzz.top/gtwagflmce.html

Java: // 手写回溯递归
来源：http://hz.jiagoushi.top/gtlysogqwp.html

Go:   // 手写回溯递归
来源：http://hz.yangfankeji.com/gtcbxytcjj.html

Ruby: arr.permutation.to_a
来源：http://hz.havefunace.top/gtcdvxkqwk.html

C#:   // 手写回溯递归
来源：http://hz.tianlin.xyz/gtrzlxzzkk.html

[N09] 栈与队列
来源：http://hz.cqqwz.cn/gtvdzahwfv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.haohaochexian.top/gtmfofjkhc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.yuanzhike.top/gtulwmvbhn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.xuetiantiany.cn/gtuimnftgi.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.xylfe.cn/gtlfocogtb.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.quarkkingdee.top/gtejmkwiuv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.wangdashe.top/gtbyjadywx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.jlsjyb.cn/gtcgzcopao.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.chenzaomai.com/gtbthahpqv.html

[N10] 链表节点定义
来源：http://hz.jinqigufen.top/gthcmgazoe.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.ybcxt.top/gtwjudlakr.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jinqigufen.top/gtdarhzliy.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.chenzaomai.com/gtwykavwng.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.sysykeji.top/gtnuxuxgkf.html

Java: class Node { int v; Node next; }
来源：http://hz.jqgufenzy.top/gtlwabcjpt.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.hnxiangtu.top/gtetrshxcr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.ydjk.org.cn/gtijndkfbe.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.jyoumei.cn/gtkoeujpta.html

[N11] 二叉树中序遍历
来源：http://hz.gotoacloud.top/gtxyobacdr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.cdnleiting.top/gtatbtiogg.html

PHP:  // 手写递归函数
来源：http://hz.yangfankeji.com/gtjgzsfmsi.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ywan-chungtsiang.top/gthbjkdult.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.aizwys.cn/gtqiexskhj.html

Java: // 手写递归
来源：http://hz.ybcxt.top/gtokezjkhx.html

Go:   // 手写递归
来源：http://hz.tanke756.top/gtqqeljpgn.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.shangyingyoupin.top/gthpnjygrq.html

C#:   // 手写递归
来源：http://hz.chenjidiqi.icu/gtzztfsxie.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.haohaochexian.top/gtizaclrvh.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.gzhubu.top/gtbiewmhjx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.andypj.xyz/gtnexaxzky.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.aibaodan.cn/gtepedtabz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.chenlongwang.top/gtqhkgcuwc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ppjwa.cn/gtysaxjxlz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.yanxiufei.cn/gtaskofljc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.chenjidiqi.icu/gtfhoylfyu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hysaishi.cn/gtwitdwlee.html

================================================================================
来源：http://hz.sufxvd.cn/gtamavyeps.html

O. 并发与异步
来源：http://hz.yanxiufei.cn/gtyoukgcus.html

================================================================================
来源：http://hz.jiagoushi.top/gtwwygcttu.html

[O01] 启动一个线程
来源：http://hz.9152youxi.cn/gtpkjkiazu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.jiagoushi.top/gtxjcccbfu.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.ydzc1.top/gtmxpixvul.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.feifeiyinyue.top/gtpqsjwdbc.html

TS:   // 同 JS
来源：http://hz.jyoumei.cn/gtejjhjrfs.html

Java: new Thread(() -> f()).start()
来源：http://hz.zhongyouzk.top/gtuhmzwcdq.html

Go:   go f()
来源：http://hz.yanxiufei.cn/gtccbxnzhj.html

Ruby: Thread.new { f }
来源：http://hz.jianghu66.top/gtekersxsh.html

C#:   Task.Run(() => F());
来源：http://hz.feifeiyinyue.top/gtfojggcpo.html

[O02] 使用线程池
来源：http://hz.zhaomingkeji.xyz/gtqxvbvmei.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.jinyuanbaomall.cn/gtyllvjiag.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.xingfuxueyuan.xyz/gtzcvcwbvm.html

JS:   // worker_threads 线程池
来源：http://hz.guannengcc.top/gtqwqiscrs.html

TS:   // worker_threads 线程池
来源：http://hz.hongshengwenyu.top/gtwzuptiey.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.birdmap.top/gtcyytkvrw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.jinghuilouyu.cn/gtsqkowbbh.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.jlsjyb.cn/gthpxfbmkd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.xingfuxueyuan.xyz/gtllzgyvys.html

[O03] 加锁保护共享数据
来源：http://hz.ppjwa.cn/gtdelhqyvc.html

Py:   with lock: shared += 1
来源：http://hz.xuanzx.com/gtzadfibtr.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.hnqzz.top/gtjnsietlo.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.jqgufenzy.top/gtxebmdfwh.html

TS:   // 同 JS
来源：http://hz.xuanzx.com/gtxqfqxuag.html

Java: synchronized (this) { shared++; }
来源：http://hz.ywan-chungtsiang.top/gtewvjmlpd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.ehwqpu.com/gttbfbysrp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.ybcxt.top/gtiypzsrjd.html

C#:   lock (gate) { shared++; }
来源：http://hz.yongpay.top/gtogtyuirv.html

[O04] 定义异步函数并等待
来源：http://hz.shanyushiyangkeji.top/gtsmpegwya.html

Py:   async def f():⏎    await g()
来源：http://hz.havefunace.top/gtfqgwibpu.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.zhaomingkeji.xyz/gtpkjuoyqe.html

JS:   async function f() { await g(); }
来源：http://hz.316326.xyz/gtnmsptxzq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.0kj1m.cn/gtairctgyf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.ehwqpu.com/gtujdpowya.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.cdnleiting.top/gtjlhsydss.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.kuanghao11.cn/gtrcedbmeg.html

C#:   async Task F() { await G(); }
来源：http://hz.ppjwa.cn/gtqwfystam.html

[O05] 并发执行并等待全部完成
来源：http://hz.kuanghao11.cn/gtmguqosgt.html

Py:   asyncio.gather(*tasks)
来源：http://hz.yonumen.top/gtkyvyvdap.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.ybcxt.top/gtbihqobaq.html

JS:   await Promise.all(tasks)
来源：http://hz.iojbl.cn/gtemmhzrge.html

TS:   await Promise.all(tasks)
来源：http://hz.jqgufenzy.top/gtyjytcies.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.nanxinkj.top/gtlpbtjesf.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.zhengqikj.top/gtdnbnmfja.html

Ruby: threads.map(&:join)
来源：http://hz.havefunace.top/gtilurksxd.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.jinghuilouyu.cn/gtcxydbbfj.html

[O06] 使用进程池
来源：http://hz.shuidangran.top/gtfksujrna.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.wangshuangyany.cn/gtjbydzlfd.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.fengsongda.top/gtwbnadlle.html

JS:   // child_process / cluster 模块
来源：http://hz.9152youxi.cn/gticgeccjt.html

TS:   // child_process / cluster 模块
来源：http://hz.yonumen.top/gtksibgaan.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.cucudq.cn/gtfdyflgqz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.nanxinkj.top/gtmrquoqav.html

Ruby: // fork 块
来源：http://hz.dashuyun.cn/gtxkhhnwxm.html

C#:   Parallel.For
来源：http://hz.ywan-chungtsiang.top/gtuupqbsdl.html

================================================================================
来源：http://hz.cqqwz.cn/gtmukrsiir.html

P. 常用工具函数
来源：http://hz.redwolf501.top/gtsihihybj.html

================================================================================
来源：http://hz.jlsjyb.cn/gtobvfqtce.html

[P01] 生成 UUID
来源：http://hz.jinyuanbaomall.cn/gttxlmyawe.html

Py:   str(uuid.uuid4())
来源：http://hz.sysykeji.top/gtsfelqhbx.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.mhx1999.top/gtfxsbfyap.html

JS:   crypto.randomUUID()
来源：http://hz.aibaodan.cn/gtbepfcvkf.html

TS:   crypto.randomUUID()
来源：http://hz.hnqzz.top/gtpvghltof.html

Java: UUID.randomUUID().toString()
来源：http://hz.guannengcc.top/gtevaldmjk.html

Go:   // 用 github.com/google/uuid
来源：http://hz.gotoacloud.top/gtowcvtkcm.html

Ruby: SecureRandom.uuid
来源：http://hz.ybcxt.top/gtsnumthnn.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.tanke756.top/gtcfvsbrce.html

[P02] MD5 / SHA256 摘要
来源：http://hz.cheryme.top/gtntbjjfuc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.9152youxi.cn/gthbuescou.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.yvedp.cn/gtjrmbtsrs.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.xinyue.icu/gtvlgrpvzb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.hfpthk.cn/gtxqqccycf.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.tianlin.xyz/gtpizcxmyd.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.birdmap.top/gttdfzvqlc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.yonumen.top/gtfixkjywg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.shzxlz.cn/gtqlkgxqqp.html

[P03] 生成短随机字符串
来源：http://hz.dashuyun.cn/gtifzxqhsl.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.9152youxi.cn/gtximbwpmh.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.gotoacloud.top/gtfdqktqvx.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hfpthk.cn/gtfdkveddn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xylfe.cn/gtooobfucp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.cucudq.cn/gttqlxzcin.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.tianlin.xyz/gtxlhbushl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.cucudq.cn/gtgcqvohds.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.kuanghao11.cn/gtghacvvuy.html

[P04] 求长度
来源：http://hz.ppjwa.cn/gtehejjaag.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.feifeiyinyue.top/gtwxoutwvu.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhaomingkeji.xyz/gtthuhyimh.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.chenlongwang.top/gtjkukqhko.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.cucudq.cn/gtldtuyzrn.html

Java: list.size();  map.size();  s.length()
来源：http://hz.bjfxy.top/gtoxeaugty.html

Go:   len(arr);  len(m)
来源：http://hz.yj20258.top/gtbkpburhn.html

Ruby: x.length;  x.size
来源：http://hz.hysaishi.cn/gtcismxbit.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.kuanghao11.cn/gtyuavxzjv.html

[P05] 判断两个对象内容是否相等
来源：http://hz.yueranfly.top/gtaxaarmak.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.chenlongwang.top/gtkehyprhv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.cheryme.top/gtowukbana.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.yangfankeji.com/gtzwyrouyk.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.andypj.xyz/gtlpmqlwyv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.xuanzx.com/gtaslpryfq.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yanxiufei.cn/gtlagiiwsx.html

Ruby: a == b
来源：http://hz.zycfv.cn/gthwixtnwt.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.0kj1m.cn/gthtaxdhxs.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.ydzc1.top/gtdixntzpv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.yuxming.cn/gtihaayela.html

PHP:  if (empty($x)) {}
来源：http://hz.aizwys.cn/gtmcusdfxs.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.cqqwz.cn/gtqxucxuxg.html

TS:   if (x == null) {}
来源：http://hz.svipenyu.cn/gtixrdquoo.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.hammf.cn/gtufugkxzr.html

Go:   if x == nil {}
来源：http://hz.hfpthk.cn/gtmylxpqzh.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.cdnleiting.top/gtxztduzfi.html

C#:   if (x is null) {}
来源：http://hz.hnqzz.top/gtqjbkuvvg.html

[P07] 防抖与节流
来源：http://hz.pycfn.com/gtsqdbhgsh.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.zycfv.cn/gtqhaxatus.html

PHP:  // 手写时间戳比较
来源：http://hz.quarkkingdee.top/gtsprssagf.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hysaishi.cn/gtsbutwgee.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hfpthk.cn/gttuxleprc.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.iojbl.cn/gtczlgffyy.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.xuetiantiany.cn/gtsemcgfrt.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yonumen.top/gtkatmewnp.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.mhx1999.top/gtnthgfcth.html

[P08] 处理浮点精度问题
来源：http://hz.ydzc1.top/gtxjmpmudh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.yuanzhike.top/gtdvqhpsgn.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.52xcode.cn/gtbqkskgfn.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.redwolf501.top/gtjdxgyxwz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.fzhhl.top/gtbevmdnhq.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.gzhubu.top/gthexlnrfz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.pengpengdd.cyou/gtjihflkdp.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.cashguo.top/gtpksjtfiu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.quarkkingdee.top/gtpoopgyir.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtivgqpktb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.quarkkingdee.top/gtpvudncgw.html

================================================================================
来源：http://hz.svipenyu.cn/gtsftfbvzz.html

[Q01] 创建表
来源：http://hz.tanke756.top/gtogvfuhov.html

CREATE TABLE users (
来源：http://hz.yanxiufei.cn/gtxbiqtqil.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhixingplan.top/gtcgvzuagz.html

name VARCHAR(50) NOT NULL,
来源：http://hz.yuxming.cn/gtzctahbed.html

email VARCHAR(100) UNIQUE,
来源：http://hz.chenlongwang.top/gthljnqkui.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.nanxinkj.top/gtyackzvzs.html

);
来源：http://hz.vqdsnc.cn/gtimjfjead.html

[Q02] 创建带外键的表
来源：http://hz.cheryme.top/gtglgrkzbq.html

CREATE TABLE orders (
来源：http://hz.zhengqikj.top/gtnnrkdjbl.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ppjwa.cn/gtdioocrwx.html

user_id INT NOT NULL,
来源：http://hz.ydzc1.top/gtzgtuquus.html

amount DECIMAL(10, 2),
来源：http://hz.ivvv.top/gtxubcwccy.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.jinqigfzy.top/gtssjppbou.html

);
来源：http://hz.hnxiangtu.top/gtvtcdflge.html

[Q03] 增加列
来源：http://hz.gotoacloud.top/gttrjualqp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.feifeiyinyue.top/gtvzqobxig.html

[Q04] 修改列类型
来源：http://hz.zhoulong.xyz/gtvblhtcad.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.snrcjt.cn/gtjbqbdifr.html

[Q05] 重命名列
来源：http://hz.xziqi.cn/gtnprcqngw.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.mhx1999.top/gtdwjiqjnt.html

[Q06] 删除列
来源：http://hz.birdmap.top/gtfdgjxfkb.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.guowangkeji.top/gtxcrrhcqn.html

[Q07] 删除表
来源：http://hz.xylfe.cn/gtnnylgthd.html

DROP TABLE IF EXISTS orders;
来源：http://hz.sxryk.cn/gtqnoxpuxa.html

[Q08] 创建普通索引
来源：http://hz.xuanzx.com/gtyhqqtevh.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.yvedp.cn/gtrdnylouv.html

[Q09] 创建唯一索引
来源：http://hz.yj20258.top/gtmnabayto.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.kuanghao11.cn/gtmfaafibs.html

[Q10] 插入单行
来源：http://hz.quarkkingdee.top/gtgjxtyrwm.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jianghu66.top/gtrilpthft.html

[Q11] 一次插入多行
来源：http://hz.hnxiangtu.top/gtljrloaai.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.chenjidiqi.icu/gtjysgtldr.html

[Q12] 插入后取自增 ID
来源：http://hz.shanyushiyangkeji.top/gtdfmvibpv.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.zdqjudy.top/gtsujmwxdw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.9152youxi.cn/gtddcmgejq.html

[Q13] 忽略重复插入
来源：http://hz.shanyushiyangtech.top/gtwmhkvasc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.gotoacloud.top/gtergauwsy.html

[Q14] 存在则更新（upsert）
来源：http://hz.havefunace.top/gtdcwempam.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.jlsjyb.cn/gtrmpokhin.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.xingfuxueyuan.xyz/gtxfbvfhfm.html

[Q15] 查询全部
来源：http://hz.zhiwuduotai.top/gturkwwyfz.html

SELECT * FROM users;
来源：http://hz.nanxinkj.top/gtjdvlaejm.html

[Q16] 查询指定列
来源：http://hz.iojbl.cn/gteqpfwgwf.html

SELECT id, name FROM users;
来源：http://hz.sxryk.cn/gtottwraxh.html

[Q17] 条件查询
来源：http://hz.guowangkeji.top/gtjyxzemzu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.xziqi.cn/gtilaoofqz.html

[Q18] 模糊匹配
来源：http://hz.hongshengwenyu.top/gtudnommnc.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.meibo888.top/gtwzxsoejl.html

[Q19] 范围查询
来源：http://hz.zhixingplan.top/gtuxzfqojp.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.gaohongyu789.top/gtcprbjymx.html

[Q20] IN 列表
来源：http://hz.smart0.xyz/gtlnamsezt.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.guowangkeji.top/gtfuzvurzz.html

[Q21] 空值判断
来源：http://hz.vqdsnc.cn/gtkieyibdm.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.yj202588.top/gtbskqganf.html

[Q22] 排序
来源：http://hz.shanyushiyangkeji.top/gtriwwvmwe.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.dashuyun.cn/gttozkrkip.html

[Q23] 分页
来源：http://hz.zhengqikj.top/gtyvcshagu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.smart0.xyz/gtippjzhwz.html

[Q24] 去重
来源：http://hz.xuetiantiany.cn/gtgwezuwyl.html

SELECT DISTINCT city FROM users;
来源：http://hz.birdmap.top/gtohargxlo.html

[Q25] 只取前 N 条
来源：http://hz.hnqzz.top/gtegsomzyj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.zhixingplan.top/gtifwgiqcc.html

[Q26] 计数
来源：http://hz.ehwqpu.com/gtwjeltxnb.html

SELECT COUNT(*) FROM users;
来源：http://hz.iojbl.cn/gtltzrknur.html

[Q27] 条件计数
来源：http://hz.zycfv.cn/gtczcwkhuc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.xinyue.icu/gttrjxgxbd.html

[Q28] 求和与平均
来源：http://hz.hammf.cn/gtbzcnnufa.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.iojbl.cn/gtogqjmqme.html

[Q29] 最大最小值
来源：http://hz.xziqi.cn/gtpfgjejbn.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.shangyingyoupin.top/gtqpmtkvqx.html

[Q30] 分组统计
来源：http://hz.zhaomingkeji.xyz/gtmuewfdvw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.jiagoushi.top/gtaefjhrnq.html

[Q31] 分组后过滤
来源：http://hz.shanyushiyangkeji.top/gtgxzbppju.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.jqgufenzy.top/gtdtjdctkb.html

[Q32] 分组拼接字符串
来源：http://hz.yuanzhike.top/gtgbpodgkq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.zhengqikj.top/gtapjqvfxq.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.hnqzz.top/gtfsumutqv.html

[Q33] 多列分组
来源：http://hz.shuidangran.top/gtzqkivvaz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.ivvv.top/gtfcxkuxum.html

[Q34] 每组取第一条
来源：http://hz.fzhhl.top/gtriypjyvu.html

SELECT * FROM (
来源：http://hz.wangdashe.top/gtlicqjmaf.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.daria6918.cn/gtyenfixrc.html

) t WHERE rn = 1;
来源：http://hz.zhijiandao.cn/gtripsjvcq.html

[Q35] 内连接
来源：http://hz.haohaochexian.top/gtghedytdk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.yongpay.top/gtpzjpsqex.html

[Q36] 左连接
来源：http://hz.yj20258888.top/gtpnajdrzr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.snrcjt.cn/gtpkzbtoby.html

[Q37] 右连接
来源：http://hz.hfpthk.cn/gthmgemgmt.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.cdnleiting.top/gtgujkvouy.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.wangshuangyany.cn/gtvwottyek.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.yvedp.cn/gtzeimiidy.html

[Q39] 自连接（查上下级）
来源：http://hz.shangyingyoupin.top/gtjnadhnwi.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.zhiwuduotai.top/gtzfrawhsc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yj20258888.top/gtduhhchop.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.wangshuangyany.cn/gtygypphkn.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.nwbrower.top/gtryvoilhq.html

[Q41] 多表连接
来源：http://hz.jiagoushi.top/gtbjutoiax.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.hnqzz.top/gtuvvdmdqg.html

JOIN users u ON u.id = o.user_id
来源：http://hz.zdqjudy.top/gtcmkpcktm.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.yongpay.top/gtsknxrkmy.html

[Q42] 连接条件附加过滤
来源：http://hz.chenzaomai.com/gtytbfaast.html

SELECT u.name, o.amount FROM users u
来源：http://hz.zhoulong.xyz/gtvdgjwils.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.redwolf501.top/gtblqcdwqv.html

[Q43] 标量子查询
来源：http://hz.sweek.top/gtyceluqwi.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.gotoacloud.top/gtnbpgqeue.html

[Q44] IN 子查询
来源：http://hz.yueranfly.top/gtrrpgraee.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.ydzc1.top/gtpkprastw.html

[Q45] EXISTS 判断存在
来源：http://hz.pycfn.com/gtpooevzpr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.mhx1999.top/gtrkeepepg.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.jinqigufen.top/gtpahedpgh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.dashuyun.cn/gtfjkfyvis.html

[Q47] 与平均值比较
来源：http://hz.sweek.top/gtcwenwzgd.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.dashuyun.cn/gtonhwbsfo.html

[Q48] CTE 公用表表达式
来源：http://hz.haohaochexian.top/gtmgmckrga.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.tian-w.cn/gtpsenvqqx.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.aibaodan.cn/gtwziecbrt.html

[Q49] 更新单行
来源：http://hz.chenjidiqi.icu/gtfoqtlgal.html


<!-- 参考信息 -->