代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.sweek.top/gthqycdbhz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.zhijiandao.cn/gtciimilce.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.cashguo.top/gtvtnoikdf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.ywan-chungtsiang.top/gtqatsynnq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.52xcode.cn/gtbnzlhshc.html

[N10] 链表节点定义
来源：http://hz.zycfv.cn/gtayratmus.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yvedp.cn/gtzlkeuisn.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.hnxiangtu.top/gtwqhgozld.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yj20258888.top/gtdfbphtsi.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.cdnleiting.top/gtcthrvodf.html

Java: class Node { int v; Node next; }
来源：http://hz.chenlongwang.top/gtgpseixib.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.dianchejie.cn/gtcmnrtsgq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.yanxiufei.cn/gtuxircloz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.shuidangran.top/gtaysjenfm.html

[N11] 二叉树中序遍历
来源：http://hz.tianlin.xyz/gtglhezufj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.tian-w.cn/gtuojdynvg.html

PHP:  // 手写递归函数
来源：http://hz.9152youxi.cn/gtrdozyrok.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jlsjyb.cn/gtojjykoru.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yuanzhike.top/gtggotmsmj.html

Java: // 手写递归
来源：http://hz.nanxuanxn.top/gtjhwpigzu.html

Go:   // 手写递归
来源：http://hz.zhongyouzk.top/gtdupyruwq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.yueranfly.top/gtkdovncri.html

C#:   // 手写递归
来源：http://hz.wangdashe.top/gtjwildrpx.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yj20258888.top/gtqffynase.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.zhijiandao.cn/gtdcbjuvor.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.zhaomingkeji.xyz/gteqtwrmgr.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.bjfxy.top/gtvuvshetq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.iojbl.cn/gtwzpxfaup.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.gaohongyu789.top/gtnvxktomf.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.guowangkeji.top/gtjqerczvf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.mhx1999.top/gtdazdxwpz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.vqdsnc.cn/gtewbrixtq.html

================================================================================
来源：http://hz.smart0.xyz/gtiwhsdstw.html

O. 并发与异步
来源：http://hz.kuanghao11.cn/gthcylolqa.html

================================================================================
来源：http://hz.zhijiandao.cn/gtgbhfwxfe.html

[O01] 启动一个线程
来源：http://hz.meibo888.top/gtpjpuinif.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.hammf.cn/gtqubuorzk.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.quarkkingdee.top/gtolhkyhgr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.jqgfzy.top/gtrlpnwkgg.html

TS:   // 同 JS
来源：http://hz.zdqjudy.top/gtboyeyrdr.html

Java: new Thread(() -> f()).start()
来源：http://hz.ivvv.top/gthsekelrl.html

Go:   go f()
来源：http://hz.gzhubu.top/gtgafgazip.html

Ruby: Thread.new { f }
来源：http://hz.guowangkeji.top/gthrbhjkdj.html

C#:   Task.Run(() => F());
来源：http://hz.cucudq.cn/gtcmhptedc.html

[O02] 使用线程池
来源：http://hz.mhx1999.top/gtwdosgrfp.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.xylfe.cn/gtklfoftpo.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.jyoumei.cn/gtinejdglo.html

JS:   // worker_threads 线程池
来源：http://hz.daxiang520.top/gtcajkqnyx.html

TS:   // worker_threads 线程池
来源：http://hz.wangdashe.top/gtydhrsbzj.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yuanzhike.top/gtwqltqaxb.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.xingfuxueyuan.xyz/gtgmaywzjs.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.zhongyouzk.top/gtpfxomkbi.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.hammf.cn/gtpffzufoh.html

[O03] 加锁保护共享数据
来源：http://hz.cdnleiting.top/gtcjgdiifb.html

Py:   with lock: shared += 1
来源：http://hz.jianghu66.top/gtymmkqdcf.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.sxryk.cn/gtvacuydlv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.snrcjt.cn/gtvlokqdxe.html

TS:   // 同 JS
来源：http://hz.xuanzx.com/gtjueqxgak.html

Java: synchronized (this) { shared++; }
来源：http://hz.zhengqikj.top/gtobrfdpdv.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.nanxinkj.top/gtoxauxern.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.52xcode.cn/gtexwxfnoi.html

C#:   lock (gate) { shared++; }
来源：http://hz.smart0.xyz/gtnbjvvrjp.html

[O04] 定义异步函数并等待
来源：http://hz.nanxuanxn.top/gtvvfkscjj.html

