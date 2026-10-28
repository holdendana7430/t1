代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yuxming.cn/gtlukyklsd.html

[N10] 链表节点定义
来源：http://hz.ywan-chungtsiang.top/gtiusrdffq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yongpay.top/gtupvfsnkq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.sweek.top/gtmxldhgvr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.nwbrower.top/gtkzkvwrzk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.sxryk.cn/gtsoaovbkd.html

Java: class Node { int v; Node next; }
来源：http://hz.guannengcc.top/gttbsbvjan.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.gaohongyu789.top/gtvhmhdnwn.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.guannengcc.top/gtrxrzdzde.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.dianchejie.cn/gtazyxygba.html

[N11] 二叉树中序遍历
来源：http://hz.xuanzx.com/gtboghvycv.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.shangyingyoupin.top/gtpuiynjbh.html

PHP:  // 手写递归函数
来源：http://hz.jianghu66.top/gtyvfextti.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.pycfn.com/gtyfaadkjq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.52xcode.cn/gthespgimq.html

Java: // 手写递归
来源：http://hz.jinyuanbaomall.cn/gtxypnsptl.html

Go:   // 手写递归
来源：http://hz.ywan-chungtsiang.top/gthqkmoyao.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.cqqwz.cn/gtrjtkbugo.html

C#:   // 手写递归
来源：http://hz.jinyuanbaomall.cn/gtdwthxezh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.hongshengwenyu.top/gtcwxgscvv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.jinqigfzy.top/gtuqzswmyc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.feifeiyinyue.top/gtaqtwekmu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yonumen.top/gtcsywnbza.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jqgufenzy.top/gtepmmekxl.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.0kj1m.cn/gtizoancie.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.0kj1m.cn/gtrqaavmwv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.jianghu66.top/gtcbhhvccy.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.pengpengdd.cyou/gtoblsjhfl.html

================================================================================
来源：http://hz.smart0.xyz/gtyudqlzox.html

O. 并发与异步
来源：http://hz.sxryk.cn/gtrehbyslb.html

================================================================================
来源：http://hz.wangshuangyany.cn/gteclcbcra.html

[O01] 启动一个线程
来源：http://hz.nanxuanxn.top/gtkawuotql.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.shangyingyoupin.top/gtippttluj.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.zhijiandao.cn/gtuvfxfewi.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.fengsongda.top/gthdsxhmet.html

TS:   // 同 JS
来源：http://hz.yuxming.cn/gtcgllwxyh.html

Java: new Thread(() -> f()).start()
来源：http://hz.aizwys.cn/gtvasusdwm.html

Go:   go f()
来源：http://hz.hnqzz.top/gtzqyrwzob.html

Ruby: Thread.new { f }
来源：http://hz.yuxming.cn/gtwghwliys.html

C#:   Task.Run(() => F());
来源：http://hz.yangfankeji.com/gtmzfmianz.html

[O02] 使用线程池
来源：http://hz.nanxuanxn.top/gtmyzlgsvq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.gaohongyu789.top/gtrfxxthfz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.zhongyouzk.top/gtbmmzrikp.html

JS:   // worker_threads 线程池
来源：http://hz.sysykeji.top/gtdgxoihhh.html

TS:   // worker_threads 线程池
来源：http://hz.snrcjt.cn/gttaeboglb.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.hfpthk.cn/gtccxecmdw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.zhixingplan.top/gtgfgjvdqs.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.wangdashe.top/gtcavktunk.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.zhaomingkeji.xyz/gtsswbmhpu.html

[O03] 加锁保护共享数据
来源：http://hz.jqgufenzy.top/gtinujruqh.html

Py:   with lock: shared += 1
来源：http://hz.daxiang520.top/gtzoitftgc.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.havefunace.top/gtrdevllgk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.yanxiufei.cn/gtndqmvpex.html

TS:   // 同 JS
来源：http://hz.yj20258.top/gtjyamawos.html

Java: synchronized (this) { shared++; }
来源：http://hz.smart0.xyz/gtgvofmskm.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.xziqi.cn/gtiyrzcpjq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.yj20258888.top/gtkbpeumbf.html

C#:   lock (gate) { shared++; }
来源：http://hz.yanxiufei.cn/gttplmqvjm.html

[O04] 定义异步函数并等待
来源：http://hz.haohaochexian.top/gtkziuecbc.html

Py:   async def f():⏎    await g()
来源：http://hz.yueranfly.top/gtlrbsvjrk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.cqqwz.cn/gtasudxdpk.html

