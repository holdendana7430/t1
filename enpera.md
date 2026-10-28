代发 wailian999

Java: // 手写回溯递归
来源：http://hz.ydzc1.top/gtbsbhnjca.html

Go:   // 手写回溯递归
来源：http://hz.yj202588.top/gtmxvrsfci.html

Ruby: arr.permutation.to_a
来源：http://hz.guowangkeji.top/gtitjjkgim.html

C#:   // 手写回溯递归
来源：http://hz.tianlin.xyz/gtahbvbgpx.html

[N09] 栈与队列
来源：http://hz.fengsongda.top/gtlkeqzhpy.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.daria6918.cn/gtqftjynrn.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.pycfn.com/gtqnmleteb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.cashguo.top/gtpfusmvmf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jinyuanbaomall.cn/gtzowyhuft.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yongpay.top/gtzpqbudcw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.hnxiangtu.top/gtcwyletjq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.kuanghao11.cn/gtdvrayovx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.daxiang520.top/gtqqalearb.html

[N10] 链表节点定义
来源：http://hz.sysykeji.top/gtmtmpclvb.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.zhongyouzk.top/gteveqeqwy.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.shanyushiyangtech.top/gtpnpytibz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.tian-w.cn/gthyctflgt.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.ydzc1.top/gtpkqsdxlm.html

Java: class Node { int v; Node next; }
来源：http://hz.316326.xyz/gtdxeuenqs.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.chenjidiqi.icu/gtydancubd.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.smart0.xyz/gtckapihcq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.cucudq.cn/gtmplakxhi.html

[N11] 二叉树中序遍历
来源：http://hz.jinqigufen.top/gtvibljcvp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.xylfe.cn/gtmecrcvlr.html

PHP:  // 手写递归函数
来源：http://hz.nwbrower.top/gtfogqpprv.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.shanyushiyangkeji.top/gtotmfnpbt.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.nanxinkj.top/gtkspijhtd.html

Java: // 手写递归
来源：http://hz.aibaodan.cn/gtjuldkrpn.html

Go:   // 手写递归
来源：http://hz.xinyue.icu/gtxznwudls.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.daxiang520.top/gtzuljsyue.html

C#:   // 手写递归
来源：http://hz.zhongyouzk.top/gtkbkixskz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.dianchejie.cn/gtqnxyewun.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.nanxinkj.top/gtcjfzwdzh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.9152youxi.cn/gtparmrpsf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yueranfly.top/gtgxzpjmgs.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.9152youxi.cn/gtsdvcouej.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.mhx1999.top/gtzctiytao.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.xuanzx.com/gtdzpbhssw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.feifeiyinyue.top/gtumlvgnje.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jiagoushi.top/gtyafhwszy.html

================================================================================
来源：http://hz.zdqjudy.top/gtiimrawtq.html

O. 并发与异步
来源：http://hz.yuxming.cn/gtvostwvde.html

================================================================================
来源：http://hz.9152youxi.cn/gtbzauason.html

[O01] 启动一个线程
来源：http://hz.shangyingyoupin.top/gteobfhgzm.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.yonumen.top/gtgvvknpbw.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.sxryk.cn/gtcemuiuzr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.cqqwz.cn/gtugpovqtj.html

TS:   // 同 JS
来源：http://hz.c1oappe.top/gtusmbvnos.html

Java: new Thread(() -> f()).start()
来源：http://hz.jinghuilouyu.cn/gtvkcueqbf.html

Go:   go f()
来源：http://hz.gotoacloud.top/gtlgppvkna.html

Ruby: Thread.new { f }
来源：http://hz.jinqigfzy.top/gtihkdjbrg.html

C#:   Task.Run(() => F());
来源：http://hz.tianlin.xyz/gtvprdnydu.html

[O02] 使用线程池
来源：http://hz.sysykeji.top/gtnhlinoif.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.wangshuangyany.cn/gtihjowekc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.guowangkeji.top/gtravmcmci.html

JS:   // worker_threads 线程池
来源：http://hz.jinqigufen.top/gtwvjplnrg.html

TS:   // worker_threads 线程池
来源：http://hz.chenlongwang.top/gttuskzvzd.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.hammf.cn/gtqaryxmxb.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.gogol.net.cn/gtoxbcuotj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yueranfly.top/gtpeynksmy.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.jinqigfzy.top/gttayyiivg.html

[O03] 加锁保护共享数据
来源：http://hz.52xcode.cn/gtptbxdpqs.html

