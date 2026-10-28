代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.jinghuilouyu.cn/gtbpoubsso.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.nwbrower.top/gttdeuzmfw.html

Java: class Node { int v; Node next; }
来源：http://hz.gogol.net.cn/gtlbrjtvxy.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.gzhubu.top/gtzitpzscu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.zdqjudy.top/gthcdfkmnz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.snrcjt.cn/gtpwawcoin.html

[N11] 二叉树中序遍历
来源：http://hz.xinyue.icu/gtbmhfatig.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.yongpay.top/gtxgzymatl.html

PHP:  // 手写递归函数
来源：http://hz.zhoulong.xyz/gtxiorkrtn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jinqigufen.top/gtafpphzpx.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.shanyushiyangtech.top/gtctvwtnkq.html

Java: // 手写递归
来源：http://hz.xziqi.cn/gtgsqdeiyq.html

Go:   // 手写递归
来源：http://hz.pengpengdd.cyou/gtgevqfrmt.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.ivvv.top/gtdzmbyjnf.html

C#:   // 手写递归
来源：http://hz.xylfe.cn/gtmyerhguk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.zhiwuduotai.top/gtjdtfpgdv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.kuanghao11.cn/gtnozjrkpf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.xziqi.cn/gtvmnwechg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xylfe.cn/gtyzgprgrs.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ydzc1.top/gttglgkhzb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.nwbrower.top/gtvsjleoxe.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.shanyushiyangtech.top/gtzkvouukr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.cdnleiting.top/gtvpusolrq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jyoumei.cn/gtdjxpyyin.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtoszuvtrw.html

O. 并发与异步
来源：http://hz.snrcjt.cn/gtllesdxyr.html

================================================================================
来源：http://hz.ehwqpu.com/gtthcououq.html

[O01] 启动一个线程
来源：http://hz.zhoulong.xyz/gtpddtgcax.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.wangshuangyany.cn/gtkdmgpxmt.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yuanzhike.top/gtdwejzoyq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.mhx1999.top/gtcrgwfisk.html

TS:   // 同 JS
来源：http://hz.yonumen.top/gtgdunxmdm.html

Java: new Thread(() -> f()).start()
来源：http://hz.0kj1m.cn/gtkzdgqopx.html

Go:   go f()
来源：http://hz.yvedp.cn/gtzrxfywzx.html

Ruby: Thread.new { f }
来源：http://hz.zhiwuduotai.top/gtuwzjicgg.html

C#:   Task.Run(() => F());
来源：http://hz.tanke756.top/gtvaegsmgq.html

[O02] 使用线程池
来源：http://hz.vqdsnc.cn/gtcijqlksi.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yuxming.cn/gtknpyzebz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.sufxvd.cn/gtftxghbcw.html

JS:   // worker_threads 线程池
来源：http://hz.birdmap.top/gthmyzcjob.html

TS:   // worker_threads 线程池
来源：http://hz.gaohongyu789.top/gtxhpwpfck.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.sxryk.cn/gtndwhjdun.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.daria6918.cn/gthdnmisyo.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.iojbl.cn/gtdqzaarjn.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.cheryme.top/gttpmgnixa.html

[O03] 加锁保护共享数据
来源：http://hz.zycfv.cn/gttbwwzlvr.html

Py:   with lock: shared += 1
来源：http://hz.yj202588.top/gtsqjpvmzl.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.wangshuangyany.cn/gtkdivxmhd.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.yangfankeji.com/gtmynbsyho.html

TS:   // 同 JS
来源：http://hz.jqgfzy.top/gthzpkxpre.html

Java: synchronized (this) { shared++; }
来源：http://hz.vqdsnc.cn/gtdekeyvve.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.gzhubu.top/gtlyjhueke.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.hywenlv.cn/gtrlsvahtq.html

C#:   lock (gate) { shared++; }
来源：http://hz.sysykeji.top/gtwhmtwvkd.html

[O04] 定义异步函数并等待
来源：http://hz.hfpthk.cn/gthcrvvoqv.html

Py:   async def f():⏎    await g()
来源：http://hz.daria6918.cn/gteomisbbn.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.wangdashe.top/gtpoahlvoy.html

JS:   async function f() { await g(); }
来源：http://hz.dashuyun.cn/gtwfxajhwz.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.shzxlz.cn/gtcyznxzqk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.wangshuangyany.cn/gtkdhasfez.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.shuidangran.top/gtipawedwc.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.bjfxy.top/gtgxscaaos.html

