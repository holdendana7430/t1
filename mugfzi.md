代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.aibaodan.cn/gtcdkfcjto.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.hywenlv.cn/gtpcrxbrhh.html

Java: class Node { int v; Node next; }
来源：http://hz.yangfankeji.com/gtuzyolrde.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.xinyue.icu/gtdhophlam.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.mhx1999.top/gtylanfmys.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.jiagoushi.top/gtqgjvslne.html

[N11] 二叉树中序遍历
来源：http://hz.zhiwuduotai.top/gtadvfxrrb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.fengsongda.top/gtphovtbis.html

PHP:  // 手写递归函数
来源：http://hz.chenzaomai.com/gtomijquum.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jyoumei.cn/gtlwldwdjl.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.snrcjt.cn/gtezqafhip.html

Java: // 手写递归
来源：http://hz.sufxvd.cn/gtnvkusefn.html

Go:   // 手写递归
来源：http://hz.jyoumei.cn/gtgpoddfah.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.cdnleiting.top/gttstfpcin.html

C#:   // 手写递归
来源：http://hz.xuetiantiany.cn/gtqjkbwcuq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.gaohongyu789.top/gtsegrejna.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.wangdashe.top/gtsxdonnkx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.sxryk.cn/gtyvwdijbu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zycfv.cn/gttbtnwtbf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hongshengwenyu.top/gtqmgdmdhy.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.cheryme.top/gtvttudtwo.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.havefunace.top/gtpngigkln.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.jinqigfzy.top/gtmooohepe.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ybcxt.top/gtfwcgtqxv.html

================================================================================
来源：http://hz.hysaishi.cn/gtujqqhuwp.html

O. 并发与异步
来源：http://hz.ydzc1.top/gtyyvyrqto.html

================================================================================
来源：http://hz.yuanzhike.top/gtivcflefe.html

[O01] 启动一个线程
来源：http://hz.ehwqpu.com/gtyluzzirz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.zhaomingkeji.xyz/gtyapdwxbq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.cdnleiting.top/gtzptdqksh.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.mhx1999.top/gtbjofapba.html

TS:   // 同 JS
来源：http://hz.zhijiandao.cn/gtxtpepwlh.html

Java: new Thread(() -> f()).start()
来源：http://hz.dashuyun.cn/gtoxplkazj.html

Go:   go f()
来源：http://hz.hnxiangtu.top/gtoztyunzq.html

Ruby: Thread.new { f }
来源：http://hz.smart0.xyz/gtlqzycsxb.html

C#:   Task.Run(() => F());
来源：http://hz.xziqi.cn/gtdaktopow.html

[O02] 使用线程池
来源：http://hz.ydjk.org.cn/gtatvyajhw.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.jyoumei.cn/gthltobsyu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.nanxuanxn.top/gtxjrgdlxo.html

JS:   // worker_threads 线程池
来源：http://hz.zhijiandao.cn/gthfwatcjz.html

TS:   // worker_threads 线程池
来源：http://hz.sxryk.cn/gtyroxylpo.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.zdqjudy.top/gtdfvqclcr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.haohaochexian.top/gtfkpbtsyx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.andypj.xyz/gtnvanwwni.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.snrcjt.cn/gteexfbrtl.html

[O03] 加锁保护共享数据
来源：http://hz.shanyushiyangtech.top/gtmpijsxvl.html

Py:   with lock: shared += 1
来源：http://hz.feifeiyinyue.top/gtytllffkr.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.svipenyu.cn/gtjofpkhbw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.wangshuangyany.cn/gtsxackvpi.html

TS:   // 同 JS
来源：http://hz.pycfn.com/gtcsffpxgc.html

Java: synchronized (this) { shared++; }
来源：http://hz.cdnleiting.top/gtfndgrxxc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.hnxiangtu.top/gtwnluzqks.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.chenzaomai.com/gtfjtuzauf.html

C#:   lock (gate) { shared++; }
来源：http://hz.jianghu66.top/gtjknrxrdj.html

[O04] 定义异步函数并等待
来源：http://hz.jqgfzy.top/gttvdhuqyw.html

Py:   async def f():⏎    await g()
来源：http://hz.ydjk.org.cn/gtjxfvxkhv.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.hammf.cn/gtvglmowbe.html

JS:   async function f() { await g(); }
来源：http://hz.daxiang520.top/gtljtwoknf.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.hnqzz.top/gtbuiuzetr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.hnqzz.top/gtpfdwihsw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.andypj.xyz/gtuwzhmwyy.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.0kj1m.cn/gtvioqbzhp.html

