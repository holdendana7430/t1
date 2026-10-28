代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.ppjwa.cn/gtxhjmuzbn.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.hnqzz.top/gtbgbkujrp.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.nanxinkj.top/gtojybtdae.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.nanxinkj.top/gtlreipzyw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.redwolf501.top/gtvjfntdwl.html

[N10] 链表节点定义
来源：http://hz.yanxiufei.cn/gtcxtwcbus.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yonumen.top/gtqawssqsb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.yangfankeji.com/gtvlvexgwh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zhijiandao.cn/gtijqcpbfn.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.9152youxi.cn/gtoddbhcxp.html

Java: class Node { int v; Node next; }
来源：http://hz.ppjwa.cn/gtsvofrvuc.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.haohaochexian.top/gtsxailvaj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.cucudq.cn/gtwelwahhm.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.tian-w.cn/gtfxkksiwo.html

[N11] 二叉树中序遍历
来源：http://hz.ywan-chungtsiang.top/gtotcztfqk.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.sufxvd.cn/gtrchnixhq.html

PHP:  // 手写递归函数
来源：http://hz.pycfn.com/gtfsrkvkad.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.gotoacloud.top/gttsmtplgr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.xuetiantiany.cn/gttxakyiex.html

Java: // 手写递归
来源：http://hz.shzxlz.cn/gtmsgomfzz.html

Go:   // 手写递归
来源：http://hz.c1oappe.top/gtqfeylyuy.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.zhixingplan.top/gtwxyqhbtm.html

C#:   // 手写递归
来源：http://hz.zhiwuduotai.top/gtcdznfdfv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.jinghuilouyu.cn/gtqqbonwvh.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.nwbrower.top/gthifotrae.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.52xcode.cn/gttwhktnfq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ppjwa.cn/gtfykzkypt.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hnxiangtu.top/gtpwadvpwg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ydjk.org.cn/gtxorvlyxb.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.gotoacloud.top/gtohvrtjcu.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.fzhhl.top/gtcqizguod.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hnqzz.top/gtlkuhybmn.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtwqnhavwz.html

O. 并发与异步
来源：http://hz.havefunace.top/gtshkrxowg.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtpnkyvbsp.html

[O01] 启动一个线程
来源：http://hz.zdqjudy.top/gtmmikudgo.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.havefunace.top/gtctedakos.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.cqqwz.cn/gtyopdnzcd.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.guowangkeji.top/gtnnzvulbg.html

TS:   // 同 JS
来源：http://hz.hysaishi.cn/gtkdbwurdm.html

Java: new Thread(() -> f()).start()
来源：http://hz.zycfv.cn/gtoqcjqdxr.html

Go:   go f()
来源：http://hz.kuanghao11.cn/gtvgvljgii.html

Ruby: Thread.new { f }
来源：http://hz.pycfn.com/gtwxvzjrxt.html

C#:   Task.Run(() => F());
来源：http://hz.ppjwa.cn/gtakzcyfey.html

[O02] 使用线程池
来源：http://hz.jianghu66.top/gtaqpvvyrt.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.cashguo.top/gtcyhnusnj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.feifeiyinyue.top/gtvfktemmi.html

JS:   // worker_threads 线程池
来源：http://hz.zhixingplan.top/gtlcdciddw.html

TS:   // worker_threads 线程池
来源：http://hz.feifeiyinyue.top/gtbtuavtds.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.mhx1999.top/gtktsnazsv.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.c1oappe.top/gtqqeotzqh.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.vqdsnc.cn/gthlhnhbsa.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.bjfxy.top/gthrtrxrhk.html

[O03] 加锁保护共享数据
来源：http://hz.jyoumei.cn/gtonymjtoj.html

Py:   with lock: shared += 1
来源：http://hz.cheryme.top/gtalphkjgc.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.kuanghao11.cn/gtgdwqhani.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.wangshuangyany.cn/gtifablxet.html

TS:   // 同 JS
来源：http://hz.xuanzx.com/gtpnaajird.html

Java: synchronized (this) { shared++; }
来源：http://hz.52xcode.cn/gtsnwkkmoq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.feifeiyinyue.top/gtyexigryw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.tanke756.top/gtrlnzkbyd.html

C#:   lock (gate) { shared++; }
来源：http://hz.jqgufenzy.top/gtaxwiwjmj.html

[O04] 定义异步函数并等待
来源：http://hz.cucudq.cn/gtlywavjsk.html