Py:   async def f():⏎    await g()
来源：http://hz.guowangkeji.top/gtdhcjntac.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.pycfn.com/gtwhyptwkm.html

JS:   async function f() { await g(); }
来源：http://hz.sufxvd.cn/gtusfoccdd.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.cucudq.cn/gttcqlpjjj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.havefunace.top/gtfsbpvpdj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.yangfankeji.com/gtzmncqskk.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yonumen.top/gtymwyoerk.html

C#:   async Task F() { await G(); }
来源：http://hz.zdqjudy.top/gtectoeank.html

[O05] 并发执行并等待全部完成
来源：http://hz.0kj1m.cn/gthisaoztl.html

Py:   asyncio.gather(*tasks)
来源：http://hz.svipenyu.cn/gtrcklsvrp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.chenlongwang.top/gtjlugavre.html

JS:   await Promise.all(tasks)
来源：http://hz.jiagoushi.top/gtwaebajah.html

TS:   await Promise.all(tasks)
来源：http://hz.ybcxt.top/gtlebhypgr.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.jqgufenzy.top/gtmfhvirmm.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yanxiufei.cn/gtwbspwikr.html

Ruby: threads.map(&:join)
来源：http://hz.smart0.xyz/gtinmoerwu.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.cdnleiting.top/gtvnafaetf.html

[O06] 使用进程池
来源：http://hz.dashuyun.cn/gtleqejqjg.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.zhoulong.xyz/gtcwxrsgmb.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.daxiang520.top/gtvqvymulz.html

JS:   // child_process / cluster 模块
来源：http://hz.guowangkeji.top/gtyqzcrjdm.html

TS:   // child_process / cluster 模块
来源：http://hz.xuanzx.com/gtmohizett.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.tian-w.cn/gtmofqdhec.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.yongpay.top/gtlmtyxccm.html

Ruby: // fork 块
来源：http://hz.zhaomingkeji.xyz/gtyetumetf.html

C#:   Parallel.For
来源：http://hz.yuxming.cn/gtepdvjalv.html

================================================================================
来源：http://hz.hnxiangtu.top/gtlzvrhlyt.html

P. 常用工具函数
来源：http://hz.chenzaomai.com/gtiqszroab.html

================================================================================
来源：http://hz.jqgfzy.top/gthxsadhuy.html

[P01] 生成 UUID
来源：http://hz.hnxiangtu.top/gthwztfqgd.html

Py:   str(uuid.uuid4())
来源：http://hz.daria6918.cn/gtjukrrcyd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.gogol.net.cn/gtpsxgliep.html

JS:   crypto.randomUUID()
来源：http://hz.wangshuangyany.cn/gtvcoyhfff.html

TS:   crypto.randomUUID()
来源：http://hz.52xcode.cn/gtdtbggpob.html

Java: UUID.randomUUID().toString()
来源：http://hz.zhengqikj.top/gtgujgihtx.html

Go:   // 用 github.com/google/uuid
来源：http://hz.xylfe.cn/gtuqfmktjj.html

Ruby: SecureRandom.uuid
来源：http://hz.yueranfly.top/gtaztyzgdy.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.vqdsnc.cn/gtslbeiqzm.html

[P02] MD5 / SHA256 摘要
来源：http://hz.tian-w.cn/gtytsfseoy.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.vqdsnc.cn/gtbfvajkaz.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.tian-w.cn/gtcghmquqt.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.xinyue.icu/gtoyjwvzhl.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jinqigufen.top/gtbkbftwae.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.tianlin.xyz/gtzjnyjccl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.feifeiyinyue.top/gtfiunifjk.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.snrcjt.cn/gtbmcckins.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.zhiwuduotai.top/gtmxlvhugl.html

[P03] 生成短随机字符串
来源：http://hz.jqgufenzy.top/gtejfqkwbk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.chenzaomai.com/gtpelftzyq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.yj20258.top/gtojaqkpcw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ivvv.top/gtltgfwtnk.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yj20258.top/gtphfsixsg.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.quarkkingdee.top/gthcpafvly.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.zhengqikj.top/gtlqzyuznh.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.fzhhl.top/gtpeddmmwx.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.9152youxi.cn/gtbgftufuc.html

[P04] 求长度
来源：http://hz.yj202588.top/gtqngcptkr.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.aizwys.cn/gtxnqpflgj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hfpthk.cn/gtxsxmkbgx.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.cashguo.top/gtzaxkzhpi.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ybcxt.top/gtfprfnwiq.html