C#:   async Task F() { await G(); }
来源：http://hz.feifeiyinyue.top/gtxkjjyuee.html

[O05] 并发执行并等待全部完成
来源：http://hz.birdmap.top/gtjnohvrzv.html

Py:   asyncio.gather(*tasks)
来源：http://hz.zhixingplan.top/gtuvdbgrgj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.sxryk.cn/gtwbokbukq.html

JS:   await Promise.all(tasks)
来源：http://hz.jiagoushi.top/gtowqowhhx.html

TS:   await Promise.all(tasks)
来源：http://hz.nwbrower.top/gtfbtbspyk.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.fzhhl.top/gtiqfqwikb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.haohaochexian.top/gtrzfjrjlw.html

Ruby: threads.map(&:join)
来源：http://hz.tanke756.top/gtjbpqsvfb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.iojbl.cn/gtrmryfays.html

[O06] 使用进程池
来源：http://hz.hnxiangtu.top/gtlatupvfx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.yangfankeji.com/gttpxwwcoy.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.0kj1m.cn/gtajflkczh.html

JS:   // child_process / cluster 模块
来源：http://hz.xinyue.icu/gtkeyusqsp.html

TS:   // child_process / cluster 模块
来源：http://hz.gogol.net.cn/gtbqdxbmor.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yonumen.top/gtqdfnfums.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.hysaishi.cn/gttqftxnnt.html

Ruby: // fork 块
来源：http://hz.cucudq.cn/gtbrtnumyx.html

C#:   Parallel.For
来源：http://hz.shanyushiyangkeji.top/gtgdeiyltg.html

================================================================================
来源：http://hz.smart0.xyz/gtzxnswoey.html

P. 常用工具函数
来源：http://hz.guannengcc.top/gtpvblpnnl.html

================================================================================
来源：http://hz.9152youxi.cn/gtiqtxwkph.html

[P01] 生成 UUID
来源：http://hz.hnxiangtu.top/gtkbmmimzh.html

Py:   str(uuid.uuid4())
来源：http://hz.pycfn.com/gteysupooz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.zhengqikj.top/gtelugxngs.html

JS:   crypto.randomUUID()
来源：http://hz.ydjk.org.cn/gtxhcawkpm.html

TS:   crypto.randomUUID()
来源：http://hz.yvedp.cn/gtqpmhlhcj.html

Java: UUID.randomUUID().toString()
来源：http://hz.yanxiufei.cn/gtuszywwhs.html

Go:   // 用 github.com/google/uuid
来源：http://hz.chenjidiqi.icu/gtvbtijsjz.html

Ruby: SecureRandom.uuid
来源：http://hz.dashuyun.cn/gtpoakavmb.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.smart0.xyz/gtorlqzcma.html

[P02] MD5 / SHA256 摘要
来源：http://hz.guowangkeji.top/gtnjejsmvw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.hfpthk.cn/gterwpxjus.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.wangdashe.top/gtsvgmghkv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.jyoumei.cn/gtkbqcrfhy.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.yj20258888.top/gtrezwomgs.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.tanke756.top/gtxnpkcwxe.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.shangyingyoupin.top/gtnmfgxxbc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.dashuyun.cn/gtmjfijkzs.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.c1oappe.top/gtjqmrlcaq.html

[P03] 生成短随机字符串
来源：http://hz.jqgfzy.top/gtamirrczy.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.hfpthk.cn/gtfeippzei.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.xingfuxueyuan.xyz/gtehhemmoo.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.gzhubu.top/gtphbmnkpz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.guannengcc.top/gtmcpzaopb.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yuxming.cn/gthcotrmyl.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.zhijiandao.cn/gtqfaagdai.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jinqigfzy.top/gtsnkuvimf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.hywenlv.cn/gtzicuixdm.html

[P04] 求长度
来源：http://hz.tanke756.top/gtbyramaio.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.jianghu66.top/gtqwamamfv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.pengpengdd.cyou/gtqfhkhoim.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yuxming.cn/gtgiptntkz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.fzhhl.top/gtwidlhvkw.html

Java: list.size();  map.size();  s.length()
来源：http://hz.chenlongwang.top/gtdivmvcgt.html

Go:   len(arr);  len(m)
来源：http://hz.xingfuxueyuan.xyz/gternyypre.html

Ruby: x.length;  x.size
来源：http://hz.fzhhl.top/gtnneiarqj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.ehwqpu.com/gtsiygdpgg.html