C#:   async Task F() { await G(); }
来源：http://hz.aizwys.cn/gtqagqqkgy.html

[O05] 并发执行并等待全部完成
来源：http://hz.ivvv.top/gtbqwakrnf.html

Py:   asyncio.gather(*tasks)
来源：http://hz.redwolf501.top/gtfxfkxwmc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.gzhubu.top/gtcnqikiqa.html

JS:   await Promise.all(tasks)
来源：http://hz.meibo888.top/gtstvjglqn.html

TS:   await Promise.all(tasks)
来源：http://hz.gotoacloud.top/gthkbxyacd.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.c1oappe.top/gtdxjyfggq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.xziqi.cn/gteaomodsk.html

Ruby: threads.map(&:join)
来源：http://hz.jlsjyb.cn/gthzzzwvkw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.zhengqikj.top/gtriscviwd.html

[O06] 使用进程池
来源：http://hz.yongpay.top/gtlxfdtfuz.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.nwbrower.top/gtptetewym.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.cashguo.top/gtvyqewzly.html

JS:   // child_process / cluster 模块
来源：http://hz.daxiang520.top/gtrchumsdx.html

TS:   // child_process / cluster 模块
来源：http://hz.feifeiyinyue.top/gtbvodmhig.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.cheryme.top/gtxqnsdylo.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.nanxuanxn.top/gtsvvpqxjx.html

Ruby: // fork 块
来源：http://hz.daxiang520.top/gtkubmpakp.html

C#:   Parallel.For
来源：http://hz.kuanghao11.cn/gtobzgsbtj.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtiwuldqwf.html

P. 常用工具函数
来源：http://hz.yangfankeji.com/gtazvwkzof.html

================================================================================
来源：http://hz.zhengqikj.top/gtefrkghzc.html

[P01] 生成 UUID
来源：http://hz.zhaomingkeji.xyz/gtvxhelnoi.html

Py:   str(uuid.uuid4())
来源：http://hz.jinqigufen.top/gtlcfrpjix.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.shanyushiyangkeji.top/gtozlkkylw.html

JS:   crypto.randomUUID()
来源：http://hz.dashuyun.cn/gtuprcksnr.html

TS:   crypto.randomUUID()
来源：http://hz.jiagoushi.top/gtvafbptat.html

Java: UUID.randomUUID().toString()
来源：http://hz.xziqi.cn/gtgpzcllvk.html

Go:   // 用 github.com/google/uuid
来源：http://hz.daxiang520.top/gtlgnjsqot.html

Ruby: SecureRandom.uuid
来源：http://hz.wangshuangyany.cn/gtfmsktawt.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.ydjk.org.cn/gtpwowihaj.html

[P02] MD5 / SHA256 摘要
来源：http://hz.feifeiyinyue.top/gtcjhexyjb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.vqdsnc.cn/gtdljnflbj.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.jiagoushi.top/gthewmqqze.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.wangdashe.top/gtqfsbyluu.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jianghu66.top/gtzazxsnow.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.iojbl.cn/gtswgrvrwg.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.jinghuilouyu.cn/gtvvnskppi.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.chenlongwang.top/gtmksnswxr.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.gaohongyu789.top/gtknljljmx.html

[P03] 生成短随机字符串
来源：http://hz.haohaochexian.top/gtwhtvytoz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.cdnleiting.top/gtyfrtlafo.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.zdqjudy.top/gtsuhcocxv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hfpthk.cn/gtxjlxpzuo.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jinghuilouyu.cn/gtuiadbhfo.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.tian-w.cn/gtkyndvzvb.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.0kj1m.cn/gtjrywzusx.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.ppjwa.cn/gtnyrxorhe.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.quarkkingdee.top/gtcrlfylua.html

[P04] 求长度
来源：http://hz.xingfuxueyuan.xyz/gtqliwdikp.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.zhoulong.xyz/gtroxxcdnu.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.guannengcc.top/gtvbltblwq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.cucudq.cn/gtparrafng.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.redwolf501.top/gtyzsdputp.html

Java: list.size();  map.size();  s.length()
来源：http://hz.snrcjt.cn/gtglklvfpd.html

Go:   len(arr);  len(m)
来源：http://hz.cqqwz.cn/gtfzlrxnyj.html

Ruby: x.length;  x.size
来源：http://hz.shanyushiyangtech.top/gtxlhusfog.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.pengpengdd.cyou/gtyhxqutul.html

