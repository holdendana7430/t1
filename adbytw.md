代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.shanyushiyangtech.top/gthofolxpe.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.tianlin.xyz/gtaqctlpub.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.sufxvd.cn/gtqckyicwb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.chenzaomai.com/gtaokjjlqj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.xuanzx.com/gtannickqx.html

[N10] 链表节点定义
来源：http://hz.0kj1m.cn/gtmvthrgee.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.zhiwuduotai.top/gthryszfub.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.ydzc1.top/gtycriexsg.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zdqjudy.top/gtbybvulbe.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.316326.xyz/gttzrzmhet.html

Java: class Node { int v; Node next; }
来源：http://hz.tian-w.cn/gtvtlyapff.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.jqgfzy.top/gtjrbxeydm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.sysykeji.top/gtqqkcyrcf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.dashuyun.cn/gtpwnhomfp.html

[N11] 二叉树中序遍历
来源：http://hz.quarkkingdee.top/gtwycvjxfy.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.sxryk.cn/gthoqnflfs.html

PHP:  // 手写递归函数
来源：http://hz.shzxlz.cn/gtkcasfusb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.gaohongyu789.top/gtpuokklfw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.tanke756.top/gthjpkhfhs.html

Java: // 手写递归
来源：http://hz.fengsongda.top/gtnwhkiesf.html

Go:   // 手写递归
来源：http://hz.pycfn.com/gthxwvhcjw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.chenzaomai.com/gtdlsbvgzv.html

C#:   // 手写递归
来源：http://hz.jqgufenzy.top/gtpgoziqgl.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.ywan-chungtsiang.top/gtvnkalogp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.xinyue.icu/gthhpafcpi.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.hammf.cn/gtxcywopha.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.dianchejie.cn/gtstdnakwm.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.snrcjt.cn/gtebkqszqz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.redwolf501.top/gtidlrtnfd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.sweek.top/gtexohcada.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.zhaomingkeji.xyz/gtepyprbtg.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hywenlv.cn/gtbptymhnb.html

================================================================================
来源：http://hz.52xcode.cn/gtvdhanoak.html

O. 并发与异步
来源：http://hz.jqgfzy.top/gtpazomces.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtyksmmbqs.html

[O01] 启动一个线程
来源：http://hz.ydzc1.top/gtehwiwduq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.wangdashe.top/gtnhmipzle.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yuanzhike.top/gtuppebfne.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.yueranfly.top/gtcvhiebzq.html

TS:   // 同 JS
来源：http://hz.zdqjudy.top/gtvkjrdimr.html

Java: new Thread(() -> f()).start()
来源：http://hz.jinghuilouyu.cn/gtuovndunf.html

Go:   go f()
来源：http://hz.wangshuangyany.cn/gtsghhxcwk.html

Ruby: Thread.new { f }
来源：http://hz.guowangkeji.top/gtygsgtyar.html

C#:   Task.Run(() => F());
来源：http://hz.cdnleiting.top/gtsaedzpto.html

[O02] 使用线程池
来源：http://hz.hnqzz.top/gtudrexrgw.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.birdmap.top/gtwlbgkpmz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.xziqi.cn/gtqwdbvefd.html

JS:   // worker_threads 线程池
来源：http://hz.jinqigufen.top/gtpupgtvcx.html

TS:   // worker_threads 线程池
来源：http://hz.iojbl.cn/gtoovzsbtt.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yj20258.top/gttntuijjm.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.gotoacloud.top/gtwsubxabt.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.vqdsnc.cn/gtlkhliwfx.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.fzhhl.top/gtzapejeda.html

[O03] 加锁保护共享数据
来源：http://hz.daria6918.cn/gthrcvandt.html

Py:   with lock: shared += 1
来源：http://hz.daria6918.cn/gtcwgfxxkh.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.ppjwa.cn/gtkdxjlthv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.xuanzx.com/gtouoephqc.html

TS:   // 同 JS
来源：http://hz.daria6918.cn/gtiidxoync.html

Java: synchronized (this) { shared++; }
来源：http://hz.fzhhl.top/gthxatxxgq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yangfankeji.com/gttcwucdwp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.guannengcc.top/gtkscdyhds.html

C#:   lock (gate) { shared++; }
来源：http://hz.fzhhl.top/gtqyaiyzei.html

[O04] 定义异步函数并等待
来源：http://hz.cucudq.cn/gtvazpcblr.html

