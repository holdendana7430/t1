代发 wailian999

[N09] 栈与队列
来源：http://hz.snrcjt.cn/gtpecbdhjt.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.tian-w.cn/gtnqjekmai.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.zycfv.cn/gtapmpiebr.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.gaohongyu789.top/gtalmlmyep.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.zhijiandao.cn/gteisvvfgg.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.smart0.xyz/gtunjbwajr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.hysaishi.cn/gtuwouphzq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.jinyuanbaomall.cn/gtypakllxu.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.tianlin.xyz/gtylwnptve.html

[N10] 链表节点定义
来源：http://hz.316326.xyz/gtrlzqmcnp.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.bjfxy.top/gtzysmpzlu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.zhoulong.xyz/gtctojyyvz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yj20258888.top/gtvynxqemw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.yueranfly.top/gtwqckilkh.html

Java: class Node { int v; Node next; }
来源：http://hz.jqgufenzy.top/gtijvjsnem.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.gaohongyu789.top/gtcvpylzew.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.ehwqpu.com/gtlugzshvg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.smart0.xyz/gtwicynrsy.html

[N11] 二叉树中序遍历
来源：http://hz.cheryme.top/gtbnytynkg.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.ybcxt.top/gtfglqntsv.html

PHP:  // 手写递归函数
来源：http://hz.sxryk.cn/gtdeqvsfri.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.pycfn.com/gtbhsmldiz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jqgfzy.top/gtgdjvagwe.html

Java: // 手写递归
来源：http://hz.nwbrower.top/gtriugqywg.html

Go:   // 手写递归
来源：http://hz.hywenlv.cn/gttfldxxsb.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.cucudq.cn/gtruddraik.html

C#:   // 手写递归
来源：http://hz.zhoulong.xyz/gttlwfobue.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.quarkkingdee.top/gtigetaqiq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.chenlongwang.top/gtaybdqnsp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.yj202588.top/gtmswcqbpj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ywan-chungtsiang.top/gtevnfghby.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.havefunace.top/gtslamhind.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhixingplan.top/gtwfsiairb.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.zycfv.cn/gtkcqmuruf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.mhx1999.top/gtiisdpyae.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.nwbrower.top/gtwilginbz.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtzfkdbvav.html

O. 并发与异步
来源：http://hz.yuanzhike.top/gtbwzvhzqz.html

================================================================================
来源：http://hz.havefunace.top/gtblcpkzwm.html

[O01] 启动一个线程
来源：http://hz.hammf.cn/gtpwshzwaz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.0kj1m.cn/gtkcbklfvx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.ywan-chungtsiang.top/gtheshpapp.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.smart0.xyz/gtebepgfyp.html

TS:   // 同 JS
来源：http://hz.zhongyouzk.top/gtdkirjgnk.html

Java: new Thread(() -> f()).start()
来源：http://hz.pycfn.com/gtxoobzndt.html

Go:   go f()
来源：http://hz.ppjwa.cn/gtiszwabtz.html

Ruby: Thread.new { f }
来源：http://hz.dashuyun.cn/gtnmkvrytr.html

C#:   Task.Run(() => F());
来源：http://hz.yongpay.top/gtrpsyoryg.html

[O02] 使用线程池
来源：http://hz.quarkkingdee.top/gtolepazoe.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.jyoumei.cn/gtouujnflh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.ivvv.top/gtetbdthhe.html

JS:   // worker_threads 线程池
来源：http://hz.cucudq.cn/gtxpckyxhr.html

TS:   // worker_threads 线程池
来源：http://hz.ydzc1.top/gtykcciqqi.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.mhx1999.top/gtnvnjyxae.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.redwolf501.top/gturfxilmw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.ydjk.org.cn/gtchaixpzt.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.jiagoushi.top/gtkywpcyrx.html

[O03] 加锁保护共享数据
来源：http://hz.hammf.cn/gtjkacoqzx.html

Py:   with lock: shared += 1
来源：http://hz.tianlin.xyz/gtdtxfjrhk.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.ydjk.org.cn/gtbzyhjvbi.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.shzxlz.cn/gthoiqvajq.html

TS:   // 同 JS
来源：http://hz.daxiang520.top/gtcbplevzj.html

Java: synchronized (this) { shared++; }
来源：http://hz.andypj.xyz/gtftdfnabm.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yangfankeji.com/gttdibqonq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.fzhhl.top/gtubybpvwn.html