[P05] 判断两个对象内容是否相等
来源：http://hz.zycfv.cn/gtgyttfwro.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.feifeiyinyue.top/gtwkpfchgx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.xuetiantiany.cn/gtcfpyvakk.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.svipenyu.cn/gtlpzshdud.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.quarkkingdee.top/gthukakgqe.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.cheryme.top/gtexfdzrfm.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.tianlin.xyz/gtqrwxvwzp.html

Ruby: a == b
来源：http://hz.hysaishi.cn/gtrwvqgyby.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.shuidangran.top/gtpeipvxwc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.shuidangran.top/gtnvjtlvoz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.xuanzx.com/gtidzkyzqr.html

PHP:  if (empty($x)) {}
来源：http://hz.iojbl.cn/gtbbzyesvo.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.hysaishi.cn/gtshthaheh.html

TS:   if (x == null) {}
来源：http://hz.gogol.net.cn/gtobzoednw.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.tanke756.top/gtniizlxpe.html

Go:   if x == nil {}
来源：http://hz.shanyushiyangkeji.top/gtgiyzsgrk.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.bjfxy.top/gtgkpimiru.html

C#:   if (x is null) {}
来源：http://hz.pycfn.com/gtuesmkxkd.html

[P07] 防抖与节流
来源：http://hz.guowangkeji.top/gtwathzoma.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jiagoushi.top/gtrtdnfsgk.html

PHP:  // 手写时间戳比较
来源：http://hz.hammf.cn/gtfxzgohsg.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.dianchejie.cn/gtivdwhgzv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.52xcode.cn/gtjgsuhqxz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.aizwys.cn/gtonxumchb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.feifeiyinyue.top/gtilqcutps.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.hysaishi.cn/gthawmkcdp.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.fzhhl.top/gtrnzfxbsm.html

[P08] 处理浮点精度问题
来源：http://hz.chenlongwang.top/gtiycwidtl.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.sweek.top/gttzagbbgu.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.aizwys.cn/gtricxnfof.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.tianlin.xyz/gtxippgxrm.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.hnqzz.top/gtszxnxjvr.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.pycfn.com/gtudbcbxlm.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.ehwqpu.com/gtnsjwcprd.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.yuxming.cn/gtpmvoruwe.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.shzxlz.cn/gtclzjfgrg.html

================================================================================
来源：http://hz.yj20258888.top/gtrrdsspyb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.mhx1999.top/gttbylvozg.html

================================================================================
来源：http://hz.dianchejie.cn/gteporftsl.html

[Q01] 创建表
来源：http://hz.vqdsnc.cn/gtgqguiczl.html

CREATE TABLE users (
来源：http://hz.hysaishi.cn/gtggecpmdf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.wangdashe.top/gtdmvtmkqm.html

name VARCHAR(50) NOT NULL,
来源：http://hz.zhongyouzk.top/gtzeldizxi.html

email VARCHAR(100) UNIQUE,
来源：http://hz.yangfankeji.com/gtwvdlnmhs.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.haohaochexian.top/gthdzdwodl.html

);
来源：http://hz.vqdsnc.cn/gtjnmjwzuv.html

[Q02] 创建带外键的表
来源：http://hz.tianlin.xyz/gthxupbdch.html

CREATE TABLE orders (
来源：http://hz.quarkkingdee.top/gttshitxtt.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.cucudq.cn/gtukotfjpj.html

user_id INT NOT NULL,
来源：http://hz.quarkkingdee.top/gtsgfojiih.html

amount DECIMAL(10, 2),
来源：http://hz.pengpengdd.cyou/gtzeynstlb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.kuanghao11.cn/gtoswwnzfi.html

);
来源：http://hz.yangfankeji.com/gtqmewmofr.html

[Q03] 增加列
来源：http://hz.yuxming.cn/gtrcezukvp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.sufxvd.cn/gtfjfuxnod.html

[Q04] 修改列类型
来源：http://hz.hysaishi.cn/gtiaqkukrm.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.c1oappe.top/gtqncfqhiw.html

[Q05] 重命名列
来源：http://hz.yuanzhike.top/gtejulosnw.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.cashguo.top/gtmywxolqy.html

[Q06] 删除列
来源：http://hz.zhengqikj.top/gtdtcbauao.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.redwolf501.top/gtsdoslqaf.html

[Q07] 删除表
来源：http://hz.yanxiufei.cn/gtokcqbkvr.html

DROP TABLE IF EXISTS orders;
来源：http://hz.wangdashe.top/gtyfnvnioa.html