Py:   async def f():⏎    await g()
来源：http://hz.xuetiantiany.cn/gtzfjsuimr.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.snrcjt.cn/gtriemwcjr.html

JS:   async function f() { await g(); }
来源：http://hz.snrcjt.cn/gtnheipmdy.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.wangdashe.top/gtobdusmms.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.gaohongyu789.top/gtqvnukdbi.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.shanyushiyangkeji.top/gtfkwauxvj.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.xingfuxueyuan.xyz/gtatebxkqo.html

C#:   async Task F() { await G(); }
来源：http://hz.zhiwuduotai.top/gtvlymjzaq.html

[O05] 并发执行并等待全部完成
来源：http://hz.iojbl.cn/gttogdcbvf.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jlsjyb.cn/gtmyiyqmqt.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.zhixingplan.top/gtvchwagro.html

JS:   await Promise.all(tasks)
来源：http://hz.xylfe.cn/gthgsellxh.html

TS:   await Promise.all(tasks)
来源：http://hz.gaohongyu789.top/gtwmevawbe.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.hywenlv.cn/gtmzlkcdvw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.chenlongwang.top/gtaijkxssu.html

Ruby: threads.map(&:join)
来源：http://hz.yvedp.cn/gtcblnnflg.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.hywenlv.cn/gthywdivdb.html

[O06] 使用进程池
来源：http://hz.zhijiandao.cn/gtysfhzxei.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.zhiwuduotai.top/gtbehegsdi.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.dianchejie.cn/gtebtollrd.html

JS:   // child_process / cluster 模块
来源：http://hz.guowangkeji.top/gtlfzrjkrl.html

TS:   // child_process / cluster 模块
来源：http://hz.yueranfly.top/gtuggbqzdj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.andypj.xyz/gtcjbguttu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.daxiang520.top/gtbvigmcwl.html

Ruby: // fork 块
来源：http://hz.gzhubu.top/gtrttaqvap.html

C#:   Parallel.For
来源：http://hz.c1oappe.top/gtryuufacc.html

================================================================================
来源：http://hz.gzhubu.top/gtskkyshyo.html

P. 常用工具函数
来源：http://hz.redwolf501.top/gtmwkxhwip.html

================================================================================
来源：http://hz.pycfn.com/gtoisxymje.html

[P01] 生成 UUID
来源：http://hz.zdqjudy.top/gtabquoacd.html

Py:   str(uuid.uuid4())
来源：http://hz.cdnleiting.top/gtjsaebqqw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.nanxuanxn.top/gtdwkrqkpc.html

JS:   crypto.randomUUID()
来源：http://hz.iojbl.cn/gthrpapwlb.html

TS:   crypto.randomUUID()
来源：http://hz.smart0.xyz/gtflfbbjie.html

Java: UUID.randomUUID().toString()
来源：http://hz.shangyingyoupin.top/gtezfoiqqn.html

Go:   // 用 github.com/google/uuid
来源：http://hz.jlsjyb.cn/gtmlzdkxel.html

Ruby: SecureRandom.uuid
来源：http://hz.cucudq.cn/gtrwlutcge.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.zhixingplan.top/gtrhlkebwg.html

[P02] MD5 / SHA256 摘要
来源：http://hz.yj20258.top/gtotjdubbf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.pycfn.com/gtmlqnmqhc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.gzhubu.top/gtlqkehqdo.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yueranfly.top/gtimmibpbz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.hnqzz.top/gtpfqydkwi.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.wangdashe.top/gtxmnvjdcz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.zhengqikj.top/gtuwgupwcd.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.fengsongda.top/gtvfmbqvjo.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yj20258.top/gtecrhiccp.html

[P03] 生成短随机字符串
来源：http://hz.tian-w.cn/gtriluxbsl.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.nanxinkj.top/gtuxvkmlzl.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.shanyushiyangtech.top/gtdsszqyff.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.birdmap.top/gtxdsmltwf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.haohaochexian.top/gtfjbebvgo.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.sweek.top/gtvscjwgou.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.shanyushiyangkeji.top/gttsrfvbhb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.xuanzx.com/gtxrxkuwal.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.yj202588.top/gtsxzdgtaw.html

[P04] 求长度
来源：http://hz.zhoulong.xyz/gtunrysguh.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.yj20258888.top/gttvzqgysv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jinqigufen.top/gtlajyazcq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.nanxuanxn.top/gtptthlhae.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.pengpengdd.cyou/gtictkndkc.html

Java: list.size();  map.size();  s.length()
来源：http://hz.dashuyun.cn/gtjzfmcmtq.html

