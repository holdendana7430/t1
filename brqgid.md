代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jqgfzy.top/gthcemskrd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yonumen.top/gtdyglldxc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.dianchejie.cn/gtkmjgjtqu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yvedp.cn/gtzyojsqtq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.shangyingyoupin.top/gtedzveadq.html

[N10] 链表节点定义
来源：http://hz.hysaishi.cn/gtfwjqjguh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.daxiang520.top/gthlajnyqv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.yuanzhike.top/gtisapxqof.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.iojbl.cn/gtyrtwhbkq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.gogol.net.cn/gtgpdyeizt.html

Java: class Node { int v; Node next; }
来源：http://hz.hywenlv.cn/gtfxfmbter.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.yj202588.top/gtybwonaqg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.aizwys.cn/gtmfhzyekg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.feifeiyinyue.top/gtiyoqnjos.html

[N11] 二叉树中序遍历
来源：http://hz.yueranfly.top/gtxdxhymmu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.zhijiandao.cn/gtorzhkvcm.html

PHP:  // 手写递归函数
来源：http://hz.ydjk.org.cn/gtklmjxmjx.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.xingfuxueyuan.xyz/gtzerogfsu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yonumen.top/gtiauozkho.html

Java: // 手写递归
来源：http://hz.dianchejie.cn/gtllcwxnln.html

Go:   // 手写递归
来源：http://hz.xylfe.cn/gtwybxzdct.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.gaohongyu789.top/gtzstnaacu.html

C#:   // 手写递归
来源：http://hz.andypj.xyz/gthmimmgdu.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.xuetiantiany.cn/gtayzrdfxu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.xuetiantiany.cn/gtrmshvsez.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jinqigfzy.top/gtjnjsbcnb.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yuxming.cn/gtirgzcmuj.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cheryme.top/gtcqtbdvqu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zycfv.cn/gtvycafueg.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.mhx1999.top/gtsmhkoxyz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.sxryk.cn/gtdihefwjn.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.tanke756.top/gtiqrujysb.html

================================================================================
来源：http://hz.nwbrower.top/gthtfjlypx.html

O. 并发与异步
来源：http://hz.daxiang520.top/gtqbusqpjo.html

================================================================================
来源：http://hz.gzhubu.top/gtworrtijz.html

[O01] 启动一个线程
来源：http://hz.xziqi.cn/gtemivzcip.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.redwolf501.top/gticcdojhv.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.gotoacloud.top/gtxmmutqps.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.kuanghao11.cn/gtiyfqlvvr.html

TS:   // 同 JS
来源：http://hz.chenjidiqi.icu/gtitvzgnpz.html

Java: new Thread(() -> f()).start()
来源：http://hz.guannengcc.top/gtondrwcys.html

Go:   go f()
来源：http://hz.quarkkingdee.top/gtqptnumdf.html

Ruby: Thread.new { f }
来源：http://hz.wangshuangyany.cn/gtftrypxib.html

C#:   Task.Run(() => F());
来源：http://hz.cashguo.top/gtpuzqyxtn.html

[O02] 使用线程池
来源：http://hz.sxryk.cn/gtbjqcuzlg.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.hnxiangtu.top/gtdblzlboq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.sweek.top/gtmzutscbc.html

JS:   // worker_threads 线程池
来源：http://hz.xingfuxueyuan.xyz/gtnciufdod.html

TS:   // worker_threads 线程池
来源：http://hz.ydjk.org.cn/gtyhyprloi.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.redwolf501.top/gtvxuifnqo.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.daxiang520.top/gtnnidayvv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.shuidangran.top/gtqntregxv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.52xcode.cn/gtcbfyjyyo.html

[O03] 加锁保护共享数据
来源：http://hz.cucudq.cn/gtqztxzyoq.html

Py:   with lock: shared += 1
来源：http://hz.gogol.net.cn/gtscnuagfn.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.ydjk.org.cn/gtndfarlxe.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.aibaodan.cn/gtxexgkcdk.html

TS:   // 同 JS
来源：http://hz.dashuyun.cn/gtfzomzmhu.html

Java: synchronized (this) { shared++; }
来源：http://hz.feifeiyinyue.top/gtykjjpgby.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.jinghuilouyu.cn/gtbaenjlpx.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.chenjidiqi.icu/gtghqnbcsg.html

C#:   lock (gate) { shared++; }
来源：http://hz.yj20258888.top/gtetaailej.html

[O04] 定义异步函数并等待
来源：http://hz.c1oappe.top/gtlpedlgco.html