JS:   async function f() { await g(); }
来源：http://hz.zhengqikj.top/gtlxwtylxq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.shanyushiyangkeji.top/gtugbwaotg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.zhijiandao.cn/gtbawwvpmf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.zhaomingkeji.xyz/gtfygzbbfy.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.fzhhl.top/gtxocmenxj.html

C#:   async Task F() { await G(); }
来源：http://hz.hnqzz.top/gtbobxfwpm.html

[O05] 并发执行并等待全部完成
来源：http://hz.yanxiufei.cn/gtzmzespyo.html

Py:   asyncio.gather(*tasks)
来源：http://hz.birdmap.top/gtkqjduvqv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.xziqi.cn/gtgkmopugu.html

JS:   await Promise.all(tasks)
来源：http://hz.jyoumei.cn/gtuujenkno.html

TS:   await Promise.all(tasks)
来源：http://hz.cashguo.top/gtlbqlpfod.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.yanxiufei.cn/gttbhdtnyw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.redwolf501.top/gtovkscimm.html

Ruby: threads.map(&:join)
来源：http://hz.kuanghao11.cn/gtgxxygamr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.zycfv.cn/gtaywicini.html

[O06] 使用进程池
来源：http://hz.ybcxt.top/gtzsxkpavu.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.daria6918.cn/gtvpnzxqgw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.yuanzhike.top/gtnsdewrbw.html

JS:   // child_process / cluster 模块
来源：http://hz.gogol.net.cn/gtjtiqlepp.html

TS:   // child_process / cluster 模块
来源：http://hz.yj20258888.top/gtqupluqnr.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.quarkkingdee.top/gthecxfspw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.jinghuilouyu.cn/gtrmzjlcel.html

Ruby: // fork 块
来源：http://hz.vqdsnc.cn/gtqziacvqt.html

C#:   Parallel.For
来源：http://hz.jinyuanbaomall.cn/gtdirvyfra.html

================================================================================
来源：http://hz.sufxvd.cn/gtuakvomyd.html

P. 常用工具函数
来源：http://hz.sufxvd.cn/gtonfrisnf.html

================================================================================
来源：http://hz.hfpthk.cn/gtsduxxooy.html

[P01] 生成 UUID
来源：http://hz.daria6918.cn/gtijevmdbh.html

Py:   str(uuid.uuid4())
来源：http://hz.pycfn.com/gtjzypqdni.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yuanzhike.top/gtwyolztlt.html

JS:   crypto.randomUUID()
来源：http://hz.gaohongyu789.top/gtrlxdqvdx.html

TS:   crypto.randomUUID()
来源：http://hz.xingfuxueyuan.xyz/gttlwwopkq.html

Java: UUID.randomUUID().toString()
来源：http://hz.yj202588.top/gtvjlsmupe.html

Go:   // 用 github.com/google/uuid
来源：http://hz.cqqwz.cn/gtydapsuzf.html

Ruby: SecureRandom.uuid
来源：http://hz.pengpengdd.cyou/gttwussxmu.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.zhoulong.xyz/gttrgggylz.html

[P02] MD5 / SHA256 摘要
来源：http://hz.meibo888.top/gtluxcgako.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.shangyingyoupin.top/gtratnapsj.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.wangdashe.top/gtemgsoshv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.cdnleiting.top/gtjqdtbxhu.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.zhixingplan.top/gtqgovwvcx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.wangshuangyany.cn/gtxlvjvkmc.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.xziqi.cn/gtfkmmnjsp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.dianchejie.cn/gtbrqtonzh.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.smart0.xyz/gtlthomkvg.html

[P03] 生成短随机字符串
来源：http://hz.jqgfzy.top/gtbrfxtgmi.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.yongpay.top/gtiqqkvjua.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.yanxiufei.cn/gtoxzizmki.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jinqigfzy.top/gtmbudfbpu.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.52xcode.cn/gtruzkzagw.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.birdmap.top/gthokppqgd.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yj20258.top/gtirhhajgf.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.tian-w.cn/gtunnmwodg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.fengsongda.top/gtygxuzfjo.html

[P04] 求长度
来源：http://hz.chenlongwang.top/gtyhegulyf.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.ydjk.org.cn/gterrgqsuc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yuxming.cn/gttajbopmf.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.cqqwz.cn/gtfmfjbqso.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.meibo888.top/gtpbtqdxtw.html

Java: list.size();  map.size();  s.length()
来源：http://hz.xingfuxueyuan.xyz/gtqdgtomof.html