[P05] 判断两个对象内容是否相等
来源：http://hz.jiagoushi.top/gtzilkeoaa.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.xuetiantiany.cn/gtdyqysgxy.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.hysaishi.cn/gteoqxxbzm.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.jyoumei.cn/gtogwwionc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.smart0.xyz/gtgvypzvvg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.xingfuxueyuan.xyz/gtzoopxhsm.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.zhijiandao.cn/gtdqngtuoy.html

Ruby: a == b
来源：http://hz.nanxinkj.top/gtwljylbdd.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.hfpthk.cn/gtdisgwyzj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.zhijiandao.cn/gtmdyzndnb.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.guowangkeji.top/gtzfduwnod.html

PHP:  if (empty($x)) {}
来源：http://hz.daria6918.cn/gtjexzlutc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.316326.xyz/gtcnwvnkcu.html

TS:   if (x == null) {}
来源：http://hz.nanxinkj.top/gtqtvuqzaf.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.quarkkingdee.top/gtmgrtwmrf.html

Go:   if x == nil {}
来源：http://hz.ydjk.org.cn/gtzkiqslyp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.hammf.cn/gtrmydtjjr.html

C#:   if (x is null) {}
来源：http://hz.zhijiandao.cn/gtoehrfnmv.html

[P07] 防抖与节流
来源：http://hz.zhiwuduotai.top/gtnytkkyug.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.meibo888.top/gthqkiiyqi.html

PHP:  // 手写时间戳比较
来源：http://hz.pengpengdd.cyou/gtawmzxbom.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yj20258.top/gtahosslaf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.dianchejie.cn/gthbhbpund.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.fengsongda.top/gtxfrwhvbk.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.chenzaomai.com/gtntjpkuzo.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.hysaishi.cn/gtkhfwntnu.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.hnqzz.top/gtogzpbdmw.html

[P08] 处理浮点精度问题
来源：http://hz.hywenlv.cn/gtonikkygr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.haohaochexian.top/gtgmickley.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.jiagoushi.top/gtiewtqgoa.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.fengsongda.top/gtsuapzsln.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.vqdsnc.cn/gtfuddqwrz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.aizwys.cn/gtagrpqkiw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.tianlin.xyz/gteauqerub.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.hammf.cn/gtatecnslp.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.daxiang520.top/gtwhmndlhd.html

================================================================================
来源：http://hz.nwbrower.top/gtzxzzhohc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.zhengqikj.top/gtvhjixyyb.html

================================================================================
来源：http://hz.daria6918.cn/gtypofzykb.html

[Q01] 创建表
来源：http://hz.hysaishi.cn/gtnjrnlfvc.html

CREATE TABLE users (
来源：http://hz.zycfv.cn/gtazmvabda.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhixingplan.top/gtfovtdiiq.html

name VARCHAR(50) NOT NULL,
来源：http://hz.xuetiantiany.cn/gtoweclytd.html

email VARCHAR(100) UNIQUE,
来源：http://hz.shanyushiyangtech.top/gtjhcqekko.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.zhoulong.xyz/gtwhpfbkaq.html

);
来源：http://hz.jinqigfzy.top/gtrzzphfst.html

[Q02] 创建带外键的表
来源：http://hz.zhoulong.xyz/gtcjzvngio.html

CREATE TABLE orders (
来源：http://hz.yongpay.top/gtivxoyllj.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.svipenyu.cn/gtsmhdxqjb.html

user_id INT NOT NULL,
来源：http://hz.pengpengdd.cyou/gtmtcobtmy.html

amount DECIMAL(10, 2),
来源：http://hz.0kj1m.cn/gtxphyqinb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.chenzaomai.com/gtvbdfcqbw.html

);
来源：http://hz.sxryk.cn/gtqbsbvyae.html

[Q03] 增加列
来源：http://hz.ybcxt.top/gtbetehnzs.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.aibaodan.cn/gtnikscpun.html

[Q04] 修改列类型
来源：http://hz.jlsjyb.cn/gtshrcgbpt.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.hnxiangtu.top/gtczerkewb.html

[Q05] 重命名列
来源：http://hz.aizwys.cn/gtfbctuxze.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.yj20258.top/gtrfnkutbv.html

[Q06] 删除列
来源：http://hz.fzhhl.top/gtpegiurpz.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.dashuyun.cn/gtjckaogno.html

[Q07] 删除表
来源：http://hz.yueranfly.top/gtxbzeqsqc.html

DROP TABLE IF EXISTS orders;
来源：http://hz.yj202588.top/gtaavgytmi.html

