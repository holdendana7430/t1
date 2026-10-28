代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.cdnleiting.top/gtvbfuwulm.html

[N10] 链表节点定义
来源：http://hz.fengsongda.top/gtpqfakylp.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.haohaochexian.top/gtklidewik.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.kuanghao11.cn/gtmjictiuw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.havefunace.top/gtyyeipeua.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.0kj1m.cn/gtkotsdtyu.html

Java: class Node { int v; Node next; }
来源：http://hz.yongpay.top/gtyukxqplm.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.ywan-chungtsiang.top/gtsaqvpfbs.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.zdqjudy.top/gttvozsckm.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.316326.xyz/gtrnlxndds.html

[N11] 二叉树中序遍历
来源：http://hz.guowangkeji.top/gtaumdcqil.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.zhengqikj.top/gtxlvckqjq.html

PHP:  // 手写递归函数
来源：http://hz.andypj.xyz/gtoquyimjc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.gzhubu.top/gtckjbdyya.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.sxryk.cn/gtdomutlry.html

Java: // 手写递归
来源：http://hz.ywan-chungtsiang.top/gtiqgpltam.html

Go:   // 手写递归
来源：http://hz.ydzc1.top/gtunpdarmo.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.wangdashe.top/gtlwxbxcrr.html

C#:   // 手写递归
来源：http://hz.xuanzx.com/gtwvulhvcp.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.havefunace.top/gtmctyydjx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.tian-w.cn/gtwcxnlzqd.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.havefunace.top/gtdtdxypqv.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.quarkkingdee.top/gtzvxmnmrk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jiagoushi.top/gthyuxedbo.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.pengpengdd.cyou/gtzpoylatg.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.jyoumei.cn/gtqtgmqnwz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.snrcjt.cn/gtfvarltxa.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.mhx1999.top/gtniimrrvc.html

================================================================================
来源：http://hz.xuanzx.com/gtfjvlpkta.html

O. 并发与异步
来源：http://hz.svipenyu.cn/gtlevfuzde.html

================================================================================
来源：http://hz.chenlongwang.top/gtkhspapfu.html

[O01] 启动一个线程
来源：http://hz.zycfv.cn/gtmeueofuu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.chenlongwang.top/gtymmvamdq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.pengpengdd.cyou/gtkbxnttec.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.xinyue.icu/gthyqvmehs.html

TS:   // 同 JS
来源：http://hz.tanke756.top/gtalelvjvt.html

Java: new Thread(() -> f()).start()
来源：http://hz.jyoumei.cn/gtduahlwtk.html

Go:   go f()
来源：http://hz.jqgfzy.top/gtlwajaitl.html

Ruby: Thread.new { f }
来源：http://hz.smart0.xyz/gtaqnzzkbx.html

C#:   Task.Run(() => F());
来源：http://hz.shuidangran.top/gtdspxspaj.html

[O02] 使用线程池
来源：http://hz.xylfe.cn/gtcqaqdtsz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.cashguo.top/gtudalacob.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.xuetiantiany.cn/gtpiahmltd.html

JS:   // worker_threads 线程池
来源：http://hz.sxryk.cn/gtzcekgqvi.html

TS:   // worker_threads 线程池
来源：http://hz.dianchejie.cn/gtgoulnjat.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.guannengcc.top/gtjoxkwepo.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.sweek.top/gtwcfbltoz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.zhixingplan.top/gtxerkbeyv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.shangyingyoupin.top/gtqnwibunk.html

[O03] 加锁保护共享数据
来源：http://hz.quarkkingdee.top/gtissfpklt.html

Py:   with lock: shared += 1
来源：http://hz.zhixingplan.top/gtfjzlarem.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.sysykeji.top/gtazmmltyb.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.zhaomingkeji.xyz/gtaitolffh.html

TS:   // 同 JS
来源：http://hz.chenlongwang.top/gtodzuqzxw.html

Java: synchronized (this) { shared++; }
来源：http://hz.jinqigufen.top/gtczicsuox.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.52xcode.cn/gtwkftsief.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.fengsongda.top/gtruzemzyk.html

C#:   lock (gate) { shared++; }
来源：http://hz.ppjwa.cn/gtgtkcxdto.html

[O04] 定义异步函数并等待
来源：http://hz.jianghu66.top/gtcsmvzfqi.html

Py:   async def f():⏎    await g()
来源：http://hz.kuanghao11.cn/gtxshmdpyu.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.daxiang520.top/gtuonyygux.html