Go:   len(arr);  len(m)
来源：http://hz.cheryme.top/gtrzlzupen.html

Ruby: x.length;  x.size
来源：http://hz.hammf.cn/gtdgqetcwr.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.shanyushiyangtech.top/gtdfykualo.html

[P05] 判断两个对象内容是否相等
来源：http://hz.sufxvd.cn/gtzrdbrdnm.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.hammf.cn/gtbnwddbqa.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.daxiang520.top/gtyhbzprqw.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.kuanghao11.cn/gtjytvlecu.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.dianchejie.cn/gtwdsvmmgv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.andypj.xyz/gtvwxzypes.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.wangshuangyany.cn/gtgomgtfah.html

Ruby: a == b
来源：http://hz.jinghuilouyu.cn/gtqzbxjtwd.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.ybcxt.top/gtbfoqmahu.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.c1oappe.top/gteulvhuyx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.yj20258.top/gtbjwfpovw.html

PHP:  if (empty($x)) {}
来源：http://hz.shzxlz.cn/gtolwavvpc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jyoumei.cn/gtsomfthyo.html

TS:   if (x == null) {}
来源：http://hz.nwbrower.top/gtepygjaje.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.jinqigfzy.top/gtbhsdauel.html

Go:   if x == nil {}
来源：http://hz.zhoulong.xyz/gtjttbvpom.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.daria6918.cn/gttsceimvh.html

C#:   if (x is null) {}
来源：http://hz.xylfe.cn/gtkmohgdov.html

[P07] 防抖与节流
来源：http://hz.guowangkeji.top/gtdmxfrfnl.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jinqigufen.top/gtcwedcvet.html

PHP:  // 手写时间戳比较
来源：http://hz.jinyuanbaomall.cn/gtjgnvwjou.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.nanxinkj.top/gtmgzfgbdg.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.smart0.xyz/gtesefazus.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.fengsongda.top/gtptoyagwp.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.chenlongwang.top/gtfrpxfiaq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.wangdashe.top/gtofwnfaaq.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.shzxlz.cn/gttawkkbcr.html

[P08] 处理浮点精度问题
来源：http://hz.fzhhl.top/gtwzizfeem.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.meibo888.top/gtajwptksm.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.yj20258888.top/gtdtwjvklu.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.hongshengwenyu.top/gtcuyrmlhi.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.shanyushiyangtech.top/gthhdfqkmd.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.birdmap.top/gtazlncwcm.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.xuetiantiany.cn/gtmpafurea.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.zhoulong.xyz/gtfgzjypri.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.feifeiyinyue.top/gtrnofqwxa.html

================================================================================
来源：http://hz.yvedp.cn/gtqlvdpyzw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.wangdashe.top/gttxqjziam.html

================================================================================
来源：http://hz.guannengcc.top/gtprzkoebg.html

[Q01] 创建表
来源：http://hz.chenlongwang.top/gtfctnxyva.html

CREATE TABLE users (
来源：http://hz.jinqigufen.top/gtxkbmibue.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.tian-w.cn/gtexiqsgrp.html

name VARCHAR(50) NOT NULL,
来源：http://hz.hongshengwenyu.top/gtbanapvkm.html

email VARCHAR(100) UNIQUE,
来源：http://hz.shangyingyoupin.top/gtdpwtwosj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.wangdashe.top/gtlxonalak.html

);
来源：http://hz.jlsjyb.cn/gtyyznspau.html

[Q02] 创建带外键的表
来源：http://hz.dashuyun.cn/gtwjmbidze.html

CREATE TABLE orders (
来源：http://hz.0kj1m.cn/gthzqvkxwx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xingfuxueyuan.xyz/gthijqtcue.html

user_id INT NOT NULL,
来源：http://hz.meibo888.top/gtyzfhrfzh.html

amount DECIMAL(10, 2),
来源：http://hz.yvedp.cn/gtskuvbxmv.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.yvedp.cn/gtmrmghdhu.html

);
来源：http://hz.andypj.xyz/gtmnekxucl.html

[Q03] 增加列
来源：http://hz.tanke756.top/gtmebagswy.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.sweek.top/gtgudikmxm.html

[Q04] 修改列类型
来源：http://hz.yangfankeji.com/gtimypxaxt.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.hysaishi.cn/gtesfqecdi.html

[Q05] 重命名列
来源：http://hz.birdmap.top/gtluytieam.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.xuetiantiany.cn/gtuvelhdpo.html

[Q06] 删除列
来源：http://hz.guowangkeji.top/gtquqxcioy.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.wangdashe.top/gtgppsstfm.html