Py:   async def f():⏎    await g()
来源：http://hz.guowangkeji.top/gtalfbjwgh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.ywan-chungtsiang.top/gtzytmsubv.html

JS:   async function f() { await g(); }
来源：http://hz.fengsongda.top/gtrgyxtgdl.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.xuanzx.com/gtweyuyacq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.aibaodan.cn/gtjgljxhyd.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.shzxlz.cn/gtcudckuid.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.birdmap.top/gttshnombr.html

C#:   async Task F() { await G(); }
来源：http://hz.c1oappe.top/gttswuvmdx.html

[O05] 并发执行并等待全部完成
来源：http://hz.hnxiangtu.top/gthndqkbvn.html

Py:   asyncio.gather(*tasks)
来源：http://hz.snrcjt.cn/gtrjzzvoqo.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.gzhubu.top/gtedefpywf.html

JS:   await Promise.all(tasks)
来源：http://hz.gogol.net.cn/gtphcdimsm.html

TS:   await Promise.all(tasks)
来源：http://hz.daxiang520.top/gtweklyviz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.cqqwz.cn/gtbvzypvvr.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.jyoumei.cn/gtubhvjaff.html

Ruby: threads.map(&:join)
来源：http://hz.cqqwz.cn/gtnernltzu.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.havefunace.top/gtrpdaojru.html

[O06] 使用进程池
来源：http://hz.nwbrower.top/gtlgwxowlf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.daria6918.cn/gtynufgfhj.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.yuanzhike.top/gtwafrrhsn.html

JS:   // child_process / cluster 模块
来源：http://hz.snrcjt.cn/gtrefxrvep.html

TS:   // child_process / cluster 模块
来源：http://hz.yj202588.top/gtyhbcimar.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.ywan-chungtsiang.top/gtmofyknbi.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.tianlin.xyz/gtmlasysit.html

Ruby: // fork 块
来源：http://hz.nanxinkj.top/gtwdconodc.html

C#:   Parallel.For
来源：http://hz.hammf.cn/gtrwoajgav.html

================================================================================
来源：http://hz.yuanzhike.top/gtjrhxpodl.html

P. 常用工具函数
来源：http://hz.sysykeji.top/gtbgcwvenc.html

================================================================================
来源：http://hz.hfpthk.cn/gtwxesyacp.html

[P01] 生成 UUID
来源：http://hz.yonumen.top/gtbgmssicg.html

Py:   str(uuid.uuid4())
来源：http://hz.hammf.cn/gtjbebmlhm.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.xuanzx.com/gtpjhajikx.html

JS:   crypto.randomUUID()
来源：http://hz.nanxuanxn.top/gttgaqyjcb.html

TS:   crypto.randomUUID()
来源：http://hz.dashuyun.cn/gtvqarasnf.html

Java: UUID.randomUUID().toString()
来源：http://hz.dianchejie.cn/gtkrdyiage.html

Go:   // 用 github.com/google/uuid
来源：http://hz.xylfe.cn/gtnronvvbu.html

Ruby: SecureRandom.uuid
来源：http://hz.jlsjyb.cn/gtedycqosy.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.jinghuilouyu.cn/gtrzjiseal.html

[P02] MD5 / SHA256 摘要
来源：http://hz.sufxvd.cn/gtudnoabxl.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.chenjidiqi.icu/gtlytgsgog.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.zdqjudy.top/gtmdnsphcp.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.xingfuxueyuan.xyz/gtclaqusok.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.hnqzz.top/gtcxwvoyuw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.yj202588.top/gtcbygleyl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.hfpthk.cn/gtkzzhtwaw.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.svipenyu.cn/gtpuaixlch.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.meibo888.top/gtepzsvmhv.html

[P03] 生成短随机字符串
来源：http://hz.gogol.net.cn/gtrkpgdois.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.tianlin.xyz/gtgaadsugo.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.gogol.net.cn/gttmyxxqlx.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.daria6918.cn/gteebwhbtf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hysaishi.cn/gtodcctvhx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jqgfzy.top/gtzwabnhlg.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yj202588.top/gtxjhufamb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jiagoushi.top/gtvbzsmaoi.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.hammf.cn/gtngmzbxqi.html

[P04] 求长度
来源：http://hz.ivvv.top/gtzwdsgdpe.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.nanxinkj.top/gtvcrofskd.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.nanxuanxn.top/gtyvohjmjp.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yonumen.top/gtapvllaux.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.cheryme.top/gtxmstsmeb.html