C#:   lock (gate) { shared++; }
来源：http://hz.0kj1m.cn/gtjoszousp.html

[O04] 定义异步函数并等待
来源：http://hz.smart0.xyz/gtbdaiqcdu.html

Py:   async def f():⏎    await g()
来源：http://hz.bjfxy.top/gtttsrcuye.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.cucudq.cn/gtdpbsdzhw.html

JS:   async function f() { await g(); }
来源：http://hz.fengsongda.top/gtjqlogoaj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.ywan-chungtsiang.top/gtjfrpcxyl.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.hywenlv.cn/gtkzaozmdt.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.xuanzx.com/gtryroaybt.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.wangshuangyany.cn/gtltfxyzuk.html

C#:   async Task F() { await G(); }
来源：http://hz.xingfuxueyuan.xyz/gtmpgsfmoj.html

[O05] 并发执行并等待全部完成
来源：http://hz.hongshengwenyu.top/gthieerbae.html

Py:   asyncio.gather(*tasks)
来源：http://hz.hfpthk.cn/gtxklkqcru.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.shanyushiyangtech.top/gtpehyjwld.html

JS:   await Promise.all(tasks)
来源：http://hz.dashuyun.cn/gtfcisuzuv.html

TS:   await Promise.all(tasks)
来源：http://hz.meibo888.top/gtdmvbfshy.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.ydzc1.top/gtvfqmdqpt.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.0kj1m.cn/gtvqzvnkji.html

Ruby: threads.map(&:join)
来源：http://hz.mhx1999.top/gtxeeusvck.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yongpay.top/gtenioofdd.html

[O06] 使用进程池
来源：http://hz.ehwqpu.com/gtmrnyvhdk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.jianghu66.top/gtkjqivegz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.shzxlz.cn/gtqyqkzosz.html

JS:   // child_process / cluster 模块
来源：http://hz.zhijiandao.cn/gtwfhxlanq.html

TS:   // child_process / cluster 模块
来源：http://hz.chenlongwang.top/gtvhfamhlu.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.tianlin.xyz/gtvntdpimm.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.tian-w.cn/gthzqnjoxo.html

Ruby: // fork 块
来源：http://hz.jyoumei.cn/gtvnocbvfr.html

C#:   Parallel.For
来源：http://hz.yueranfly.top/gtolcoedlx.html

================================================================================
来源：http://hz.shzxlz.cn/gtclzsnbcn.html

P. 常用工具函数
来源：http://hz.smart0.xyz/gtjsvwkjwx.html

================================================================================
来源：http://hz.52xcode.cn/gtsmurbrnx.html

[P01] 生成 UUID
来源：http://hz.yj20258888.top/gthzalmlrs.html

Py:   str(uuid.uuid4())
来源：http://hz.guannengcc.top/gtnblnchrf.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.52xcode.cn/gtgiokrsih.html

JS:   crypto.randomUUID()
来源：http://hz.birdmap.top/gteblfopft.html

TS:   crypto.randomUUID()
来源：http://hz.xylfe.cn/gtxaxqzjju.html

Java: UUID.randomUUID().toString()
来源：http://hz.jqgfzy.top/gtdeyxhwhl.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yuxming.cn/gtjikomwrx.html

Ruby: SecureRandom.uuid
来源：http://hz.jiagoushi.top/gtmxdhnecz.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.birdmap.top/gtoezfjaju.html

[P02] MD5 / SHA256 摘要
来源：http://hz.sxryk.cn/gtjprbtnxo.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.gotoacloud.top/gtxbhyhwzg.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.wangdashe.top/gtdcgiqadk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.cashguo.top/gtqmuhfhfv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.nanxinkj.top/gtqpakzbzp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.yj20258888.top/gtrgybxbpn.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.ehwqpu.com/gtgfbjedgb.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.yuanzhike.top/gtinwqjhui.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.xuanzx.com/gtzydjyymk.html

[P03] 生成短随机字符串
来源：http://hz.jinyuanbaomall.cn/gtrpymcaew.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.daria6918.cn/gthbcrzsbh.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.sufxvd.cn/gtutvembpb.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.cqqwz.cn/gtvqtdhspo.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhiwuduotai.top/gtywccqqlf.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.zhixingplan.top/gtiikmcfwn.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.hysaishi.cn/gtfuansoov.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jqgufenzy.top/gtynlhooky.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.guowangkeji.top/gtmjciiiha.html