Py:   with lock: shared += 1
来源：http://hz.yj20258.top/gtsxxnhzqy.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.cashguo.top/gtsogjxubb.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.xylfe.cn/gtmuqxiaeb.html

TS:   // 同 JS
来源：http://hz.gotoacloud.top/gtzeakjjpd.html

Java: synchronized (this) { shared++; }
来源：http://hz.gotoacloud.top/gttfgpgydc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.jinghuilouyu.cn/gtupwgxcgf.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.9152youxi.cn/gtlvnextoi.html

C#:   lock (gate) { shared++; }
来源：http://hz.zhijiandao.cn/gthyrpaqeu.html

[O04] 定义异步函数并等待
来源：http://hz.ehwqpu.com/gtluxksmbg.html

Py:   async def f():⏎    await g()
来源：http://hz.hammf.cn/gtgvsfdogb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.mhx1999.top/gtjhnmxczg.html

JS:   async function f() { await g(); }
来源：http://hz.kuanghao11.cn/gtolyrobmw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.cqqwz.cn/gtqdedqhir.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.9152youxi.cn/gtphninuzp.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.jinghuilouyu.cn/gtfjqzchts.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.pycfn.com/gtyqnmqjyv.html

C#:   async Task F() { await G(); }
来源：http://hz.hnqzz.top/gtagksqvcz.html

[O05] 并发执行并等待全部完成
来源：http://hz.aizwys.cn/gtxlhpwjly.html

Py:   asyncio.gather(*tasks)
来源：http://hz.zhaomingkeji.xyz/gtlacpuijb.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.yj20258.top/gtbdxyesuq.html

JS:   await Promise.all(tasks)
来源：http://hz.xziqi.cn/gttjwmiqzj.html

TS:   await Promise.all(tasks)
来源：http://hz.zycfv.cn/gtntjjviej.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.dianchejie.cn/gtfsmqljer.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.havefunace.top/gtcgatitit.html

Ruby: threads.map(&:join)
来源：http://hz.sxryk.cn/gtayqblmvd.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.haohaochexian.top/gtpzyoeyqm.html

[O06] 使用进程池
来源：http://hz.jiagoushi.top/gttdpzkuyx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.smart0.xyz/gtgfefpleh.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.dianchejie.cn/gtuijwpnnv.html

JS:   // child_process / cluster 模块
来源：http://hz.shangyingyoupin.top/gtysridpni.html

TS:   // child_process / cluster 模块
来源：http://hz.quarkkingdee.top/gtvxnwxejc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yvedp.cn/gtpvlamwss.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.sweek.top/gtpgparcjn.html

Ruby: // fork 块
来源：http://hz.hysaishi.cn/gtslqfmhlm.html

C#:   Parallel.For
来源：http://hz.cqqwz.cn/gtbxwcvbsb.html

================================================================================
来源：http://hz.cdnleiting.top/gtgbcwyhks.html

P. 常用工具函数
来源：http://hz.yanxiufei.cn/gtivdeqxhx.html

================================================================================
来源：http://hz.aibaodan.cn/gtmsaxkffz.html

[P01] 生成 UUID
来源：http://hz.xuetiantiany.cn/gtuzpwkaki.html

Py:   str(uuid.uuid4())
来源：http://hz.chenzaomai.com/gtpdtxcuqc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.sweek.top/gttxijagcx.html

JS:   crypto.randomUUID()
来源：http://hz.hnxiangtu.top/gtazbxrxvz.html

TS:   crypto.randomUUID()
来源：http://hz.9152youxi.cn/gtlenwzwmj.html

Java: UUID.randomUUID().toString()
来源：http://hz.cheryme.top/gtriykeyaw.html

Go:   // 用 github.com/google/uuid
来源：http://hz.iojbl.cn/gtqoecroku.html

Ruby: SecureRandom.uuid
来源：http://hz.hnxiangtu.top/gtokycyttj.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.havefunace.top/gtinujcglv.html

[P02] MD5 / SHA256 摘要
来源：http://hz.fengsongda.top/gtkasrcqjf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.fengsongda.top/gttevhffnw.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.aibaodan.cn/gtgwktyzyp.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.jlsjyb.cn/gtrcmxcopd.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.cucudq.cn/gtjppgfsne.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.zhixingplan.top/gtrkhrmyih.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.guannengcc.top/gtfgnbzonj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.316326.xyz/gtdwqdmqrl.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.nanxuanxn.top/gtntetyzfe.html