Py:   async def f():⏎    await g()
来源：http://hz.nwbrower.top/gtkdxxkytf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.wangdashe.top/gthteuvsmg.html

JS:   async function f() { await g(); }
来源：http://hz.ydjk.org.cn/gttyvxzthb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.nanxuanxn.top/gtxdcjgjdn.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.zhongyouzk.top/gtmuvzlscf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.9152youxi.cn/gtajxqbmgg.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.vqdsnc.cn/gttmafvghr.html

C#:   async Task F() { await G(); }
来源：http://hz.jinyuanbaomall.cn/gtcrvxypcu.html

[O05] 并发执行并等待全部完成
来源：http://hz.yueranfly.top/gtnjcsfpzr.html

Py:   asyncio.gather(*tasks)
来源：http://hz.pengpengdd.cyou/gtsipxlciv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.guannengcc.top/gtzegnvsmp.html

JS:   await Promise.all(tasks)
来源：http://hz.zhixingplan.top/gtihggvuhs.html

TS:   await Promise.all(tasks)
来源：http://hz.yongpay.top/gtrlzoszii.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.andypj.xyz/gtiawlikly.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.chenjidiqi.icu/gtdtrgbwch.html

Ruby: threads.map(&:join)
来源：http://hz.shuidangran.top/gtwlcukgbp.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.chenlongwang.top/gttwynrxgd.html

[O06] 使用进程池
来源：http://hz.bjfxy.top/gtiftfbywc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.jianghu66.top/gteofpbzve.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.havefunace.top/gtctolprfr.html

JS:   // child_process / cluster 模块
来源：http://hz.cucudq.cn/gtcabntgzu.html

TS:   // child_process / cluster 模块
来源：http://hz.yanxiufei.cn/gthryliyjd.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jianghu66.top/gtrnnlduuv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.tanke756.top/gtgbmtbshz.html

Ruby: // fork 块
来源：http://hz.mhx1999.top/gtnrgwakxt.html

C#:   Parallel.For
来源：http://hz.haohaochexian.top/gtlhbuckyf.html

================================================================================
来源：http://hz.nanxuanxn.top/gthhyxqxvw.html

P. 常用工具函数
来源：http://hz.nanxinkj.top/gtnifillsx.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtcbyhjkmc.html

[P01] 生成 UUID
来源：http://hz.daxiang520.top/gttwtbqwqw.html

Py:   str(uuid.uuid4())
来源：http://hz.shangyingyoupin.top/gtomwawvuc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jinghuilouyu.cn/gtcdylzbdu.html

JS:   crypto.randomUUID()
来源：http://hz.yj20258.top/gtfzswmedv.html

TS:   crypto.randomUUID()
来源：http://hz.nanxuanxn.top/gtcedyfaab.html

Java: UUID.randomUUID().toString()
来源：http://hz.cashguo.top/gttvrbvlss.html

Go:   // 用 github.com/google/uuid
来源：http://hz.shzxlz.cn/gtpgvvhihr.html

Ruby: SecureRandom.uuid
来源：http://hz.nanxinkj.top/gtghymoato.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.feifeiyinyue.top/gtqtuuwyao.html

[P02] MD5 / SHA256 摘要
来源：http://hz.vqdsnc.cn/gtujpfhfer.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.jinqigfzy.top/gtsevifjjn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.ivvv.top/gtflriezin.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.zdqjudy.top/gtjxjkkdtn.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.dashuyun.cn/gtgkccsvxr.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.xziqi.cn/gtjvjniqnl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.0kj1m.cn/gtspiwrqyr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.fengsongda.top/gtumuslzbn.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.hfpthk.cn/gtjtyjecpd.html

[P03] 生成短随机字符串
来源：http://hz.cdnleiting.top/gtdwgqhjjo.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.tian-w.cn/gttasgxqtj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.cqqwz.cn/gtgkcxevel.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.cucudq.cn/gtgcurmanj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yangfankeji.com/gtytiphetu.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.tianlin.xyz/gtqnsvevxl.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yanxiufei.cn/gtyobzpugc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.dashuyun.cn/gtzsadrfbq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.shanyushiyangtech.top/gtnrzqlcsf.html

[P04] 求长度
来源：http://hz.shzxlz.cn/gthrnpjgza.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.shanyushiyangkeji.top/gtiyljsmyo.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.gotoacloud.top/gtbydkdgww.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yuxming.cn/gtifjnltfl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.cdnleiting.top/gtfvxqcpkf.html