[P04] 求长度
来源：http://hz.ehwqpu.com/gtlxnsbzrs.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.tian-w.cn/gtoobhvlrf.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.wangdashe.top/gtfxmzihgy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.fengsongda.top/gtkklolhwm.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yuxming.cn/gtxpmwervc.html

Java: list.size();  map.size();  s.length()
来源：http://hz.chenlongwang.top/gttyyqydyn.html

Go:   len(arr);  len(m)
来源：http://hz.hfpthk.cn/gthhpaocng.html

Ruby: x.length;  x.size
来源：http://hz.hysaishi.cn/gtfwceyoxo.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.zdqjudy.top/gtqbjtrcgk.html

[P05] 判断两个对象内容是否相等
来源：http://hz.wangshuangyany.cn/gtznilvsez.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.fengsongda.top/gtukxuzzmn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.meibo888.top/gtddipjgwi.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.hnqzz.top/gtsylsmudd.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.shuidangran.top/gtblnyekmh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.gzhubu.top/gteatmffhn.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.chenzaomai.com/gtktorxgeb.html

Ruby: a == b
来源：http://hz.wangshuangyany.cn/gtpqdgzowk.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.guannengcc.top/gtovgfzoej.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.jinghuilouyu.cn/gtmkjmbvij.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.yj202588.top/gtxeqhqiie.html

PHP:  if (empty($x)) {}
来源：http://hz.jinqigfzy.top/gtotdueidz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.svipenyu.cn/gtjrlbbtmr.html

TS:   if (x == null) {}
来源：http://hz.ywan-chungtsiang.top/gtprxmxinb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.yueranfly.top/gtddxbjygl.html

Go:   if x == nil {}
来源：http://hz.vqdsnc.cn/gtyotvmuly.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.yuxming.cn/gtujvectfu.html

C#:   if (x is null) {}
来源：http://hz.havefunace.top/gtbkhpownn.html

[P07] 防抖与节流
来源：http://hz.zdqjudy.top/gthwwedvxx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.chenjidiqi.icu/gtydeayfin.html

PHP:  // 手写时间戳比较
来源：http://hz.hammf.cn/gtisiaukct.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xingfuxueyuan.xyz/gtitxcgnsy.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yangfankeji.com/gtdvvhaimg.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.xuanzx.com/gtuadrymfg.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.yvedp.cn/gtzasdqovc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.bjfxy.top/gtbtniowia.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.daria6918.cn/gtpepdmxgl.html

[P08] 处理浮点精度问题
来源：http://hz.daxiang520.top/gtxbynqmqw.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.zhijiandao.cn/gtjwpysrqp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.quarkkingdee.top/gtapteoqws.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.jlsjyb.cn/gtqznzwcys.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.feifeiyinyue.top/gtfhporwfc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.xingfuxueyuan.xyz/gtdfdutvad.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.xylfe.cn/gtelacazwx.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.bjfxy.top/gtcifykjfe.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.0kj1m.cn/gtpzqjoncn.html

================================================================================
来源：http://hz.tanke756.top/gtxtwkpugk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.sysykeji.top/gtjlrctzpa.html

================================================================================
来源：http://hz.aibaodan.cn/gtbyxvhrdr.html

[Q01] 创建表
来源：http://hz.sufxvd.cn/gtdwvejfuh.html

CREATE TABLE users (
来源：http://hz.xuetiantiany.cn/gtgdenwxcz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.cheryme.top/gtkwotsdjc.html

name VARCHAR(50) NOT NULL,
来源：http://hz.mhx1999.top/gtvlsqcrtb.html

email VARCHAR(100) UNIQUE,
来源：http://hz.kuanghao11.cn/gtkbseouge.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.zdqjudy.top/gtxqnvswyw.html

);
来源：http://hz.yuxming.cn/gtehxlyllt.html

[Q02] 创建带外键的表
来源：http://hz.svipenyu.cn/gtpukveefy.html

CREATE TABLE orders (
来源：http://hz.wangshuangyany.cn/gtdcesdmqx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhengqikj.top/gtjzdblbdu.html

user_id INT NOT NULL,
来源：http://hz.yj20258888.top/gtludsmcgr.html

amount DECIMAL(10, 2),
来源：http://hz.yj202588.top/gtfweotrgo.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.feifeiyinyue.top/gtqykdrvbi.html

);
来源：http://hz.yueranfly.top/gtqbhoiexb.html

[Q03] 增加列
来源：http://hz.dashuyun.cn/gtkvpnpsck.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.zhongyouzk.top/gtxnbpmpjf.html