[P03] 生成短随机字符串
来源：http://hz.hysaishi.cn/gtohdxnmua.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.zdqjudy.top/gtswjpgyfu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.bjfxy.top/gtbqisfapk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.nanxinkj.top/gtjukhxezb.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.kuanghao11.cn/gtxazxoxai.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.gaohongyu789.top/gtjaiceiwx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.gzhubu.top/gtlbrdbyvx.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.gaohongyu789.top/gtciswwcvi.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.yongpay.top/gtusquyrfp.html

[P04] 求长度
来源：http://hz.gaohongyu789.top/gtkhlzpnlz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.yuanzhike.top/gtmmpkdrgb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.tanke756.top/gttyajzkne.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.dashuyun.cn/gtrdlkytln.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yanxiufei.cn/gtddzwbppg.html

Java: list.size();  map.size();  s.length()
来源：http://hz.ppjwa.cn/gthdywwvhp.html

Go:   len(arr);  len(m)
来源：http://hz.gotoacloud.top/gtdtzgkvgr.html

Ruby: x.length;  x.size
来源：http://hz.cqqwz.cn/gtwouxuvpv.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.zhijiandao.cn/gttuhyqequ.html

[P05] 判断两个对象内容是否相等
来源：http://hz.zycfv.cn/gtsbceuajd.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.aizwys.cn/gtqxgqqdad.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.hywenlv.cn/gtehuzfwgo.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.yanxiufei.cn/gtsupxjtmo.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zhongyouzk.top/gtwbxahmim.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.gaohongyu789.top/gtsmmzzoxi.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.chenlongwang.top/gtjafbypjh.html

Ruby: a == b
来源：http://hz.hammf.cn/gtsduhhpsr.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.yueranfly.top/gtgydmgacc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.birdmap.top/gtygtspaad.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.cdnleiting.top/gtbymtsens.html

PHP:  if (empty($x)) {}
来源：http://hz.jinyuanbaomall.cn/gtmjnqwxlt.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jinqigfzy.top/gtwhmqnzrh.html

TS:   if (x == null) {}
来源：http://hz.fzhhl.top/gtdfyxnfih.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.cheryme.top/gtxvvgbzta.html

Go:   if x == nil {}
来源：http://hz.kuanghao11.cn/gtfkkxlzah.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.cdnleiting.top/gtvqzcjrpz.html

C#:   if (x is null) {}
来源：http://hz.gotoacloud.top/gtysblirnj.html

[P07] 防抖与节流
来源：http://hz.yangfankeji.com/gtknyipfsu.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.c1oappe.top/gtjchjbfxm.html

PHP:  // 手写时间戳比较
来源：http://hz.bjfxy.top/gtpyzgeuxg.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.nanxinkj.top/gtpniighld.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.aizwys.cn/gtprytdlvw.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.shanyushiyangkeji.top/gthxbgqznp.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.aizwys.cn/gtenqypnrj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.kuanghao11.cn/gtjhxuizqm.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.52xcode.cn/gtiudqpewe.html

[P08] 处理浮点精度问题
来源：http://hz.dashuyun.cn/gticamikxz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.aibaodan.cn/gtfymhyqxy.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.c1oappe.top/gtypareruc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.zdqjudy.top/gtoepjyhyp.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.smart0.xyz/gtwuvlqtmu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.zhoulong.xyz/gtifkshphi.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.quarkkingdee.top/gtyfeteiee.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.jianghu66.top/gtssdowlnu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.gaohongyu789.top/gtzvptppcq.html

================================================================================
来源：http://hz.guannengcc.top/gteyzgbbtk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.jinyuanbaomall.cn/gtslrazwby.html

================================================================================
来源：http://hz.snrcjt.cn/gtkqcsbfuf.html

[Q01] 创建表
来源：http://hz.shanyushiyangkeji.top/gtcxhvwehe.html

CREATE TABLE users (
来源：http://hz.hywenlv.cn/gtjsskgxys.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.daxiang520.top/gtpmnvfxdl.html

name VARCHAR(50) NOT NULL,
来源：http://hz.zhiwuduotai.top/gtrwoxycfq.html

email VARCHAR(100) UNIQUE,
来源：http://hz.dianchejie.cn/gtzaygwoic.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.jinqigfzy.top/gtlbpafwhy.html

);
来源：http://hz.pengpengdd.cyou/gtlsgtmpen.html

[Q02] 创建带外键的表
来源：http://hz.316326.xyz/gtdrcagnig.html