Go:   len(arr);  len(m)
来源：http://hz.cucudq.cn/gtkfrxpamg.html

Ruby: x.length;  x.size
来源：http://hz.hywenlv.cn/gtzkomzuwu.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.chenjidiqi.icu/gtjqhgdgfc.html

[P05] 判断两个对象内容是否相等
来源：http://hz.meibo888.top/gtukavatbk.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.sysykeji.top/gtalaghvuj.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.nanxuanxn.top/gtpzlkjuny.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.aizwys.cn/gtzksqekyp.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yonumen.top/gtoaltowar.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.yj20258888.top/gtrrknasuf.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.xingfuxueyuan.xyz/gtaojlsalb.html

Ruby: a == b
来源：http://hz.dashuyun.cn/gtgiarsiei.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.hnxiangtu.top/gtjrjkehdb.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.iojbl.cn/gtlzyjxyrl.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.jinqigfzy.top/gtpncwrfax.html

PHP:  if (empty($x)) {}
来源：http://hz.ehwqpu.com/gthibklpsz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.iojbl.cn/gtovrsiznf.html

TS:   if (x == null) {}
来源：http://hz.ydzc1.top/gtxvrmakzl.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.tanke756.top/gthbyxkcyk.html

Go:   if x == nil {}
来源：http://hz.kuanghao11.cn/gtqvvmdkzj.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.0kj1m.cn/gthmupavci.html

C#:   if (x is null) {}
来源：http://hz.shzxlz.cn/gtdfzygjbq.html

[P07] 防抖与节流
来源：http://hz.vqdsnc.cn/gtttvvevms.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.zhixingplan.top/gtbbkyofrk.html

PHP:  // 手写时间戳比较
来源：http://hz.jlsjyb.cn/gtujeujtfp.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yvedp.cn/gtmrqvvpyu.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.sweek.top/gtzlkjqred.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.jinyuanbaomall.cn/gtznbghdss.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.andypj.xyz/gtvzupbmlz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.jiagoushi.top/gtjyvlvopn.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.dashuyun.cn/gtfcwwxthc.html

[P08] 处理浮点精度问题
来源：http://hz.shanyushiyangkeji.top/gtyessxiyq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.quarkkingdee.top/gtlsngxgsu.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.hnxiangtu.top/gtlxxisrpc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.shanyushiyangkeji.top/gtzuapmtfo.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.nanxuanxn.top/gtgvxwzzqf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.chenlongwang.top/gtlzstkolu.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.redwolf501.top/gtrklzbyxe.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.zdqjudy.top/gtsxjzabca.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.shangyingyoupin.top/gtuaxcyrgn.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtnjmsxcvn.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.c1oappe.top/gtplihnons.html

================================================================================
来源：http://hz.dashuyun.cn/gtcdfsznuj.html

[Q01] 创建表
来源：http://hz.bjfxy.top/gtplwyiwzj.html

CREATE TABLE users (
来源：http://hz.52xcode.cn/gthiaivfuz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.shzxlz.cn/gtfnagezxg.html

name VARCHAR(50) NOT NULL,
来源：http://hz.nwbrower.top/gtvlnlkjrs.html

email VARCHAR(100) UNIQUE,
来源：http://hz.9152youxi.cn/gtldowwkhm.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.quarkkingdee.top/gtjbokkedu.html

);
来源：http://hz.xuetiantiany.cn/gtxsgoalos.html

[Q02] 创建带外键的表
来源：http://hz.ppjwa.cn/gtroxbzpmf.html

CREATE TABLE orders (
来源：http://hz.quarkkingdee.top/gtudlalutt.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.fzhhl.top/gtpszvvbsw.html

user_id INT NOT NULL,
来源：http://hz.cashguo.top/gtefpvirld.html

amount DECIMAL(10, 2),
来源：http://hz.xylfe.cn/gtgmplcukj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.cdnleiting.top/gtbposfzoz.html

);
来源：http://hz.shanyushiyangkeji.top/gtjkfvemcv.html

[Q03] 增加列
来源：http://hz.ybcxt.top/gtgxowkdye.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.wangdashe.top/gtxhdartwb.html

[Q04] 修改列类型
来源：http://hz.hammf.cn/gtngfaosmk.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.kuanghao11.cn/gtsnflchna.html

[Q05] 重命名列
来源：http://hz.haohaochexian.top/gtjqgjzhtc.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.c1oappe.top/gtwpdowjbn.html