Java: list.size();  map.size();  s.length()
来源：http://hz.dashuyun.cn/gtzdfojuqv.html

Go:   len(arr);  len(m)
来源：http://hz.andypj.xyz/gtyqwuetar.html

Ruby: x.length;  x.size
来源：http://hz.316326.xyz/gtjopespcc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.nanxuanxn.top/gthhztbtbq.html

[P05] 判断两个对象内容是否相等
来源：http://hz.nwbrower.top/gtroealpmr.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.zhengqikj.top/gtptydwlde.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.daxiang520.top/gtsbgcvbae.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.pengpengdd.cyou/gtdikpgccs.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.kuanghao11.cn/gtiinroqqb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.shanyushiyangtech.top/gtwfofueqk.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.shzxlz.cn/gtrvcwrdix.html

Ruby: a == b
来源：http://hz.ywan-chungtsiang.top/gtmqgzmsuy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.shuidangran.top/gtdxhbaxrl.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.9152youxi.cn/gtvkqydcfv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.hysaishi.cn/gtrahogjqj.html

PHP:  if (empty($x)) {}
来源：http://hz.chenzaomai.com/gtrayoplqi.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.shanyushiyangkeji.top/gtpsiikigr.html

TS:   if (x == null) {}
来源：http://hz.guowangkeji.top/gttqbldevg.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.xuetiantiany.cn/gtrfizqcxg.html

Go:   if x == nil {}
来源：http://hz.andypj.xyz/gtjhnerpuf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.hammf.cn/gtgwzjbxjf.html

C#:   if (x is null) {}
来源：http://hz.mhx1999.top/gtxngjpsyx.html

[P07] 防抖与节流
来源：http://hz.cheryme.top/gtmcxglrcm.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.zycfv.cn/gtrlrhafgu.html

PHP:  // 手写时间戳比较
来源：http://hz.pengpengdd.cyou/gthntpdses.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.nanxuanxn.top/gtzqnzshwj.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ybcxt.top/gtgmeozezk.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.daxiang520.top/gtlqnwnhcv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.cashguo.top/gtakgkckhl.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.tanke756.top/gtbupkbpft.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.cdnleiting.top/gtvfquzhjj.html

[P08] 处理浮点精度问题
来源：http://hz.dianchejie.cn/gtlvltcalm.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.xinyue.icu/gtkjttlvdf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.fengsongda.top/gtnzpoluse.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.vqdsnc.cn/gtapkvjmpj.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.hongshengwenyu.top/gtqsfkjphv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yuxming.cn/gtvudbvvyd.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.chenzaomai.com/gtttefmsko.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.daxiang520.top/gtclgdhcxa.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.yuxming.cn/gtgfbdzkny.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtsjmjlbcp.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.sufxvd.cn/gtfzwsygxp.html

================================================================================
来源：http://hz.c1oappe.top/gtkxtqvaam.html

[Q01] 创建表
来源：http://hz.guannengcc.top/gtikukazjj.html

CREATE TABLE users (
来源：http://hz.chenlongwang.top/gtwaeaoovr.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.kuanghao11.cn/gtxvxxviqp.html

name VARCHAR(50) NOT NULL,
来源：http://hz.svipenyu.cn/gtjsqwqkxd.html

email VARCHAR(100) UNIQUE,
来源：http://hz.zhongyouzk.top/gtaxbkikcs.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.tanke756.top/gtswgshwuc.html

);
来源：http://hz.c1oappe.top/gtxwlnceej.html

[Q02] 创建带外键的表
来源：http://hz.pycfn.com/gtbzjsymkn.html

CREATE TABLE orders (
来源：http://hz.ydjk.org.cn/gtzzmnuotm.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jqgfzy.top/gtuyijxzjx.html

user_id INT NOT NULL,
来源：http://hz.yuanzhike.top/gtoxnszmqw.html

amount DECIMAL(10, 2),
来源：http://hz.xuanzx.com/gtvfwimvnm.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.snrcjt.cn/gtnzjsuvem.html

);
来源：http://hz.yangfankeji.com/gtuaocarzd.html

[Q03] 增加列
来源：http://hz.smart0.xyz/gtarlgoitx.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.chenlongwang.top/gtdcrjiluy.html

[Q04] 修改列类型
来源：http://hz.daria6918.cn/gtwrrqxcll.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.jinqigufen.top/gtfrcxbinm.html