JS:   async function f() { await g(); }
来源：http://hz.hongshengwenyu.top/gtklrzfnzv.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.mhx1999.top/gtohotihtj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.yueranfly.top/gtdzxxwrez.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.hywenlv.cn/gtmfsuvwle.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.jyoumei.cn/gthndlvnkt.html

C#:   async Task F() { await G(); }
来源：http://hz.chenjidiqi.icu/gtohrpdepi.html

[O05] 并发执行并等待全部完成
来源：http://hz.jiagoushi.top/gthemywynw.html

Py:   asyncio.gather(*tasks)
来源：http://hz.ydjk.org.cn/gtpmhlwphj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.pycfn.com/gtpllkyyzd.html

JS:   await Promise.all(tasks)
来源：http://hz.xuetiantiany.cn/gtfeygwaxl.html

TS:   await Promise.all(tasks)
来源：http://hz.iojbl.cn/gtpbeqprwr.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.pycfn.com/gtemtcncyv.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.jinghuilouyu.cn/gtlkaxdvgj.html

Ruby: threads.map(&:join)
来源：http://hz.cashguo.top/gtwpiefruc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.ywan-chungtsiang.top/gtlioujrek.html

[O06] 使用进程池
来源：http://hz.andypj.xyz/gtpbfepixr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.iojbl.cn/gtuvjhnjho.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.tanke756.top/gtwecigovz.html

JS:   // child_process / cluster 模块
来源：http://hz.yueranfly.top/gtjrqwmzxw.html

TS:   // child_process / cluster 模块
来源：http://hz.jiagoushi.top/gtftrszeau.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yj202588.top/gtxwbamffj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.yanxiufei.cn/gtmtbficgc.html

Ruby: // fork 块
来源：http://hz.svipenyu.cn/gtvogzimcw.html

C#:   Parallel.For
来源：http://hz.yuxming.cn/gtejeaoqsk.html

================================================================================
来源：http://hz.zhongyouzk.top/gtkcrbymgl.html

P. 常用工具函数
来源：http://hz.yuanzhike.top/gtiezwmibc.html

================================================================================
来源：http://hz.snrcjt.cn/gtsavkwdmo.html

[P01] 生成 UUID
来源：http://hz.zhoulong.xyz/gtsqeiydia.html

Py:   str(uuid.uuid4())
来源：http://hz.shanyushiyangkeji.top/gtuictbcnb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jinghuilouyu.cn/gtebihmgxc.html

JS:   crypto.randomUUID()
来源：http://hz.chenjidiqi.icu/gtgoaehdsl.html

TS:   crypto.randomUUID()
来源：http://hz.guannengcc.top/gtmwctmilh.html

Java: UUID.randomUUID().toString()
来源：http://hz.pycfn.com/gtrprzpdpl.html

Go:   // 用 github.com/google/uuid
来源：http://hz.cheryme.top/gtsriccsap.html

Ruby: SecureRandom.uuid
来源：http://hz.dianchejie.cn/gtpdceermw.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.pengpengdd.cyou/gtiirwjoub.html

[P02] MD5 / SHA256 摘要
来源：http://hz.sweek.top/gtshdxaafv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.xuanzx.com/gtukxanlou.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.hnxiangtu.top/gtyxntmela.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.daxiang520.top/gtktkzfkat.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.cdnleiting.top/gtodthvyfm.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.pycfn.com/gtfgqdrtry.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.xziqi.cn/gtdnavlask.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.mhx1999.top/gtwousvcew.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.nanxuanxn.top/gtxybqsgaw.html

[P03] 生成短随机字符串
来源：http://hz.sweek.top/gtkulifcoi.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.cdnleiting.top/gtzthupeua.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.ehwqpu.com/gtpficbvrj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ydzc1.top/gtzczbmsvo.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xuetiantiany.cn/gtivruhzso.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.birdmap.top/gtfrupwxcj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.zhengqikj.top/gtfmswwbck.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.cashguo.top/gtabdltjyt.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.andypj.xyz/gtyhnkiqqk.html

[P04] 求长度
来源：http://hz.hammf.cn/gtluhduxmi.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.gaohongyu789.top/gtoftfvhhn.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.fengsongda.top/gtolagtghh.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.snrcjt.cn/gtlfnmyucu.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.52xcode.cn/gtkswbcpdl.html

Java: list.size();  map.size();  s.length()
来源：http://hz.jianghu66.top/gtedbosapv.html

Go:   len(arr);  len(m)
来源：http://hz.yonumen.top/gtnmhupuol.html