[Q07] 删除表
来源：http://hz.jinqigufen.top/gtemkcrava.html

DROP TABLE IF EXISTS orders;
来源：http://hz.cqqwz.cn/gtgiatyuky.html

[Q08] 创建普通索引
来源：http://hz.gzhubu.top/gtwqpcjzsj.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.xylfe.cn/gtzqjkorsj.html

[Q09] 创建唯一索引
来源：http://hz.9152youxi.cn/gtyurtvgue.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.cdnleiting.top/gtybryoyfu.html

[Q10] 插入单行
来源：http://hz.ywan-chungtsiang.top/gtjhngydbn.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.zdqjudy.top/gtlpnsyktt.html

[Q11] 一次插入多行
来源：http://hz.sufxvd.cn/gtspptbvry.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yongpay.top/gtvigjpksc.html

[Q12] 插入后取自增 ID
来源：http://hz.sysykeji.top/gtzajscfli.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.0kj1m.cn/gtkhxnjezw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.shzxlz.cn/gtrlowfoty.html

[Q13] 忽略重复插入
来源：http://hz.jqgufenzy.top/gtmbvnictt.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.yonumen.top/gtkmmipbcb.html

[Q14] 存在则更新（upsert）
来源：http://hz.quarkkingdee.top/gtyisghnyt.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.cashguo.top/gttdconezr.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.guowangkeji.top/gtdavpgoqn.html

[Q15] 查询全部
来源：http://hz.yj202588.top/gtzszbpvms.html

SELECT * FROM users;
来源：http://hz.chenzaomai.com/gtxtejceay.html

[Q16] 查询指定列
来源：http://hz.wangshuangyany.cn/gtppbnfsqs.html

SELECT id, name FROM users;
来源：http://hz.cheryme.top/gtvxwbcxpa.html

[Q17] 条件查询
来源：http://hz.zhengqikj.top/gtlxfnwwki.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.jinyuanbaomall.cn/gtsqhoivkl.html

[Q18] 模糊匹配
来源：http://hz.kuanghao11.cn/gtjnbaxxgi.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.nanxinkj.top/gtbuihnjlk.html

[Q19] 范围查询
来源：http://hz.vqdsnc.cn/gtrbvyhnla.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.andypj.xyz/gticpvcvkd.html

[Q20] IN 列表
来源：http://hz.kuanghao11.cn/gtmtqeylsp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.nwbrower.top/gtviixfixb.html

[Q21] 空值判断
来源：http://hz.jlsjyb.cn/gtdspzcfsz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.0kj1m.cn/gtqwdkalom.html

[Q22] 排序
来源：http://hz.ivvv.top/gtiohhtbvo.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.fengsongda.top/gtlkzdxonv.html

[Q23] 分页
来源：http://hz.snrcjt.cn/gtoixsucld.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yj202588.top/gtfcvqbfzl.html

[Q24] 去重
来源：http://hz.shangyingyoupin.top/gthkxdwdwi.html

SELECT DISTINCT city FROM users;
来源：http://hz.xziqi.cn/gtlubujkth.html

[Q25] 只取前 N 条
来源：http://hz.guannengcc.top/gthioaaqay.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.shanyushiyangkeji.top/gtsqfiahbh.html

[Q26] 计数
来源：http://hz.daria6918.cn/gtvulfonfi.html

SELECT COUNT(*) FROM users;
来源：http://hz.sxryk.cn/gtyuzqcwzv.html

[Q27] 条件计数
来源：http://hz.tanke756.top/gtltguzlfn.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.zdqjudy.top/gtbpvrwtmp.html

[Q28] 求和与平均
来源：http://hz.sxryk.cn/gtdaewensw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.jlsjyb.cn/gtotuccdmb.html

[Q29] 最大最小值
来源：http://hz.aibaodan.cn/gtplblzdqv.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.hywenlv.cn/gtqjmdsngf.html

[Q30] 分组统计
来源：http://hz.birdmap.top/gtwayqjuko.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.nanxinkj.top/gtbmkncvcn.html

[Q31] 分组后过滤
来源：http://hz.tianlin.xyz/gtfgrjutgy.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.xylfe.cn/gtzywcawgx.html

[Q32] 分组拼接字符串
来源：http://hz.hnxiangtu.top/gtylqvzaca.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.cheryme.top/gtnjeszpia.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.shanyushiyangkeji.top/gtgrvrvdoq.html

[Q33] 多列分组
来源：http://hz.zhongyouzk.top/gtsxxaqbgm.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.ivvv.top/gtkuccgxlk.html