Java: list.size();  map.size();  s.length()
来源：http://hz.quarkkingdee.top/gtoqisjiso.html

Go:   len(arr);  len(m)
来源：http://hz.xingfuxueyuan.xyz/gtxmnkooyp.html

Ruby: x.length;  x.size
来源：http://hz.feifeiyinyue.top/gtacedyytk.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.jlsjyb.cn/gttkgkqwsw.html

[P05] 判断两个对象内容是否相等
来源：http://hz.wangdashe.top/gthpedozqx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.nwbrower.top/gtiugeruii.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.nanxuanxn.top/gtnghrgjih.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.0kj1m.cn/gtfhhbbjeu.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.tian-w.cn/gtfhkdxzzt.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.gzhubu.top/gtqttqvqky.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.feifeiyinyue.top/gtgbcptdhc.html

Ruby: a == b
来源：http://hz.cqqwz.cn/gtzfttucng.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.316326.xyz/gtdwzonvjp.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.sysykeji.top/gtkpywyabq.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.shuidangran.top/gtshdgnhtu.html

PHP:  if (empty($x)) {}
来源：http://hz.jinqigufen.top/gtmvtavbcz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.ydjk.org.cn/gtmvgutohn.html

TS:   if (x == null) {}
来源：http://hz.zhaomingkeji.xyz/gtdaducwxz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.birdmap.top/gtazdwakzf.html

Go:   if x == nil {}
来源：http://hz.yj20258.top/gtvmtbfjio.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.xuetiantiany.cn/gtqxpwcqhf.html

C#:   if (x is null) {}
来源：http://hz.zycfv.cn/gtlzymclvg.html

[P07] 防抖与节流
来源：http://hz.hnxiangtu.top/gtxajixkym.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.xziqi.cn/gtmflrbcmu.html

PHP:  // 手写时间戳比较
来源：http://hz.chenlongwang.top/gtpcvpvfoc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.316326.xyz/gthbckdvbo.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.nwbrower.top/gtmfycqpgc.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.aibaodan.cn/gtwvhnbzdz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.zhaomingkeji.xyz/gtsmzeqili.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.shuidangran.top/gtzsuqxayc.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.vqdsnc.cn/gtwmqfhyyw.html

[P08] 处理浮点精度问题
来源：http://hz.svipenyu.cn/gtnknylevr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.yangfankeji.com/gtzpwtbife.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.zhengqikj.top/gtyonkrfdo.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.meibo888.top/gtdetjuvtl.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.fzhhl.top/gtvbgilzqm.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.dianchejie.cn/gtzhbrwptb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.sufxvd.cn/gtlquikzlj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.sysykeji.top/gtxyglgnof.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.nanxinkj.top/gtrhzrqhne.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtveulgrjv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.quarkkingdee.top/gtmheunzwx.html

================================================================================
来源：http://hz.haohaochexian.top/gtgwwmkuea.html

[Q01] 创建表
来源：http://hz.tianlin.xyz/gtbdqyvela.html

CREATE TABLE users (
来源：http://hz.gogol.net.cn/gtbszwfiat.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.gzhubu.top/gtloxlrgkr.html

name VARCHAR(50) NOT NULL,
来源：http://hz.andypj.xyz/gteeeygvos.html

email VARCHAR(100) UNIQUE,
来源：http://hz.yj20258.top/gtprigrasv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.snrcjt.cn/gtujvutihh.html

);
来源：http://hz.cashguo.top/gtnweakyaw.html

[Q02] 创建带外键的表
来源：http://hz.shanyushiyangkeji.top/gtytmaochf.html

CREATE TABLE orders (
来源：http://hz.yvedp.cn/gtbhbgfhto.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ywan-chungtsiang.top/gtvtaaufro.html

user_id INT NOT NULL,
来源：http://hz.ydzc1.top/gtikwoejjz.html

amount DECIMAL(10, 2),
来源：http://hz.jlsjyb.cn/gtcfwkllku.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.quarkkingdee.top/gtschwfxmq.html

);
来源：http://hz.jinqigufen.top/gtpqmelcax.html

[Q03] 增加列
来源：http://hz.aibaodan.cn/gtikobthtu.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.cucudq.cn/gtqhkwhqyy.html

[Q04] 修改列类型
来源：http://hz.birdmap.top/gtcyzcgked.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.jyoumei.cn/gtbblaayll.html