Ruby: x.length;  x.size
来源：http://hz.shanyushiyangkeji.top/gtmzpypzzo.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.ydjk.org.cn/gtnbooizij.html

[P05] 判断两个对象内容是否相等
来源：http://hz.hfpthk.cn/gtlmurbyrn.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.316326.xyz/gtxotibsap.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.nwbrower.top/gthelcknie.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.9152youxi.cn/gtpxgxthza.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.guannengcc.top/gtibehypbm.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jianghu66.top/gtrclvpnuu.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.nwbrower.top/gtkxjcqylw.html

Ruby: a == b
来源：http://hz.havefunace.top/gthcdafwhp.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.birdmap.top/gtuyazwltr.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.aibaodan.cn/gteubcoeww.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.xinyue.icu/gtbezpnzcr.html

PHP:  if (empty($x)) {}
来源：http://hz.xinyue.icu/gtbpmrfgdf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.hongshengwenyu.top/gtvjmigzbk.html

TS:   if (x == null) {}
来源：http://hz.ydjk.org.cn/gttcwdoezm.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.birdmap.top/gtyqfnsrac.html

Go:   if x == nil {}
来源：http://hz.zycfv.cn/gtlojkbvfq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.hongshengwenyu.top/gtpogwscvg.html

C#:   if (x is null) {}
来源：http://hz.hysaishi.cn/gtqlucsbhq.html

[P07] 防抖与节流
来源：http://hz.havefunace.top/gtpyruswkz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.0kj1m.cn/gttqbzftob.html

PHP:  // 手写时间戳比较
来源：http://hz.zhaomingkeji.xyz/gtxrwttlte.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.daxiang520.top/gtbjgatgdd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.chenlongwang.top/gtnlschuka.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.cqqwz.cn/gtmdzchdwt.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.aibaodan.cn/gteniuvtqs.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.birdmap.top/gtipiwrxwe.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.redwolf501.top/gtzwmopskv.html

[P08] 处理浮点精度问题
来源：http://hz.jinghuilouyu.cn/gtsxliioei.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jqgufenzy.top/gttsksbtfs.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.cqqwz.cn/gtjuizrsps.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.c1oappe.top/gtejffxmas.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.ydjk.org.cn/gtaclkhfin.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.zhijiandao.cn/gtyfxowzkm.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.jlsjyb.cn/gtzhxmdbke.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.jyoumei.cn/gttsdmqfxt.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.yongpay.top/gteyshcilw.html

================================================================================
来源：http://hz.daria6918.cn/gtpqyjtdpi.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.jinyuanbaomall.cn/gtjzlrlpiy.html

================================================================================
来源：http://hz.gotoacloud.top/gttvxfqmoo.html

[Q01] 创建表
来源：http://hz.316326.xyz/gtepvymakh.html

CREATE TABLE users (
来源：http://hz.c1oappe.top/gtuvmejlpm.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yangfankeji.com/gtvflcmgrv.html

name VARCHAR(50) NOT NULL,
来源：http://hz.shanyushiyangtech.top/gtkowpfmae.html

email VARCHAR(100) UNIQUE,
来源：http://hz.yanxiufei.cn/gtvlhbkzpe.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.xylfe.cn/gtmoeyftuj.html

);
来源：http://hz.chenzaomai.com/gthsbwhofb.html

[Q02] 创建带外键的表
来源：http://hz.zhiwuduotai.top/gtltyjbrmj.html

CREATE TABLE orders (
来源：http://hz.jlsjyb.cn/gtjidwpoiw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.sweek.top/gtpwufzsbz.html

user_id INT NOT NULL,
来源：http://hz.sufxvd.cn/gtmcorsqht.html

amount DECIMAL(10, 2),
来源：http://hz.cashguo.top/gtuclfujnw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.sysykeji.top/gtewzivsha.html

);
来源：http://hz.yj202588.top/gtkzivaysq.html

[Q03] 增加列
来源：http://hz.zhongyouzk.top/gtmhnflfvj.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.nanxinkj.top/gtnszhuzpf.html

[Q04] 修改列类型
来源：http://hz.hongshengwenyu.top/gtzacshraz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.shangyingyoupin.top/gtkpnusoma.html

[Q05] 重命名列
来源：http://hz.9152youxi.cn/gtsbtgdajn.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.tianlin.xyz/gthzarzscl.html

[Q06] 删除列
来源：http://hz.ydjk.org.cn/gtjgunmqld.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.ydzc1.top/gtoqahwyuy.html