[Q04] 修改列类型
来源：http://hz.aibaodan.cn/gtiilkmjhl.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.tian-w.cn/gtatqwleiz.html

[Q05] 重命名列
来源：http://hz.yuxming.cn/gtnbpzfspt.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.nanxinkj.top/gtmhwwdquv.html

[Q06] 删除列
来源：http://hz.jinghuilouyu.cn/gtyxgavqkl.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.meibo888.top/gtqubjaecu.html

[Q07] 删除表
来源：http://hz.zhixingplan.top/gtvajlneqm.html

DROP TABLE IF EXISTS orders;
来源：http://hz.vqdsnc.cn/gtuminndrg.html

[Q08] 创建普通索引
来源：http://hz.cucudq.cn/gtgbatukrk.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.xuanzx.com/gtvfvxjtsf.html

[Q09] 创建唯一索引
来源：http://hz.chenzaomai.com/gtdyysmwiy.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.haohaochexian.top/gtlosxcnrd.html

[Q10] 插入单行
来源：http://hz.yj202588.top/gtyigattri.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.9152youxi.cn/gtabhowmqz.html

[Q11] 一次插入多行
来源：http://hz.316326.xyz/gtxjctcxbm.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.gzhubu.top/gtczdwamfe.html

[Q12] 插入后取自增 ID
来源：http://hz.shanyushiyangtech.top/gtzdspagnv.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.quarkkingdee.top/gtwxfkgfen.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.cheryme.top/gtuknenpqs.html

[Q13] 忽略重复插入
来源：http://hz.yj20258.top/gtukomviyx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.fengsongda.top/gtbrgiyayk.html

[Q14] 存在则更新（upsert）
来源：http://hz.iojbl.cn/gtkcrugalw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.zhengqikj.top/gtbcwniqyj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.cdnleiting.top/gtnuvlmdkj.html

[Q15] 查询全部
来源：http://hz.fengsongda.top/gtvjponkcd.html

SELECT * FROM users;
来源：http://hz.bjfxy.top/gtlsjejweo.html

[Q16] 查询指定列
来源：http://hz.shanyushiyangkeji.top/gtowlfdvkc.html

SELECT id, name FROM users;
来源：http://hz.zycfv.cn/gtvnzguhbu.html

[Q17] 条件查询
来源：http://hz.yuanzhike.top/gtvguvouri.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.zhijiandao.cn/gtwjskdsfd.html

[Q18] 模糊匹配
来源：http://hz.sweek.top/gtpzuoxaut.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.shanyushiyangkeji.top/gtsahvfkou.html

[Q19] 范围查询
来源：http://hz.wangdashe.top/gtvgkisxxn.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.sweek.top/gthwbknssy.html

[Q20] IN 列表
来源：http://hz.hammf.cn/gtxdavftmi.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.jiagoushi.top/gtvtnzxhpw.html

[Q21] 空值判断
来源：http://hz.bjfxy.top/gtsxxgxnif.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.yj20258.top/gtulxrrltv.html

[Q22] 排序
来源：http://hz.ywan-chungtsiang.top/gtqomtsnmt.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.jianghu66.top/gtzlpolnht.html

[Q23] 分页
来源：http://hz.havefunace.top/gtgbrnzcot.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.nanxinkj.top/gtdgciucog.html

[Q24] 去重
来源：http://hz.chenlongwang.top/gttgquezqq.html

SELECT DISTINCT city FROM users;
来源：http://hz.yongpay.top/gtjgaolazh.html

[Q25] 只取前 N 条
来源：http://hz.tianlin.xyz/gtaibboumn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.zhixingplan.top/gtatgecjhw.html

[Q26] 计数
来源：http://hz.shanyushiyangkeji.top/gtnviqxodf.html

SELECT COUNT(*) FROM users;
来源：http://hz.gotoacloud.top/gtzutvoapd.html

[Q27] 条件计数
来源：http://hz.cashguo.top/gtsyxpsnuq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.aibaodan.cn/gtpzaubueh.html

[Q28] 求和与平均
来源：http://hz.ppjwa.cn/gtyzsrtmdj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.daxiang520.top/gtbbvtfuds.html

[Q29] 最大最小值
来源：http://hz.hongshengwenyu.top/gtqvmkwbvl.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.jyoumei.cn/gtintyyout.html

[Q30] 分组统计
来源：http://hz.cucudq.cn/gtzlhmupvo.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.zhijiandao.cn/gtusmgolmb.html