[Q05] 重命名列
来源：http://hz.haohaochexian.top/gtzyuizyyq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.shangyingyoupin.top/gtwgdryvrz.html

[Q06] 删除列
来源：http://hz.sweek.top/gtvlyxqics.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.yvedp.cn/gtskdzjrqb.html

[Q07] 删除表
来源：http://hz.xylfe.cn/gtpxgvotjo.html

DROP TABLE IF EXISTS orders;
来源：http://hz.cdnleiting.top/gtgvgdhjel.html

[Q08] 创建普通索引
来源：http://hz.jinyuanbaomall.cn/gtdzfrmonv.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.dianchejie.cn/gtrdeihvcx.html

[Q09] 创建唯一索引
来源：http://hz.gogol.net.cn/gtnwdurxdx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.zycfv.cn/gtphjpnzzc.html

[Q10] 插入单行
来源：http://hz.jinyuanbaomall.cn/gtpwnyhjrw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jinyuanbaomall.cn/gtylgomsel.html

[Q11] 一次插入多行
来源：http://hz.jinyuanbaomall.cn/gtfdwuozjw.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.jinyuanbaomall.cn/gtcmiebysh.html

[Q12] 插入后取自增 ID
来源：http://hz.yuanzhike.top/gtichwgcux.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.shuidangran.top/gtjpvobfhx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.jinghuilouyu.cn/gtddyqozrf.html

[Q13] 忽略重复插入
来源：http://hz.dashuyun.cn/gtqroetuhr.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.sufxvd.cn/gtzzxgccjh.html

[Q14] 存在则更新（upsert）
来源：http://hz.kuanghao11.cn/gtdgjahgcp.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.jqgfzy.top/gtmmokcosw.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.dashuyun.cn/gtypqqhioc.html

[Q15] 查询全部
来源：http://hz.jqgfzy.top/gtpyhfmxho.html

SELECT * FROM users;
来源：http://hz.ppjwa.cn/gtujtpdbjc.html

[Q16] 查询指定列
来源：http://hz.pycfn.com/gthwdkxykl.html

SELECT id, name FROM users;
来源：http://hz.jiagoushi.top/gtvbzgghqr.html

[Q17] 条件查询
来源：http://hz.yuxming.cn/gtanqqnfjr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.meibo888.top/gthykwzyhd.html

[Q18] 模糊匹配
来源：http://hz.dashuyun.cn/gtsobiymlq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.zhiwuduotai.top/gtpipmrtto.html

[Q19] 范围查询
来源：http://hz.ydjk.org.cn/gtgwcwtqjb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.chenlongwang.top/gtykpiqugi.html

[Q20] IN 列表
来源：http://hz.jinqigufen.top/gtpyqhnvuv.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.smart0.xyz/gtshworgbk.html

[Q21] 空值判断
来源：http://hz.guannengcc.top/gtbrqdpiya.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.jiagoushi.top/gtwgzkeyif.html

[Q22] 排序
来源：http://hz.ydzc1.top/gtodsbcurq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.zhoulong.xyz/gtncpvspcp.html

[Q23] 分页
来源：http://hz.hysaishi.cn/gtnbiaania.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.ehwqpu.com/gtbpwswpdf.html

[Q24] 去重
来源：http://hz.tianlin.xyz/gtvhirbrfr.html

SELECT DISTINCT city FROM users;
来源：http://hz.jinghuilouyu.cn/gtmkevzgtw.html

[Q25] 只取前 N 条
来源：http://hz.guannengcc.top/gtoafcgmgp.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.sysykeji.top/gtcfdffjld.html

[Q26] 计数
来源：http://hz.hysaishi.cn/gtquuohaxu.html

SELECT COUNT(*) FROM users;
来源：http://hz.jianghu66.top/gtiydnnjzs.html

[Q27] 条件计数
来源：http://hz.yangfankeji.com/gtrjgfohah.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.guowangkeji.top/gtyjqwshqk.html

[Q28] 求和与平均
来源：http://hz.yanxiufei.cn/gtskjgxuzh.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.sweek.top/gtnjhbslwo.html

[Q29] 最大最小值
来源：http://hz.vqdsnc.cn/gtupxvurwh.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.jiagoushi.top/gtfjimdgfd.html

[Q30] 分组统计
来源：http://hz.jinghuilouyu.cn/gtxuxouupd.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.xinyue.icu/gtcvfrqfix.html

[Q31] 分组后过滤
来源：http://hz.jinqigfzy.top/gtixkwvgwv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yueranfly.top/gtaueghfju.html