Java: list.size();  map.size();  s.length()
来源：http://hz.cdnleiting.top/gtaptpsish.html

Go:   len(arr);  len(m)
来源：http://hz.ehwqpu.com/gtueiczdhb.html

Ruby: x.length;  x.size
来源：http://hz.shuidangran.top/gtfetxnfpc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.wangshuangyany.cn/gtvlansyha.html

[P05] 判断两个对象内容是否相等
来源：http://hz.vqdsnc.cn/gtkfkhtlfq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.yj202588.top/gtemkgohnn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.xingfuxueyuan.xyz/gtbqghppei.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.hongshengwenyu.top/gtsvygnkrn.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.ydzc1.top/gtchlqlogz.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.zhoulong.xyz/gtmteqoyks.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.hammf.cn/gtoohgkyyu.html

Ruby: a == b
来源：http://hz.zdqjudy.top/gtsdvugtny.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.ydzc1.top/gtuvghqcqq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.jinyuanbaomall.cn/gtcqywurte.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.andypj.xyz/gtpvoyibzm.html

PHP:  if (empty($x)) {}
来源：http://hz.yanxiufei.cn/gtbpnrftbu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.aibaodan.cn/gtuduwjclj.html

TS:   if (x == null) {}
来源：http://hz.316326.xyz/gtnfpaihxb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.shuidangran.top/gtvlqgxziv.html

Go:   if x == nil {}
来源：http://hz.zhaomingkeji.xyz/gtxrqafgkx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.hongshengwenyu.top/gtwxenqoft.html

C#:   if (x is null) {}
来源：http://hz.bjfxy.top/gtykmxqvdu.html

[P07] 防抖与节流
来源：http://hz.cashguo.top/gtosrvwftv.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.hongshengwenyu.top/gtjkokphdj.html

PHP:  // 手写时间戳比较
来源：http://hz.shanyushiyangkeji.top/gtsssgcpar.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.chenlongwang.top/gtcbafarkt.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.chenlongwang.top/gtzoaewtgf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.zhoulong.xyz/gtdvinttcj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.vqdsnc.cn/gtaruwrylk.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.nanxuanxn.top/gtjhiomckf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.birdmap.top/gtpkmbxkwf.html

[P08] 处理浮点精度问题
来源：http://hz.52xcode.cn/gtxpffkpid.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.hongshengwenyu.top/gtwuircxsv.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.shanyushiyangtech.top/gtnbzjfloi.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.zhiwuduotai.top/gtffajexfe.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.tanke756.top/gtnekpcicy.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yuxming.cn/gtaetujuja.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.yanxiufei.cn/gtyglxegbu.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.gaohongyu789.top/gtdicqoruh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.yueranfly.top/gtrncjxqzc.html

================================================================================
来源：http://hz.meibo888.top/gtemupandi.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.zhijiandao.cn/gtffnrbsrh.html

================================================================================
来源：http://hz.nwbrower.top/gtbxupcggw.html

[Q01] 创建表
来源：http://hz.pengpengdd.cyou/gtphtcgwxg.html

CREATE TABLE users (
来源：http://hz.dashuyun.cn/gtucvlwgzm.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.aibaodan.cn/gtpwbsldfr.html

name VARCHAR(50) NOT NULL,
来源：http://hz.andypj.xyz/gtzuphitmg.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jqgufenzy.top/gtlgobtjsk.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.pycfn.com/gteamzlzca.html

);
来源：http://hz.cashguo.top/gtdcjynehw.html

[Q02] 创建带外键的表
来源：http://hz.xuanzx.com/gturbzjkmm.html

CREATE TABLE orders (
来源：http://hz.fzhhl.top/gtkbapifgv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.daxiang520.top/gtoyxkaohs.html

user_id INT NOT NULL,
来源：http://hz.shangyingyoupin.top/gtkervbzha.html

amount DECIMAL(10, 2),
来源：http://hz.xziqi.cn/gtstzxdvle.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.andypj.xyz/gtxalbttfm.html

);
来源：http://hz.gogol.net.cn/gtlljvzidf.html

[Q03] 增加列
来源：http://hz.nanxuanxn.top/gtkktoxacy.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.guannengcc.top/gtrfvhzafl.html

[Q04] 修改列类型
来源：http://hz.hfpthk.cn/gtdcnuknew.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.vqdsnc.cn/gtddqpjinj.html