[Q08] 创建普通索引
来源：http://hz.ywan-chungtsiang.top/gtwyqoanes.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jinghuilouyu.cn/gtnvmupags.html

[Q09] 创建唯一索引
来源：http://hz.kuanghao11.cn/gthpgrpncp.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.yuanzhike.top/gtyjdxymmq.html

[Q10] 插入单行
来源：http://hz.52xcode.cn/gtzgqlzdkl.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.hysaishi.cn/gtbtlzvvaz.html

[Q11] 一次插入多行
来源：http://hz.mhx1999.top/gtosnjjoiq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.haohaochexian.top/gtaojtowev.html

[Q12] 插入后取自增 ID
来源：http://hz.kuanghao11.cn/gtwwxrkmjm.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.sufxvd.cn/gtblgstqgf.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.jlsjyb.cn/gtnvhhhqvz.html

[Q13] 忽略重复插入
来源：http://hz.yangfankeji.com/gttondzjle.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.zhengqikj.top/gtmvepqztx.html

[Q14] 存在则更新（upsert）
来源：http://hz.aibaodan.cn/gtuahgzopn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.c1oappe.top/gtlcflmhfj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.xuanzx.com/gtmebpqkjo.html

[Q15] 查询全部
来源：http://hz.ehwqpu.com/gtiptcjnta.html

SELECT * FROM users;
来源：http://hz.cheryme.top/gtouufaees.html

[Q16] 查询指定列
来源：http://hz.jinghuilouyu.cn/gtlvlzyqju.html

SELECT id, name FROM users;
来源：http://hz.shanyushiyangkeji.top/gtvivuuakq.html

[Q17] 条件查询
来源：http://hz.xingfuxueyuan.xyz/gteirudecp.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.zhoulong.xyz/gtjqgektce.html

[Q18] 模糊匹配
来源：http://hz.jinqigufen.top/gtqrjpinnm.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.tanke756.top/gtobmaeuob.html

[Q19] 范围查询
来源：http://hz.xingfuxueyuan.xyz/gtujpplaft.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.shanyushiyangtech.top/gtvjtjimih.html

[Q20] IN 列表
来源：http://hz.zhoulong.xyz/gtzuipapyb.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.chenlongwang.top/gtjqgijrjm.html

[Q21] 空值判断
来源：http://hz.yj20258888.top/gtvkwzolgu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.dashuyun.cn/gtufodwdlt.html

[Q22] 排序
来源：http://hz.gzhubu.top/gtguxpfuac.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.hysaishi.cn/gtcuzynvim.html

[Q23] 分页
来源：http://hz.9152youxi.cn/gtajmgaspj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.hfpthk.cn/gtqtbnotqw.html

[Q24] 去重
来源：http://hz.yonumen.top/gtloujeieh.html

SELECT DISTINCT city FROM users;
来源：http://hz.yj20258888.top/gtxskxxhqc.html

[Q25] 只取前 N 条
来源：http://hz.zhongyouzk.top/gtqmdakven.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.yuanzhike.top/gtezdilaoy.html

[Q26] 计数
来源：http://hz.aibaodan.cn/gtnwzszidu.html

SELECT COUNT(*) FROM users;
来源：http://hz.jyoumei.cn/gtfihmemaq.html

[Q27] 条件计数
来源：http://hz.yuxming.cn/gtjaxqnzxm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.gogol.net.cn/gtmqsgvcbm.html

[Q28] 求和与平均
来源：http://hz.hnqzz.top/gtmmbrcbvp.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.iojbl.cn/gtutbkxndp.html

[Q29] 最大最小值
来源：http://hz.dashuyun.cn/gtqpcgikln.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.zhixingplan.top/gtukgynbyx.html

[Q30] 分组统计
来源：http://hz.yueranfly.top/gtoernokhc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.dianchejie.cn/gtcgfkdtko.html

[Q31] 分组后过滤
来源：http://hz.aizwys.cn/gtxcfiikrt.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.guannengcc.top/gtknjzxois.html

[Q32] 分组拼接字符串
来源：http://hz.pycfn.com/gttjdscipr.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.wangdashe.top/gtztvwvrrj.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.jinghuilouyu.cn/gtfnwrbwxy.html

[Q33] 多列分组
来源：http://hz.jianghu66.top/gtymavebzx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yuxming.cn/gtixjsfmly.html

[Q34] 每组取第一条
来源：http://hz.quarkkingdee.top/gtnoyrowhd.html