[Q32] 分组拼接字符串
来源：http://hz.zhixingplan.top/gtkbozlxtq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.zhengqikj.top/gtlumhfbvi.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yj202588.top/gtyqtvqzlx.html

[Q33] 多列分组
来源：http://hz.hfpthk.cn/gtztqqspax.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.9152youxi.cn/gtdkxverpb.html

[Q34] 每组取第一条
来源：http://hz.yanxiufei.cn/gtblwsosil.html

SELECT * FROM (
来源：http://hz.cashguo.top/gtojuklfzq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.hammf.cn/gtocqlmnwk.html

) t WHERE rn = 1;
来源：http://hz.yangfankeji.com/gtueopadof.html

[Q35] 内连接
来源：http://hz.xuetiantiany.cn/gtkjalyuxl.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.shangyingyoupin.top/gtiywhcgjk.html

[Q36] 左连接
来源：http://hz.ehwqpu.com/gtnfjdokdc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.yj20258888.top/gtudsxhben.html

[Q37] 右连接
来源：http://hz.nwbrower.top/gtjcvjvfjz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.wangshuangyany.cn/gtdcujirqv.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.sweek.top/gtylymftor.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.xinyue.icu/gtrcnbunuf.html

[Q39] 自连接（查上下级）
来源：http://hz.nanxuanxn.top/gthddgamoq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.hnqzz.top/gtaojagrno.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.wangshuangyany.cn/gtmlrtqwoc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.chenlongwang.top/gtupobzmcg.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.cdnleiting.top/gtetovsdin.html

[Q41] 多表连接
来源：http://hz.52xcode.cn/gtnjytfzsv.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.zhengqikj.top/gtfypxbato.html

JOIN users u ON u.id = o.user_id
来源：http://hz.gotoacloud.top/gtacbmhsfg.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.dashuyun.cn/gtlxmibazm.html

[Q42] 连接条件附加过滤
来源：http://hz.wangshuangyany.cn/gtqhxuwouv.html

SELECT u.name, o.amount FROM users u
来源：http://hz.xziqi.cn/gtyrnwdesc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yj202588.top/gtoqhctxqw.html

[Q43] 标量子查询
来源：http://hz.meibo888.top/gthnliovun.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.redwolf501.top/gtcqihfeop.html

[Q44] IN 子查询
来源：http://hz.jianghu66.top/gtesgszdrd.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.yuxming.cn/gtbwcbgnyd.html

[Q45] EXISTS 判断存在
来源：http://hz.jinqigfzy.top/gtpptmgoqi.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.gotoacloud.top/gtrupmvsha.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.0kj1m.cn/gtvqfumaeq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jiagoushi.top/gttpzxlgxq.html

[Q47] 与平均值比较
来源：http://hz.hnxiangtu.top/gtvbzkvlcv.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.yj20258888.top/gtletehzsi.html

[Q48] CTE 公用表表达式
来源：http://hz.shangyingyoupin.top/gtohjspiwn.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.andypj.xyz/gtofbppohg.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.9152youxi.cn/gtzjizihhu.html

[Q49] 更新单行
来源：http://hz.chenzaomai.com/gtqpulvjau.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.daria6918.cn/gtlngmxkmd.html

[Q50] 批量更新
来源：http://hz.ehwqpu.com/gtsfyydbwo.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.316326.xyz/gtgwkcnjkn.html

[Q51] 用子查询更新
来源：http://hz.nanxuanxn.top/gtwowafjqv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.aizwys.cn/gthiiwcjus.html

[Q52] 删除指定行
来源：http://hz.smart0.xyz/gtilpnvmyp.html

DELETE FROM users WHERE id = 10;
来源：http://hz.hongshengwenyu.top/gtyvsoxrzh.html

[Q53] 按条件删除
来源：http://hz.xuetiantiany.cn/gtozrdwmth.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.guannengcc.top/gtuaksfegv.html

[Q54] 清空表
来源：http://hz.meibo888.top/gtlqnspqwy.html

TRUNCATE TABLE logs;
来源：http://hz.mhx1999.top/gtrhtnrjsm.html

[Q55] 排名（并列占位）
来源：http://hz.jqgfzy.top/gtibairfeq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.chenlongwang.top/gttivfqmxq.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jlsjyb.cn/gtubxyryen.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.316326.xyz/gtiralsduw.html

[Q57] 行号
来源：http://hz.hnqzz.top/gtilvetwph.html


<!-- 参考信息 -->