[Q07] 删除表
来源：http://hz.chenlongwang.top/gtpzugnncv.html

DROP TABLE IF EXISTS orders;
来源：http://hz.jinqigfzy.top/gtuveowcke.html

[Q08] 创建普通索引
来源：http://hz.cdnleiting.top/gtepprsmav.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.tian-w.cn/gttrkdccbu.html

[Q09] 创建唯一索引
来源：http://hz.hammf.cn/gttubwfzcn.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.jqgfzy.top/gtfhehkpqk.html

[Q10] 插入单行
来源：http://hz.cqqwz.cn/gttgobytax.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.nanxuanxn.top/gtiipxvdmr.html

[Q11] 一次插入多行
来源：http://hz.yj20258888.top/gtunkpefnp.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.cdnleiting.top/gtfcmubgcx.html

[Q12] 插入后取自增 ID
来源：http://hz.gotoacloud.top/gtaflauorz.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.pengpengdd.cyou/gtrxtjbaus.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.cqqwz.cn/gtzhpinrkw.html

[Q13] 忽略重复插入
来源：http://hz.dianchejie.cn/gtviyaingr.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jiagoushi.top/gtqwkjlvpe.html

[Q14] 存在则更新（upsert）
来源：http://hz.chenzaomai.com/gtfoadorch.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.svipenyu.cn/gttnaqyauo.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.wangshuangyany.cn/gtlucuemke.html

[Q15] 查询全部
来源：http://hz.jlsjyb.cn/gtfvynqfog.html

SELECT * FROM users;
来源：http://hz.fzhhl.top/gtwqkugsyi.html

[Q16] 查询指定列
来源：http://hz.yonumen.top/gtwegyagon.html

SELECT id, name FROM users;
来源：http://hz.zycfv.cn/gturawygcs.html

[Q17] 条件查询
来源：http://hz.meibo888.top/gtehuwthum.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.yongpay.top/gtrmtguvod.html

[Q18] 模糊匹配
来源：http://hz.ydjk.org.cn/gtwjiikbks.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.nanxuanxn.top/gtldkzpmlt.html

[Q19] 范围查询
来源：http://hz.ybcxt.top/gttaehvuyl.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.zhengqikj.top/gtkwbfkxlw.html

[Q20] IN 列表
来源：http://hz.sweek.top/gtwnitvkqj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.kuanghao11.cn/gtsbdquqeq.html

[Q21] 空值判断
来源：http://hz.dashuyun.cn/gtmoknltdl.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.yj20258.top/gtvfietpfl.html

[Q22] 排序
来源：http://hz.birdmap.top/gtmjrbasxg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.shangyingyoupin.top/gtuboiczpx.html

[Q23] 分页
来源：http://hz.ydzc1.top/gthohiincm.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.gogol.net.cn/gthwjbbfdq.html

[Q24] 去重
来源：http://hz.yvedp.cn/gtgbfgsuqf.html

SELECT DISTINCT city FROM users;
来源：http://hz.cqqwz.cn/gtvmlpbvor.html

[Q25] 只取前 N 条
来源：http://hz.52xcode.cn/gtxlwbuqak.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.snrcjt.cn/gtinpniqnm.html

[Q26] 计数
来源：http://hz.nanxuanxn.top/gtgvhlzeud.html

SELECT COUNT(*) FROM users;
来源：http://hz.vqdsnc.cn/gtcgagrzhi.html

[Q27] 条件计数
来源：http://hz.shangyingyoupin.top/gthogzkero.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.guowangkeji.top/gtmlozgcfv.html

[Q28] 求和与平均
来源：http://hz.yvedp.cn/gtjualqknz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.ybcxt.top/gtymntisgk.html

[Q29] 最大最小值
来源：http://hz.yueranfly.top/gtrjosqxxl.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.havefunace.top/gtkopfgmbz.html

[Q30] 分组统计
来源：http://hz.tianlin.xyz/gtcwosatbw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.9152youxi.cn/gtxumpvimc.html

[Q31] 分组后过滤
来源：http://hz.iojbl.cn/gtuxtmnqsq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.wangshuangyany.cn/gtzklhcwcw.html

[Q32] 分组拼接字符串
来源：http://hz.yueranfly.top/gtqagptmea.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.cashguo.top/gtuuhukuns.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.quarkkingdee.top/gthmluggdv.html

[Q33] 多列分组
来源：http://hz.zhongyouzk.top/gtzraazico.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.jqgufenzy.top/gtadgjszmn.html