[Q34] 每组取第一条
来源：http://hz.feifeiyinyue.top/gtaxgoiwal.html

SELECT * FROM (
来源：http://hz.yuxming.cn/gtphzwmkoq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.cqqwz.cn/gtnkfatosy.html

) t WHERE rn = 1;
来源：http://hz.dianchejie.cn/gtpzhymolr.html

[Q35] 内连接
来源：http://hz.andypj.xyz/gtjbubuimq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.jinqigfzy.top/gtyblkjboh.html

[Q36] 左连接
来源：http://hz.daria6918.cn/gtpebffsxh.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.guowangkeji.top/gtnkwwcsxp.html

[Q37] 右连接
来源：http://hz.fengsongda.top/gtejbktoda.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.wangshuangyany.cn/gtcxjrsvkf.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.sxryk.cn/gtafcomilh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.sysykeji.top/gtrlrxhmfz.html

[Q39] 自连接（查上下级）
来源：http://hz.sweek.top/gthuchjzeb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.yueranfly.top/gttfztqqlu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.zhengqikj.top/gtmirkcujs.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.ydzc1.top/gtfzyqwfzd.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.dianchejie.cn/gtvwqakzku.html

[Q41] 多表连接
来源：http://hz.zhaomingkeji.xyz/gtfuxpmcya.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.cheryme.top/gthuulzhao.html

JOIN users u ON u.id = o.user_id
来源：http://hz.andypj.xyz/gtamgwsrrh.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.cdnleiting.top/gtbvafecdp.html

[Q42] 连接条件附加过滤
来源：http://hz.wangshuangyany.cn/gturpjljcw.html

SELECT u.name, o.amount FROM users u
来源：http://hz.tianlin.xyz/gtsewidwqn.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.gotoacloud.top/gtnvohbqzx.html

[Q43] 标量子查询
来源：http://hz.ydjk.org.cn/gtdyetziqp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.ehwqpu.com/gtcedtwukh.html

[Q44] IN 子查询
来源：http://hz.chenlongwang.top/gtisomoazq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.shanyushiyangkeji.top/gtpjjllbde.html

[Q45] EXISTS 判断存在
来源：http://hz.daria6918.cn/gtolctrznh.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jianghu66.top/gtkjpfcfqv.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.ywan-chungtsiang.top/gtdrgrmlny.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yj20258.top/gtcnrwlumy.html

[Q47] 与平均值比较
来源：http://hz.haohaochexian.top/gtgzzgaloc.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.shzxlz.cn/gtuvpvoshx.html

[Q48] CTE 公用表表达式
来源：http://hz.zhengqikj.top/gtxibmjzkc.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.chenzaomai.com/gtzcxktlwv.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.jianghu66.top/gthkidofhj.html

[Q49] 更新单行
来源：http://hz.wangdashe.top/gteuavbirn.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yanxiufei.cn/gtnahtdzbw.html

[Q50] 批量更新
来源：http://hz.vqdsnc.cn/gttjfpiqyj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.sysykeji.top/gthuzuknme.html

[Q51] 用子查询更新
来源：http://hz.chenjidiqi.icu/gtjsmliyxc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.haohaochexian.top/gtbughequs.html

[Q52] 删除指定行
来源：http://hz.fengsongda.top/gtxbtzvevj.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yj20258888.top/gtgvswmnav.html

[Q53] 按条件删除
来源：http://hz.yonumen.top/gtrghzqeho.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.meibo888.top/gtkobjdiug.html

[Q54] 清空表
来源：http://hz.xuetiantiany.cn/gtekguuckb.html

TRUNCATE TABLE logs;
来源：http://hz.zhiwuduotai.top/gtdgntgeph.html

[Q55] 排名（并列占位）
来源：http://hz.52xcode.cn/gtpfwjwkcc.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yueranfly.top/gtlenzrwxj.html

[Q56] 密集排名（并列不占位）
来源：http://hz.0kj1m.cn/gtjeyonrvr.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yangfankeji.com/gtpajbwcir.html

[Q57] 行号
来源：http://hz.9152youxi.cn/gtytfhnlyn.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.shzxlz.cn/gttnszfnuj.html

[Q58] 累计求和
来源：http://hz.sxryk.cn/gtfmlklmgg.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.jlsjyb.cn/gtwdlfhivi.html

[Q59] 分组内累计
来源：http://hz.shanyushiyangtech.top/gtdhtnhxbm.html


<!-- 参考信息 -->