[Q05] 重命名列
来源：http://hz.bjfxy.top/gtqcokogtr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.ivvv.top/gtqkwlxscf.html

[Q06] 删除列
来源：http://hz.dashuyun.cn/gtttnexloj.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.zhixingplan.top/gtqhqkybxn.html

[Q07] 删除表
来源：http://hz.aizwys.cn/gtpkkamwms.html

DROP TABLE IF EXISTS orders;
来源：http://hz.kuanghao11.cn/gtowpndrup.html

[Q08] 创建普通索引
来源：http://hz.gogol.net.cn/gtxvrahtbp.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.pycfn.com/gtxzuylazd.html

[Q09] 创建唯一索引
来源：http://hz.zycfv.cn/gtoeudivjo.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.yuxming.cn/gtjnpwyfni.html

[Q10] 插入单行
来源：http://hz.vqdsnc.cn/gtmuamxrmq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.yj20258.top/gtlgugfwgu.html

[Q11] 一次插入多行
来源：http://hz.daria6918.cn/gtnatdutvs.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.mhx1999.top/gtzrsstamu.html

[Q12] 插入后取自增 ID
来源：http://hz.ivvv.top/gtgjotceiu.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.cdnleiting.top/gtvehlmfgr.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.jyoumei.cn/gtrymwlhvp.html

[Q13] 忽略重复插入
来源：http://hz.cdnleiting.top/gtocqfnovw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.yuxming.cn/gtblnwlxds.html

[Q14] 存在则更新（upsert）
来源：http://hz.aibaodan.cn/gtfglehvgb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.andypj.xyz/gtpemwdysv.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.sweek.top/gtvltimsec.html

[Q15] 查询全部
来源：http://hz.daria6918.cn/gtwhhbjxrf.html

SELECT * FROM users;
来源：http://hz.sxryk.cn/gttynbusys.html

[Q16] 查询指定列
来源：http://hz.zhixingplan.top/gttjeadwrm.html

SELECT id, name FROM users;
来源：http://hz.ivvv.top/gtliarvwql.html

[Q17] 条件查询
来源：http://hz.snrcjt.cn/gtosdpfmmp.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.jianghu66.top/gtsavozwae.html

[Q18] 模糊匹配
来源：http://hz.jinqigufen.top/gtiasfotds.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.shanyushiyangtech.top/gtwyrdswjv.html

[Q19] 范围查询
来源：http://hz.havefunace.top/gtjswhmsbq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.zhixingplan.top/gtlumivvci.html

[Q20] IN 列表
来源：http://hz.dianchejie.cn/gtpysecmoo.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.hnqzz.top/gtvouwaget.html

[Q21] 空值判断
来源：http://hz.gogol.net.cn/gtutiyqhwg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.nanxinkj.top/gtzcwpjfyo.html

[Q22] 排序
来源：http://hz.hysaishi.cn/gttrjuzihj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.bjfxy.top/gtowdcjsvd.html

[Q23] 分页
来源：http://hz.9152youxi.cn/gttyaipkri.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yuanzhike.top/gtlbnrvsos.html

[Q24] 去重
来源：http://hz.mhx1999.top/gtvdatdmlm.html

SELECT DISTINCT city FROM users;
来源：http://hz.9152youxi.cn/gtwwjbexar.html

[Q25] 只取前 N 条
来源：http://hz.ppjwa.cn/gtfgbxwinf.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.haohaochexian.top/gtxjgiuuam.html

[Q26] 计数
来源：http://hz.cashguo.top/gtnjtssbej.html

SELECT COUNT(*) FROM users;
来源：http://hz.jqgfzy.top/gttaqqftrl.html

[Q27] 条件计数
来源：http://hz.yuanzhike.top/gtgryrwqwq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.zhongyouzk.top/gtqnfvpmwk.html

[Q28] 求和与平均
来源：http://hz.zhoulong.xyz/gtzjrxxtws.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.yj20258888.top/gtudwfwjuf.html

[Q29] 最大最小值
来源：http://hz.dashuyun.cn/gtmlcablse.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.zhixingplan.top/gtrczyapvf.html

[Q30] 分组统计
来源：http://hz.jinghuilouyu.cn/gtutahlnoj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.zycfv.cn/gtymhnujlz.html

[Q31] 分组后过滤
来源：http://hz.vqdsnc.cn/gtvjivtgcv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.nanxuanxn.top/gtriidtifq.html

[Q32] 分组拼接字符串
来源：http://hz.zhengqikj.top/gtlxyeutxk.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.vqdsnc.cn/gtusmhdxhd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.bjfxy.top/gtfksculbz.html