[Q34] 每组取第一条
来源：http://hz.jlsjyb.cn/gtxqrhnigb.html

SELECT * FROM (
来源：http://hz.daria6918.cn/gtqefndude.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.zhiwuduotai.top/gtsvnxaugz.html

) t WHERE rn = 1;
来源：http://hz.zhaomingkeji.xyz/gtpkimuhyp.html

[Q35] 内连接
来源：http://hz.hongshengwenyu.top/gtaunubcyh.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.yanxiufei.cn/gtfrnkclsb.html

[Q36] 左连接
来源：http://hz.nanxinkj.top/gtwvgyccxn.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.shzxlz.cn/gtmrchrgiy.html

[Q37] 右连接
来源：http://hz.ybcxt.top/gtifcukqvd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.havefunace.top/gtcqmreikv.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.fzhhl.top/gtwxtscbhu.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.iojbl.cn/gtvooqysjh.html

[Q39] 自连接（查上下级）
来源：http://hz.xingfuxueyuan.xyz/gtmdghfgod.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jyoumei.cn/gtmxelwjkv.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.shanyushiyangkeji.top/gtwnvjdisy.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.yj202588.top/gtansofcvp.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.gzhubu.top/gtyavqekav.html

[Q41] 多表连接
来源：http://hz.aizwys.cn/gtotdnqexw.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.sysykeji.top/gtfszyjrqy.html

JOIN users u ON u.id = o.user_id
来源：http://hz.shangyingyoupin.top/gtgjkaszfq.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.yj20258.top/gtsadpbyeb.html

[Q42] 连接条件附加过滤
来源：http://hz.tanke756.top/gtjbhcsfhw.html

SELECT u.name, o.amount FROM users u
来源：http://hz.jinyuanbaomall.cn/gtpsxheosj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.nwbrower.top/gtqbrtqodm.html

[Q43] 标量子查询
来源：http://hz.nanxinkj.top/gtoikdzcqw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.zhiwuduotai.top/gtapigovih.html

[Q44] IN 子查询
来源：http://hz.9152youxi.cn/gtpuwtgqgp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.xinyue.icu/gthyjpivyf.html

[Q45] EXISTS 判断存在
来源：http://hz.xuanzx.com/gtlyafoiyl.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.shuidangran.top/gtkolwzgtk.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.vqdsnc.cn/gtkmtapqcb.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hywenlv.cn/gtrrdlvtny.html

[Q47] 与平均值比较
来源：http://hz.tian-w.cn/gtopbshlni.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.zhijiandao.cn/gtgxawgvvk.html

[Q48] CTE 公用表表达式
来源：http://hz.andypj.xyz/gtyjsmuflr.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.yj20258888.top/gtdbpmcubc.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.mhx1999.top/gtgjpyaupx.html

[Q49] 更新单行
来源：http://hz.redwolf501.top/gtanshuycb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.havefunace.top/gtdmcpqbtf.html

[Q50] 批量更新
来源：http://hz.zycfv.cn/gtlnadqzad.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.snrcjt.cn/gtuxilgdnb.html

[Q51] 用子查询更新
来源：http://hz.zhaomingkeji.xyz/gtwgcmjsjc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.andypj.xyz/gtbrlyroqp.html

[Q52] 删除指定行
来源：http://hz.yj20258.top/gtrolphcqy.html

DELETE FROM users WHERE id = 10;
来源：http://hz.cheryme.top/gtpjfirmip.html

[Q53] 按条件删除
来源：http://hz.shangyingyoupin.top/gtzqvijtgz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.hammf.cn/gtvqebovpl.html

[Q54] 清空表
来源：http://hz.xinyue.icu/gtkogyatyn.html

TRUNCATE TABLE logs;
来源：http://hz.shuidangran.top/gtkcltpmay.html

[Q55] 排名（并列占位）
来源：http://hz.pycfn.com/gthnqkvarz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.zhijiandao.cn/gtxmrvwnjm.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jyoumei.cn/gtprfybdnx.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.shanyushiyangkeji.top/gtouegttqa.html

[Q57] 行号
来源：http://hz.sysykeji.top/gtuaootvwq.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.ywan-chungtsiang.top/gtiujmjlvj.html

[Q58] 累计求和
来源：http://hz.haohaochexian.top/gtyxibavtx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.tanke756.top/gtoecjixgu.html

[Q59] 分组内累计
来源：http://hz.guowangkeji.top/gtytautyqo.html


<!-- 参考信息 -->