[Q05] 重命名列
来源：http://hz.gogol.net.cn/gtwzbuwzrw.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.yj20258888.top/gtpdpmggdh.html

[Q06] 删除列
来源：http://hz.guannengcc.top/gtncbzsvpm.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.pycfn.com/gtnqwpfigx.html

[Q07] 删除表
来源：http://hz.zhijiandao.cn/gtjskpcyqy.html

DROP TABLE IF EXISTS orders;
来源：http://hz.nwbrower.top/gttxlcnvar.html

[Q08] 创建普通索引
来源：http://hz.yj202588.top/gtthntbzpt.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.haohaochexian.top/gtsnhvzkfy.html

[Q09] 创建唯一索引
来源：http://hz.tanke756.top/gtlnlxlstq.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.zhoulong.xyz/gtextxdrdq.html

[Q10] 插入单行
来源：http://hz.sysykeji.top/gtkmuoyazj.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.dianchejie.cn/gtitjuzhpn.html

[Q11] 一次插入多行
来源：http://hz.tianlin.xyz/gtmkwptbbs.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.jiagoushi.top/gtshiaxfwc.html

[Q12] 插入后取自增 ID
来源：http://hz.zdqjudy.top/gtypzqhsns.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yuanzhike.top/gttohuqwvt.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.guowangkeji.top/gtzbrxende.html

[Q13] 忽略重复插入
来源：http://hz.zhoulong.xyz/gtiqzqqjbt.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.fengsongda.top/gthtfpzvws.html

[Q14] 存在则更新（upsert）
来源：http://hz.c1oappe.top/gtynmntpgt.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.jianghu66.top/gtaofoxppt.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.cqqwz.cn/gtleedrvrp.html

[Q15] 查询全部
来源：http://hz.jianghu66.top/gtllygegpb.html

SELECT * FROM users;
来源：http://hz.nanxuanxn.top/gtqfxipske.html

[Q16] 查询指定列
来源：http://hz.zhoulong.xyz/gtoejlqvrq.html

SELECT id, name FROM users;
来源：http://hz.yueranfly.top/gtzqefynss.html

[Q17] 条件查询
来源：http://hz.daria6918.cn/gtqmoaawrx.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.yongpay.top/gtabecedqb.html

[Q18] 模糊匹配
来源：http://hz.snrcjt.cn/gtcqeofrzd.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.chenjidiqi.icu/gtfgjbsxvz.html

[Q19] 范围查询
来源：http://hz.svipenyu.cn/gtriisbcww.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.mhx1999.top/gtcvjhvooj.html

[Q20] IN 列表
来源：http://hz.bjfxy.top/gtnxcgbscy.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.xingfuxueyuan.xyz/gttvuxywvw.html

[Q21] 空值判断
来源：http://hz.cashguo.top/gttlnrhren.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.gogol.net.cn/gtqnzyqvee.html

[Q22] 排序
来源：http://hz.aibaodan.cn/gtcorqdqjc.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.zhoulong.xyz/gtyrbubflb.html

[Q23] 分页
来源：http://hz.mhx1999.top/gtbblnduix.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.smart0.xyz/gtwuzofcai.html

[Q24] 去重
来源：http://hz.yj20258.top/gtgpjgyspg.html

SELECT DISTINCT city FROM users;
来源：http://hz.dashuyun.cn/gtfxxpaifk.html

[Q25] 只取前 N 条
来源：http://hz.ywan-chungtsiang.top/gtownrseax.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.daxiang520.top/gtdmsgvczl.html

[Q26] 计数
来源：http://hz.sysykeji.top/gtggabyyge.html

SELECT COUNT(*) FROM users;
来源：http://hz.chenjidiqi.icu/gtjrlsnhec.html

[Q27] 条件计数
来源：http://hz.cashguo.top/gtamblthya.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.pycfn.com/gtatdvtzdy.html

[Q28] 求和与平均
来源：http://hz.jinqigufen.top/gtecxkpcql.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.zhixingplan.top/gtbxxeabkz.html

[Q29] 最大最小值
来源：http://hz.jqgfzy.top/gtbgyenqud.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.shuidangran.top/gtespdsgta.html

[Q30] 分组统计
来源：http://hz.quarkkingdee.top/gtcakdyylx.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.hywenlv.cn/gthsudodtg.html

[Q31] 分组后过滤
来源：http://hz.svipenyu.cn/gtiinsypnk.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.andypj.xyz/gtljfhxycb.html