[Q33] 多列分组
来源：http://hz.quarkkingdee.top/gtaykclabb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.zhengqikj.top/gtdwiupagk.html

[Q34] 每组取第一条
来源：http://hz.jlsjyb.cn/gtwbkrasjs.html

SELECT * FROM (
来源：http://hz.mhx1999.top/gtwannzdri.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.sxryk.cn/gtwqmllovu.html

) t WHERE rn = 1;
来源：http://hz.yj20258.top/gtrkvyjcfp.html

[Q35] 内连接
来源：http://hz.andypj.xyz/gtpwfpqenj.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.tian-w.cn/gtjssetyhf.html

[Q36] 左连接
来源：http://hz.jqgfzy.top/gtywvrrifk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.tanke756.top/gtcvhxwprh.html

[Q37] 右连接
来源：http://hz.ppjwa.cn/gthifvsniu.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.cqqwz.cn/gtaaspcekf.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.iojbl.cn/gtpsefcmbr.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.shuidangran.top/gtcieijnto.html

[Q39] 自连接（查上下级）
来源：http://hz.xingfuxueyuan.xyz/gtbvyiavbd.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.yj20258888.top/gtkljibihc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.snrcjt.cn/gtgjptdwxh.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.0kj1m.cn/gtdsuquaro.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.guannengcc.top/gtkjddewaj.html

[Q41] 多表连接
来源：http://hz.iojbl.cn/gtheqhytxx.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.316326.xyz/gtfvpfnzsk.html

JOIN users u ON u.id = o.user_id
来源：http://hz.cqqwz.cn/gtkficbgwd.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.jinqigufen.top/gtvyzjjsqf.html

[Q42] 连接条件附加过滤
来源：http://hz.yj20258888.top/gtlglhmfqk.html

SELECT u.name, o.amount FROM users u
来源：http://hz.cucudq.cn/gtdfzxklqm.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.birdmap.top/gtlowqlgdg.html

[Q43] 标量子查询
来源：http://hz.ydjk.org.cn/gtrjzfmfhr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.xuetiantiany.cn/gtczhbdajz.html

[Q44] IN 子查询
来源：http://hz.svipenyu.cn/gtvcasoxkt.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.tian-w.cn/gtcjnuxjuy.html

[Q45] EXISTS 判断存在
来源：http://hz.jinghuilouyu.cn/gtrmaiiiqg.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.ivvv.top/gtgfshlsvo.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.chenzaomai.com/gtwxyaijux.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.redwolf501.top/gtceswthcm.html

[Q47] 与平均值比较
来源：http://hz.svipenyu.cn/gtykkaywdh.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jqgfzy.top/gtwkjdigfs.html

[Q48] CTE 公用表表达式
来源：http://hz.yueranfly.top/gtmkxqhhdt.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.yuanzhike.top/gtgfkvefqy.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.0kj1m.cn/gtmtvjxdzj.html

[Q49] 更新单行
来源：http://hz.guowangkeji.top/gtpoxczuhk.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yj20258888.top/gtrirovhem.html

[Q50] 批量更新
来源：http://hz.shanyushiyangkeji.top/gtwqmcafhs.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.jyoumei.cn/gtdqlgktnd.html

[Q51] 用子查询更新
来源：http://hz.jinghuilouyu.cn/gtvnczmzzs.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.cqqwz.cn/gtftgszyej.html

[Q52] 删除指定行
来源：http://hz.daria6918.cn/gthgimbxpd.html

DELETE FROM users WHERE id = 10;
来源：http://hz.shangyingyoupin.top/gtuzpuwfif.html

[Q53] 按条件删除
来源：http://hz.jqgufenzy.top/gtqzrlbkil.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yvedp.cn/gtdsxipswe.html

[Q54] 清空表
来源：http://hz.yongpay.top/gtcyelgxnu.html

TRUNCATE TABLE logs;
来源：http://hz.snrcjt.cn/gtsnwcawrg.html

[Q55] 排名（并列占位）
来源：http://hz.aibaodan.cn/gtlncgsykl.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.ydjk.org.cn/gtxjotmpgd.html

[Q56] 密集排名（并列不占位）
来源：http://hz.gogol.net.cn/gthhiykssn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.316326.xyz/gtxcdmaczh.html

[Q57] 行号
来源：http://hz.jiagoushi.top/gtccokatqz.html


<!-- 参考信息 -->