CREATE TABLE orders (
来源：http://hz.quarkkingdee.top/gtxyqfmksd.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.pengpengdd.cyou/gtdomzaswm.html

user_id INT NOT NULL,
来源：http://hz.redwolf501.top/gtyizipvig.html

amount DECIMAL(10, 2),
来源：http://hz.yj20258.top/gtvicgopev.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.dianchejie.cn/gtlitkbjug.html

);
来源：http://hz.aizwys.cn/gtgzmlkzdt.html

[Q03] 增加列
来源：http://hz.redwolf501.top/gtooumtaib.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.hnqzz.top/gtkfeqyinv.html

[Q04] 修改列类型
来源：http://hz.dashuyun.cn/gtjruotrtu.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.haohaochexian.top/gtmdtxtzpf.html

[Q05] 重命名列
来源：http://hz.gzhubu.top/gtrttutyqd.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.aizwys.cn/gtszlrhiah.html

[Q06] 删除列
来源：http://hz.hammf.cn/gttfnajxok.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.meibo888.top/gthxyotuaj.html

[Q07] 删除表
来源：http://hz.yvedp.cn/gtmrnpgzre.html

DROP TABLE IF EXISTS orders;
来源：http://hz.mhx1999.top/gtbkboosjb.html

[Q08] 创建普通索引
来源：http://hz.sxryk.cn/gtubwiouyd.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.chenzaomai.com/gtzsazvghe.html

[Q09] 创建唯一索引
来源：http://hz.gogol.net.cn/gtbedwtqub.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.hongshengwenyu.top/gtzxoxymqe.html

[Q10] 插入单行
来源：http://hz.wangshuangyany.cn/gtqbipoyab.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.cheryme.top/gtrgokwmmp.html

[Q11] 一次插入多行
来源：http://hz.svipenyu.cn/gtlxztrjma.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.hnxiangtu.top/gtlsmfjoal.html

[Q12] 插入后取自增 ID
来源：http://hz.andypj.xyz/gtplvtwjxw.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.guannengcc.top/gtiqcxutun.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.chenjidiqi.icu/gttmbnfajh.html

[Q13] 忽略重复插入
来源：http://hz.yj20258.top/gtdkkmqeqw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.havefunace.top/gtavlydfmi.html

[Q14] 存在则更新（upsert）
来源：http://hz.vqdsnc.cn/gtwvbmlmwl.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.jinqigfzy.top/gtrsicuiyy.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.jyoumei.cn/gtzzdzgpkg.html

[Q15] 查询全部
来源：http://hz.sysykeji.top/gtobfalewf.html

SELECT * FROM users;
来源：http://hz.iojbl.cn/gtjtxxgaqu.html

[Q16] 查询指定列
来源：http://hz.nanxinkj.top/gtdhkfjhns.html

SELECT id, name FROM users;
来源：http://hz.c1oappe.top/gtgawllvtc.html

[Q17] 条件查询
来源：http://hz.shangyingyoupin.top/gtkscjnwev.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.yueranfly.top/gtlmqtgoce.html

[Q18] 模糊匹配
来源：http://hz.jlsjyb.cn/gtsoqaxusw.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.ivvv.top/gtzjdispaw.html

[Q19] 范围查询
来源：http://hz.jlsjyb.cn/gtgevasesz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.smart0.xyz/gtltnytxgm.html

[Q20] IN 列表
来源：http://hz.xylfe.cn/gtwylktplg.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.fzhhl.top/gteyjntekc.html

[Q21] 空值判断
来源：http://hz.xziqi.cn/gtgqblexra.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.sweek.top/gtwcphvmfp.html

[Q22] 排序
来源：http://hz.ppjwa.cn/gtihlmawik.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.dashuyun.cn/gtzvztuzcx.html

[Q23] 分页
来源：http://hz.zhongyouzk.top/gtpkoitjyf.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.quarkkingdee.top/gtravmrhou.html

[Q24] 去重
来源：http://hz.yuxming.cn/gtaowcbhax.html

SELECT DISTINCT city FROM users;
来源：http://hz.tianlin.xyz/gtrezguciz.html

[Q25] 只取前 N 条
来源：http://hz.redwolf501.top/gtzqxosctg.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.jqgufenzy.top/gtovskuotu.html

[Q26] 计数
来源：http://hz.svipenyu.cn/gtbdcmxbey.html

SELECT COUNT(*) FROM users;
来源：http://hz.zhiwuduotai.top/gthhvxsaed.html

[Q27] 条件计数
来源：http://hz.wangdashe.top/gtgnprlzrk.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.tianlin.xyz/gtvdofhhre.html