[Q31] 分组后过滤
来源：http://hz.yj20258888.top/gtpqxjidys.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.nanxuanxn.top/gtwivitoyb.html

[Q32] 分组拼接字符串
来源：http://hz.nwbrower.top/gtwgqriumg.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.cheryme.top/gtqokxndtj.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yj20258888.top/gtwqjfpxxn.html

[Q33] 多列分组
来源：http://hz.dashuyun.cn/gtvtkkaclm.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.shzxlz.cn/gtqblklubs.html

[Q34] 每组取第一条
来源：http://hz.hnxiangtu.top/gtkzwgkrcc.html

SELECT * FROM (
来源：http://hz.9152youxi.cn/gtrtxflali.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.kuanghao11.cn/gttochpiew.html

) t WHERE rn = 1;
来源：http://hz.bjfxy.top/gtbtugbluj.html

[Q35] 内连接
来源：http://hz.birdmap.top/gtjpitizvy.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.dianchejie.cn/gtibemkubv.html

[Q36] 左连接
来源：http://hz.smart0.xyz/gthyyblpwy.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.ivvv.top/gtgycrzmrk.html

[Q37] 右连接
来源：http://hz.jiagoushi.top/gtcdnpliar.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.zycfv.cn/gtljrxeubn.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.chenzaomai.com/gtagxijfvh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.cashguo.top/gturrgaitz.html

[Q39] 自连接（查上下级）
来源：http://hz.svipenyu.cn/gtmjwcpklj.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.redwolf501.top/gtxsbfrnwf.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.zhongyouzk.top/gtuocrhjvy.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.ppjwa.cn/gttccsnbdb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.yanxiufei.cn/gtlcbmvsqh.html

[Q41] 多表连接
来源：http://hz.yj20258888.top/gtavejbyqp.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.hnxiangtu.top/gtgtkhtnlh.html

JOIN users u ON u.id = o.user_id
来源：http://hz.smart0.xyz/gtxdkblush.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.chenlongwang.top/gtrwqjoiew.html

[Q42] 连接条件附加过滤
来源：http://hz.daria6918.cn/gtbvcckhac.html

SELECT u.name, o.amount FROM users u
来源：http://hz.hfpthk.cn/gtittrajff.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.zhoulong.xyz/gtaazvoeoi.html

[Q43] 标量子查询
来源：http://hz.gotoacloud.top/gtbjhnthck.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yj20258888.top/gthniimudo.html

[Q44] IN 子查询
来源：http://hz.zhongyouzk.top/gtwifgmdjl.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.hywenlv.cn/gtfosuxvbm.html

[Q45] EXISTS 判断存在
来源：http://hz.haohaochexian.top/gtyhdyrdje.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jqgfzy.top/gtnvwzzhmy.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.dianchejie.cn/gtovetuwnd.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jyoumei.cn/gtfwqwpriz.html

[Q47] 与平均值比较
来源：http://hz.zdqjudy.top/gtxudbtudf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.chenlongwang.top/gttbqvajlp.html

[Q48] CTE 公用表表达式
来源：http://hz.52xcode.cn/gtpeymooil.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.cucudq.cn/gtbdtrpwfb.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.ehwqpu.com/gtvayldlct.html

[Q49] 更新单行
来源：http://hz.yongpay.top/gtknzdbgvw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.jinghuilouyu.cn/gtnxmgusoa.html

[Q50] 批量更新
来源：http://hz.daria6918.cn/gtknznvbwx.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.chenjidiqi.icu/gtqhsmzrkc.html

[Q51] 用子查询更新
来源：http://hz.jyoumei.cn/gtkordmgtx.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.aizwys.cn/gtqxljewya.html

[Q52] 删除指定行
来源：http://hz.guannengcc.top/gttfbcbolz.html

DELETE FROM users WHERE id = 10;
来源：http://hz.shzxlz.cn/gtgnmvjeex.html

[Q53] 按条件删除
来源：http://hz.xuetiantiany.cn/gtsthphafw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.xuanzx.com/gtonyimdfo.html

[Q54] 清空表
来源：http://hz.haohaochexian.top/gtshneuejr.html

TRUNCATE TABLE logs;
来源：http://hz.chenzaomai.com/gtffvbhrqd.html

[Q55] 排名（并列占位）
来源：http://hz.nanxuanxn.top/gtumqdhqqd.html


<!-- 参考信息 -->