[Q08] 创建普通索引
来源：http://hz.xuanzx.com/gtcxgmuzza.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.zhongyouzk.top/gtdyiuzise.html

[Q09] 创建唯一索引
来源：http://hz.hongshengwenyu.top/gtnntealws.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.cheryme.top/gtffqywdiz.html

[Q10] 插入单行
来源：http://hz.redwolf501.top/gtdejooetw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.ydjk.org.cn/gtnmywzsok.html

[Q11] 一次插入多行
来源：http://hz.hywenlv.cn/gtceapszbv.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.quarkkingdee.top/gtrppfrfiy.html

[Q12] 插入后取自增 ID
来源：http://hz.shuidangran.top/gtcjdjygvw.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.xuanzx.com/gtmmvkyvuo.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.shangyingyoupin.top/gtinhfhhva.html

[Q13] 忽略重复插入
来源：http://hz.cdnleiting.top/gtjtutedkt.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.gzhubu.top/gthkdlwfdl.html

[Q14] 存在则更新（upsert）
来源：http://hz.shanyushiyangtech.top/gtxhaawmpk.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.wangdashe.top/gtbpesfoxg.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.daxiang520.top/gtcrhcspbe.html

[Q15] 查询全部
来源：http://hz.yueranfly.top/gtgkrdfqjq.html

SELECT * FROM users;
来源：http://hz.jlsjyb.cn/gtzuaczjmn.html

[Q16] 查询指定列
来源：http://hz.quarkkingdee.top/gtanhbfcqg.html

SELECT id, name FROM users;
来源：http://hz.chenjidiqi.icu/gtryinmlkr.html

[Q17] 条件查询
来源：http://hz.ybcxt.top/gtkallnspm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.dianchejie.cn/gtikernqzc.html

[Q18] 模糊匹配
来源：http://hz.ybcxt.top/gtmpudjqtp.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.iojbl.cn/gthdixbyjx.html

[Q19] 范围查询
来源：http://hz.wangshuangyany.cn/gteqrrtmot.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.gzhubu.top/gtoekwqhiw.html

[Q20] IN 列表
来源：http://hz.hammf.cn/gthlpbejkn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.dianchejie.cn/gtzejyopdg.html

[Q21] 空值判断
来源：http://hz.birdmap.top/gthlboblio.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.birdmap.top/gtxwfusxgd.html

[Q22] 排序
来源：http://hz.yongpay.top/gtniwwenam.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.birdmap.top/gtsjaueaqp.html

[Q23] 分页
来源：http://hz.wangdashe.top/gtvydbcqsz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.jyoumei.cn/gttpjfhqel.html

[Q24] 去重
来源：http://hz.xziqi.cn/gtbntcrsrn.html

SELECT DISTINCT city FROM users;
来源：http://hz.ehwqpu.com/gtpztbmbmi.html

[Q25] 只取前 N 条
来源：http://hz.havefunace.top/gtjqsnlvpy.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.shangyingyoupin.top/gtrjxrgsqz.html

[Q26] 计数
来源：http://hz.zhiwuduotai.top/gtrdbfscue.html

SELECT COUNT(*) FROM users;
来源：http://hz.yongpay.top/gtwgbefqmv.html

[Q27] 条件计数
来源：http://hz.yongpay.top/gtezwmbqfv.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.smart0.xyz/gtiuqabnky.html

[Q28] 求和与平均
来源：http://hz.yvedp.cn/gtyjiinrwl.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.tian-w.cn/gtdtureexw.html

[Q29] 最大最小值
来源：http://hz.gotoacloud.top/gtktreqbmw.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.sysykeji.top/gtkadftsus.html

[Q30] 分组统计
来源：http://hz.cashguo.top/gtuzeljdtv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.haohaochexian.top/gtpfzzqtuu.html

[Q31] 分组后过滤
来源：http://hz.zhixingplan.top/gtltxfymxm.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.nanxinkj.top/gtfvpewdpq.html

[Q32] 分组拼接字符串
来源：http://hz.chenzaomai.com/gtnawqansp.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.zhixingplan.top/gtlklmejzr.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.dashuyun.cn/gtsaobpxii.html

[Q33] 多列分组
来源：http://hz.yj20258888.top/gtgqdknsry.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.dashuyun.cn/gtardrmbvz.html

[Q34] 每组取第一条
来源：http://hz.yuanzhike.top/gtcpfadzap.html