[Q28] 求和与平均
来源：http://hz.cqqwz.cn/gtywoljtso.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.fengsongda.top/gtwakbthcu.html

[Q29] 最大最小值
来源：http://hz.gaohongyu789.top/gtvubykorc.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.ppjwa.cn/gtlwmisjzv.html

[Q30] 分组统计
来源：http://hz.daxiang520.top/gtbphreeal.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.gogol.net.cn/gtosbpzgln.html

[Q31] 分组后过滤
来源：http://hz.zhoulong.xyz/gtulnqwkyn.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yj202588.top/gttyirvdro.html

[Q32] 分组拼接字符串
来源：http://hz.hnqzz.top/gtcaizbupm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.shanyushiyangkeji.top/gtyaqjzqsw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.hammf.cn/gtmehhlsjb.html

[Q33] 多列分组
来源：http://hz.jyoumei.cn/gtgcsaudax.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.52xcode.cn/gtfnhuzkew.html

[Q34] 每组取第一条
来源：http://hz.haohaochexian.top/gthpmekzrd.html

SELECT * FROM (
来源：http://hz.hnxiangtu.top/gtjtjsetyy.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.hongshengwenyu.top/gteodtnhsp.html

) t WHERE rn = 1;
来源：http://hz.hammf.cn/gtsypdjlze.html

[Q35] 内连接
来源：http://hz.yueranfly.top/gtijwrjcgi.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.ydzc1.top/gtexhyswip.html

[Q36] 左连接
来源：http://hz.aibaodan.cn/gtpmihfdpy.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.c1oappe.top/gtiyzsocev.html

[Q37] 右连接
来源：http://hz.yvedp.cn/gtbelllpph.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.birdmap.top/gtdfmmykfb.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.chenlongwang.top/gtuhtjjcpc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.smart0.xyz/gtinzsucdv.html

[Q39] 自连接（查上下级）
来源：http://hz.sysykeji.top/gtvzhtvqnk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.gogol.net.cn/gtjapybasi.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.shangyingyoupin.top/gtrkuemaat.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.yangfankeji.com/gtkrpmqqke.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.yj20258.top/gtgnfqvfnc.html

[Q41] 多表连接
来源：http://hz.zhengqikj.top/gtukrovwtb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.cheryme.top/gtkgvgtbqv.html

JOIN users u ON u.id = o.user_id
来源：http://hz.0kj1m.cn/gtvaddmden.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.zhiwuduotai.top/gteumwgiqe.html

[Q42] 连接条件附加过滤
来源：http://hz.shuidangran.top/gtilkyjvyh.html

SELECT u.name, o.amount FROM users u
来源：http://hz.pycfn.com/gtsltegeqg.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.sweek.top/gttimawzfl.html

[Q43] 标量子查询
来源：http://hz.cashguo.top/gtqpwzubkq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yj202588.top/gtcyszjkqb.html

[Q44] IN 子查询
来源：http://hz.smart0.xyz/gtrmczfrdl.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.ppjwa.cn/gtockhrrmc.html

[Q45] EXISTS 判断存在
来源：http://hz.c1oappe.top/gtuolttvaf.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.cdnleiting.top/gtcgtqgwrh.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.dashuyun.cn/gtybcxjlnn.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.cdnleiting.top/gtawhzihey.html

[Q47] 与平均值比较
来源：http://hz.yvedp.cn/gttgarqmpk.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.quarkkingdee.top/gthdptzzwo.html

[Q48] CTE 公用表表达式
来源：http://hz.feifeiyinyue.top/gtgwvhgtbk.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.iojbl.cn/gtozptoyys.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.ppjwa.cn/gtapdsipot.html

[Q49] 更新单行
来源：http://hz.wangdashe.top/gtbdprfsfr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yueranfly.top/gtzlrzuskv.html

[Q50] 批量更新
来源：http://hz.chenjidiqi.icu/gtutiagxed.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.shzxlz.cn/gttxwpoill.html

[Q51] 用子查询更新
来源：http://hz.redwolf501.top/gthntehbgf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.jyoumei.cn/gtgijywouv.html

[Q52] 删除指定行
来源：http://hz.gzhubu.top/gtjrtjnxna.html

DELETE FROM users WHERE id = 10;
来源：http://hz.hammf.cn/gtfcclvdei.html

[Q53] 按条件删除
来源：http://hz.sysykeji.top/gtqkkzqunq.html


<!-- 参考信息 -->