[Q06] 删除列
来源：http://hz.aizwys.cn/gtyiyxdgxl.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.shanyushiyangkeji.top/gtpvupanhe.html

[Q07] 删除表
来源：http://hz.gaohongyu789.top/gtjmyyjazp.html

DROP TABLE IF EXISTS orders;
来源：http://hz.redwolf501.top/gtipjtusyz.html

[Q08] 创建普通索引
来源：http://hz.chenlongwang.top/gtayixhkyv.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.hfpthk.cn/gtookpyist.html

[Q09] 创建唯一索引
来源：http://hz.zhaomingkeji.xyz/gtnntxxqwe.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.yuanzhike.top/gtcpuijcfi.html

[Q10] 插入单行
来源：http://hz.ywan-chungtsiang.top/gtqlgmejha.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.zhoulong.xyz/gtkljuzgin.html

[Q11] 一次插入多行
来源：http://hz.tianlin.xyz/gtaxgljtha.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.dashuyun.cn/gtfotbomjt.html

[Q12] 插入后取自增 ID
来源：http://hz.quarkkingdee.top/gtppnarysc.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.ybcxt.top/gtcgefqmiw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.aibaodan.cn/gtyrabfnym.html

[Q13] 忽略重复插入
来源：http://hz.mhx1999.top/gttvmfiwgg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.ehwqpu.com/gtuegwqywt.html

[Q14] 存在则更新（upsert）
来源：http://hz.jinqigfzy.top/gtxrgagdsl.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.chenzaomai.com/gtfzgkhdsc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.cashguo.top/gtzzcdlykr.html

[Q15] 查询全部
来源：http://hz.52xcode.cn/gtqtdbfhrx.html

SELECT * FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtiihyxhgk.html

[Q16] 查询指定列
来源：http://hz.zhiwuduotai.top/gtkhccxufz.html

SELECT id, name FROM users;
来源：http://hz.cheryme.top/gtduawfwxp.html

[Q17] 条件查询
来源：http://hz.ehwqpu.com/gtfvmaavgv.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.chenzaomai.com/gtiqyqvtav.html

[Q18] 模糊匹配
来源：http://hz.gogol.net.cn/gtwyjpxqqy.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.kuanghao11.cn/gtercssnzz.html

[Q19] 范围查询
来源：http://hz.316326.xyz/gtyyirvnvk.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.ydzc1.top/gtzvealypa.html

[Q20] IN 列表
来源：http://hz.ehwqpu.com/gtpyrnogtz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.zhiwuduotai.top/gttyourjru.html

[Q21] 空值判断
来源：http://hz.0kj1m.cn/gtwtmmjuoz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.zhongyouzk.top/gtpftnpwfc.html

[Q22] 排序
来源：http://hz.hywenlv.cn/gtvycveixo.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.jinyuanbaomall.cn/gtcgkwcewx.html

[Q23] 分页
来源：http://hz.kuanghao11.cn/gtzirwpvvj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.shanyushiyangtech.top/gtacarvyhm.html

[Q24] 去重
来源：http://hz.feifeiyinyue.top/gtlqwvmbhh.html

SELECT DISTINCT city FROM users;
来源：http://hz.yanxiufei.cn/gthoxujqxe.html

[Q25] 只取前 N 条
来源：http://hz.jiagoushi.top/gtbkitjrrq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.havefunace.top/gthpjosllz.html

[Q26] 计数
来源：http://hz.316326.xyz/gtpyylvenf.html

SELECT COUNT(*) FROM users;
来源：http://hz.gaohongyu789.top/gtxtxlpofn.html

[Q27] 条件计数
来源：http://hz.ivvv.top/gtywbyshfc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yj20258888.top/gtzffqxamy.html

[Q28] 求和与平均
来源：http://hz.xziqi.cn/gtyfgjyetu.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.svipenyu.cn/gtlgjizhvx.html

[Q29] 最大最小值
来源：http://hz.ybcxt.top/gtytdyrudx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.svipenyu.cn/gtgyvyqauz.html

[Q30] 分组统计
来源：http://hz.tian-w.cn/gtrwefjxhd.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.yuxming.cn/gtmthkqgel.html

[Q31] 分组后过滤
来源：http://hz.c1oappe.top/gtcuxgzxdt.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.sufxvd.cn/gtpkyypcuh.html

[Q32] 分组拼接字符串
来源：http://hz.yuanzhike.top/gthukugzin.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.birdmap.top/gtxacaeeid.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.cqqwz.cn/gthrhzesil.html