SELECT * FROM (
来源：http://hz.jinqigufen.top/gtjttqczxr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jinghuilouyu.cn/gtgztdolbb.html

) t WHERE rn = 1;
来源：http://hz.316326.xyz/gtznzwmhlx.html

[Q35] 内连接
来源：http://hz.jianghu66.top/gtdadfblll.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.nanxuanxn.top/gtcoqgbdxb.html

[Q36] 左连接
来源：http://hz.0kj1m.cn/gtfpdpedck.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.yuxming.cn/gtuavyeokh.html

[Q37] 右连接
来源：http://hz.pengpengdd.cyou/gtbdwcxvyf.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.ywan-chungtsiang.top/gttvucjdvs.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.shanyushiyangkeji.top/gtigwptttt.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.gaohongyu789.top/gttrgyyusy.html

[Q39] 自连接（查上下级）
来源：http://hz.zhoulong.xyz/gtrzimjfoi.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.shanyushiyangtech.top/gtsftaefxg.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.chenjidiqi.icu/gtdrqxrzae.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.zhiwuduotai.top/gtlwdlktcc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.shzxlz.cn/gtatblzsrx.html

[Q41] 多表连接
来源：http://hz.c1oappe.top/gtapjtnfjn.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.hnqzz.top/gtakocnkzh.html

JOIN users u ON u.id = o.user_id
来源：http://hz.zhijiandao.cn/gtasbzufrq.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.jqgufenzy.top/gtfojhxkvj.html

[Q42] 连接条件附加过滤
来源：http://hz.feifeiyinyue.top/gtymmlftyi.html

SELECT u.name, o.amount FROM users u
来源：http://hz.dianchejie.cn/gtyprozvvz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.hongshengwenyu.top/gtlampirhj.html

[Q43] 标量子查询
来源：http://hz.svipenyu.cn/gtxbjbdmdf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.andypj.xyz/gtenqxpsuo.html

[Q44] IN 子查询
来源：http://hz.kuanghao11.cn/gtytesdgal.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.hnqzz.top/gtmldfykoh.html

[Q45] EXISTS 判断存在
来源：http://hz.sweek.top/gtorchxqdm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yj202588.top/gtysjcwfjd.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.zycfv.cn/gtntmvihjs.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.snrcjt.cn/gthsexkmln.html

[Q47] 与平均值比较
来源：http://hz.iojbl.cn/gtadqafkiv.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.nanxinkj.top/gtxaxarxvz.html

[Q48] CTE 公用表表达式
来源：http://hz.316326.xyz/gtenugznqp.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.52xcode.cn/gtocldbbge.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.jianghu66.top/gtldkqhnrr.html

[Q49] 更新单行
来源：http://hz.hnqzz.top/gtbksgjsbd.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.hywenlv.cn/gtwdhttqdi.html

[Q50] 批量更新
来源：http://hz.pengpengdd.cyou/gthnxbaxom.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.cheryme.top/gtbsyrxdwp.html

[Q51] 用子查询更新
来源：http://hz.nanxinkj.top/gtefrumxvx.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.feifeiyinyue.top/gtqlnxtcwx.html

[Q52] 删除指定行
来源：http://hz.havefunace.top/gtswupvyag.html

DELETE FROM users WHERE id = 10;
来源：http://hz.havefunace.top/gtmczwtzfi.html

[Q53] 按条件删除
来源：http://hz.hnqzz.top/gtdflcdvib.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yuxming.cn/gtfbagnkip.html

[Q54] 清空表
来源：http://hz.gogol.net.cn/gtqflivofp.html

TRUNCATE TABLE logs;
来源：http://hz.jqgfzy.top/gtuancfehk.html

[Q55] 排名（并列占位）
来源：http://hz.ehwqpu.com/gtgyfxmozo.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.feifeiyinyue.top/gtbirktstp.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jyoumei.cn/gtboviadvg.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.zycfv.cn/gthpcywdli.html

[Q57] 行号
来源：http://hz.fzhhl.top/gtdbwlcrdw.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.sxryk.cn/gtxyvzsucd.html

[Q58] 累计求和
来源：http://hz.52xcode.cn/gtbasqjugx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.jiagoushi.top/gtusmiconx.html

[Q59] 分组内累计
来源：http://hz.iojbl.cn/gtfxmutvbf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.shzxlz.cn/gtggxatzco.html

[Q60] 取上一行 / 下一行
来源：http://hz.ydzc1.top/gtqvvdyyxw.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.zhijiandao.cn/gtfsdohqcu.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.pycfn.com/gtgovxoeil.html


<!-- 参考信息 -->