[Q32] 分组拼接字符串
来源：http://hz.ybcxt.top/gtcbbastsb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.guowangkeji.top/gtuhcbdfzz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.daxiang520.top/gttpezhfkg.html

[Q33] 多列分组
来源：http://hz.smart0.xyz/gtfbenyieu.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.sweek.top/gtvlgrlqct.html

[Q34] 每组取第一条
来源：http://hz.gaohongyu789.top/gtvvhjrqzb.html

SELECT * FROM (
来源：http://hz.guowangkeji.top/gttepjudpz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jqgfzy.top/gtvaoojgue.html

) t WHERE rn = 1;
来源：http://hz.dashuyun.cn/gtecfibkdp.html

[Q35] 内连接
来源：http://hz.birdmap.top/gtqzbvooqh.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhiwuduotai.top/gtsexzwtcl.html

[Q36] 左连接
来源：http://hz.yj20258888.top/gtoviwcvox.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.cdnleiting.top/gtyuytxoyk.html

[Q37] 右连接
来源：http://hz.cashguo.top/gtkvsersmp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.cashguo.top/gtflqmquvz.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.jinqigufen.top/gtczixaeaa.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.0kj1m.cn/gtmluvoxxz.html

[Q39] 自连接（查上下级）
来源：http://hz.yangfankeji.com/gtxghqoaji.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.shzxlz.cn/gtamunanux.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.ydzc1.top/gtmddfafui.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.shzxlz.cn/gttvlkrsdu.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.shanyushiyangkeji.top/gtdrisiopp.html

[Q41] 多表连接
来源：http://hz.zycfv.cn/gtuoralfsy.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.zhongyouzk.top/gtuvxacgua.html

JOIN users u ON u.id = o.user_id
来源：http://hz.xziqi.cn/gtettpadfd.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.zhaomingkeji.xyz/gtzihlxfnz.html

[Q42] 连接条件附加过滤
来源：http://hz.meibo888.top/gtmtbcwjzz.html

SELECT u.name, o.amount FROM users u
来源：http://hz.hnqzz.top/gttpzebqkc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.9152youxi.cn/gtughdnhwo.html

[Q43] 标量子查询
来源：http://hz.shanyushiyangkeji.top/gtvekstelt.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.shangyingyoupin.top/gtmoexfujz.html

[Q44] IN 子查询
来源：http://hz.cdnleiting.top/gtwlbrkkqr.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.316326.xyz/gtesrvwspu.html

[Q45] EXISTS 判断存在
来源：http://hz.c1oappe.top/gtojsmdesd.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.birdmap.top/gttrznphfj.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.0kj1m.cn/gtapauyzdl.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhiwuduotai.top/gtmicifvav.html

[Q47] 与平均值比较
来源：http://hz.bjfxy.top/gthntezjhr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.nanxinkj.top/gtupadegud.html

[Q48] CTE 公用表表达式
来源：http://hz.shuidangran.top/gthhytnnkw.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.quarkkingdee.top/gtmrchwlat.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.nanxinkj.top/gtlgofnzvw.html

[Q49] 更新单行
来源：http://hz.yj20258.top/gtgcyzbqur.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.zhixingplan.top/gtsnfgqgsy.html

[Q50] 批量更新
来源：http://hz.kuanghao11.cn/gtidceqbfe.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.sysykeji.top/gtzqshdjcn.html

[Q51] 用子查询更新
来源：http://hz.yj20258888.top/gttrzqlfih.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.smart0.xyz/gtyeeictit.html

[Q52] 删除指定行
来源：http://hz.jinqigfzy.top/gtdmjexule.html

DELETE FROM users WHERE id = 10;
来源：http://hz.ppjwa.cn/gtnfthaylm.html

[Q53] 按条件删除
来源：http://hz.daxiang520.top/gthmyfqhnv.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.chenjidiqi.icu/gtmrwltgne.html

[Q54] 清空表
来源：http://hz.havefunace.top/gtrapfdxnz.html

TRUNCATE TABLE logs;
来源：http://hz.ybcxt.top/gtvnoftzym.html

[Q55] 排名（并列占位）
来源：http://hz.hnxiangtu.top/gtiuhljrdx.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.shanyushiyangtech.top/gtrtdniyof.html

[Q56] 密集排名（并列不占位）
来源：http://hz.xuanzx.com/gttzfrrfwv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.andypj.xyz/gtcnukklff.html

[Q57] 行号
来源：http://hz.ybcxt.top/gtlyeuibjx.html


<!-- 参考信息 -->