[Q33] 多列分组
来源：http://hz.mhx1999.top/gtbnttyher.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.316326.xyz/gtijyvnpwt.html

[Q34] 每组取第一条
来源：http://hz.pycfn.com/gtmtxrnmtn.html

SELECT * FROM (
来源：http://hz.hfpthk.cn/gtmfwumizv.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.shanyushiyangtech.top/gtyrciuwgb.html

) t WHERE rn = 1;
来源：http://hz.zhengqikj.top/gtsuzjywxy.html

[Q35] 内连接
来源：http://hz.daxiang520.top/gtjadzxhlc.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.jinghuilouyu.cn/gtplpncfxa.html

[Q36] 左连接
来源：http://hz.ydjk.org.cn/gtvqjkjppq.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.jqgufenzy.top/gttkupgwha.html

[Q37] 右连接
来源：http://hz.jqgfzy.top/gtykldqhuo.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.haohaochexian.top/gtrxowakbi.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.ywan-chungtsiang.top/gtshrvcckd.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.zhaomingkeji.xyz/gtykvbsbyu.html

[Q39] 自连接（查上下级）
来源：http://hz.shanyushiyangtech.top/gtycjvazjz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.chenjidiqi.icu/gtouxcuczu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yvedp.cn/gtgtpczwsw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.haohaochexian.top/gtpepxrchi.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.wangshuangyany.cn/gtdlxmjwvg.html

[Q41] 多表连接
来源：http://hz.vqdsnc.cn/gtctblglaf.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.mhx1999.top/gtrdipwfij.html

JOIN users u ON u.id = o.user_id
来源：http://hz.9152youxi.cn/gtrssjoyzg.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.fzhhl.top/gtfoggreml.html

[Q42] 连接条件附加过滤
来源：http://hz.xziqi.cn/gtvpkfwxgr.html

SELECT u.name, o.amount FROM users u
来源：http://hz.cashguo.top/gthwqwfwuo.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.shzxlz.cn/gtqaxrdpik.html

[Q43] 标量子查询
来源：http://hz.aibaodan.cn/gtyjflikay.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.cqqwz.cn/gtxuxcnhfr.html

[Q44] IN 子查询
来源：http://hz.jinyuanbaomall.cn/gtwohyauwr.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.yongpay.top/gtohqrqmdg.html

[Q45] EXISTS 判断存在
来源：http://hz.xinyue.icu/gtgprlcoxn.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yueranfly.top/gtfzsbygvm.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.xuanzx.com/gtgaaidzbu.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.cheryme.top/gtycysjgem.html

[Q47] 与平均值比较
来源：http://hz.xuetiantiany.cn/gtaidvgnvu.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jinqigufen.top/gtxitvurps.html

[Q48] CTE 公用表表达式
来源：http://hz.aibaodan.cn/gtlzxieulc.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.chenjidiqi.icu/gtiiqkdwmr.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.zhiwuduotai.top/gtqkabgaoi.html

[Q49] 更新单行
来源：http://hz.ppjwa.cn/gtkwajiojv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.c1oappe.top/gtdwsorkdw.html

[Q50] 批量更新
来源：http://hz.52xcode.cn/gtihxwjjbk.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.sufxvd.cn/gtpefskljv.html

[Q51] 用子查询更新
来源：http://hz.gaohongyu789.top/gteeazcywe.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.chenjidiqi.icu/gtfdjormpf.html

[Q52] 删除指定行
来源：http://hz.gaohongyu789.top/gtkwlzxwbm.html

DELETE FROM users WHERE id = 10;
来源：http://hz.feifeiyinyue.top/gtrctxfhdd.html

[Q53] 按条件删除
来源：http://hz.tianlin.xyz/gtgzfyzfar.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.hnqzz.top/gtihrrgsak.html

[Q54] 清空表
来源：http://hz.52xcode.cn/gtxiguenct.html

TRUNCATE TABLE logs;
来源：http://hz.andypj.xyz/gtiidlhyro.html

[Q55] 排名（并列占位）
来源：http://hz.sweek.top/gtapcgovyx.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.hnxiangtu.top/gttwczmudt.html

[Q56] 密集排名（并列不占位）
来源：http://hz.sweek.top/gtnicjxtyv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.cashguo.top/gtvdxtsioy.html

[Q57] 行号
来源：http://hz.ybcxt.top/gtvuyzjemr.html


<!-- 参考信息 -->