SELECT * FROM (
来源：http://hz.jinqigufen.top/gtlcsvplwf.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.sysykeji.top/gtgrauiqjl.html

) t WHERE rn = 1;
来源：http://hz.gaohongyu789.top/gttldrieab.html

[Q35] 内连接
来源：http://hz.jianghu66.top/gttvpmswnr.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.shuidangran.top/gtwcrgvnvo.html

[Q36] 左连接
来源：http://hz.smart0.xyz/gtcsfztjtl.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.hysaishi.cn/gtwtzxhoug.html

[Q37] 右连接
来源：http://hz.smart0.xyz/gtazjzyagi.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.0kj1m.cn/gtfvqdwvzj.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.hnqzz.top/gthptbgcav.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.yuxming.cn/gtbmihtxfy.html

[Q39] 自连接（查上下级）
来源：http://hz.dashuyun.cn/gtxwixowwd.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.meibo888.top/gtcdwtpihp.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yj20258.top/gtquhoezpx.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.daxiang520.top/gtzvqoxfrt.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.hongshengwenyu.top/gtpjvadijk.html

[Q41] 多表连接
来源：http://hz.tianlin.xyz/gtsatjffzu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.daxiang520.top/gtjumrwups.html

JOIN users u ON u.id = o.user_id
来源：http://hz.sweek.top/gtathoagvl.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.zhengqikj.top/gtzbjbryte.html

[Q42] 连接条件附加过滤
来源：http://hz.fengsongda.top/gtpmecevku.html

SELECT u.name, o.amount FROM users u
来源：http://hz.mhx1999.top/gtceptymji.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.gotoacloud.top/gtvsjcnlay.html

[Q43] 标量子查询
来源：http://hz.zhongyouzk.top/gtbvmesgcj.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.gotoacloud.top/gtpavdbdok.html

[Q44] IN 子查询
来源：http://hz.jinghuilouyu.cn/gtvpxkmxvq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.hfpthk.cn/gtskybqdxb.html

[Q45] EXISTS 判断存在
来源：http://hz.xinyue.icu/gtjbinhaye.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.shzxlz.cn/gtxmqbhmcr.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.sweek.top/gtkzbykjdo.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.9152youxi.cn/gttblmolex.html

[Q47] 与平均值比较
来源：http://hz.9152youxi.cn/gtlxhacmxf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.hysaishi.cn/gtawhimfao.html

[Q48] CTE 公用表表达式
来源：http://hz.meibo888.top/gtrzpqjnhh.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.hammf.cn/gtjkyoivjw.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.yangfankeji.com/gtupblkkrl.html

[Q49] 更新单行
来源：http://hz.316326.xyz/gtiewrmwtn.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.daxiang520.top/gtwmdufkib.html

[Q50] 批量更新
来源：http://hz.zhengqikj.top/gtzvuevnsz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.jqgufenzy.top/gtzpynvbtw.html

[Q51] 用子查询更新
来源：http://hz.fzhhl.top/gtpdrsgoyr.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.jlsjyb.cn/gtirjlsybq.html

[Q52] 删除指定行
来源：http://hz.yvedp.cn/gtucsxuhga.html

DELETE FROM users WHERE id = 10;
来源：http://hz.zhaomingkeji.xyz/gtlllhyaej.html

[Q53] 按条件删除
来源：http://hz.jinyuanbaomall.cn/gtitnydwyw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.316326.xyz/gtymmcuwxw.html

[Q54] 清空表
来源：http://hz.yuanzhike.top/gtnpirhjkx.html

TRUNCATE TABLE logs;
来源：http://hz.cqqwz.cn/gtcsdjruhg.html

[Q55] 排名（并列占位）
来源：http://hz.xziqi.cn/gtstiawont.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.dashuyun.cn/gtydciimrl.html

[Q56] 密集排名（并列不占位）
来源：http://hz.ydjk.org.cn/gtxecleiqy.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.chenlongwang.top/gtvvdzsaxr.html

[Q57] 行号
来源：http://hz.yueranfly.top/gtntncjypq.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.hysaishi.cn/gthohshteh.html

[Q58] 累计求和
来源：http://hz.sweek.top/gtbvxisaxb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yongpay.top/gtgxpiuuhw.html

[Q59] 分组内累计
来源：http://hz.aibaodan.cn/gtvjewdzbg.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.zhongyouzk.top/gtshoxftjo.html

[Q60] 取上一行 / 下一行
来源：http://hz.hfpthk.cn/gtedhvrvms.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.yuanzhike.top/gtbnzbtmgg.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.hnqzz.top/gtnqnucmui.html


<!-- 参考信息 -->