代发 wailian999

[N09] 栈与队列
来源：http://hz.ydzc1.top/gtqojnnprh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.mhx1999.top/gteanpfdkz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.feifeiyinyue.top/gtfurtjzpo.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.cucudq.cn/gtgquxpbvr.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.fengsongda.top/gtifrrrumz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.shuidangran.top/gtdywyutle.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.cqqwz.cn/gtttcfvfzb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.cucudq.cn/gtgcriwxiv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.aizwys.cn/gtwfgdbdnt.html

[N10] 链表节点定义
来源：http://hz.jqgfzy.top/gtnupwftwp.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yj20258.top/gtchntiuxd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.yj20258888.top/gtvbrvywua.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.meibo888.top/gtinwrmvyh.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.dianchejie.cn/gtizprwybp.html

Java: class Node { int v; Node next; }
来源：http://hz.cashguo.top/gtmorowgcx.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.zhengqikj.top/gtlzduizxh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.xingfuxueyuan.xyz/gtgqzyydiv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.jlsjyb.cn/gtapxqzwao.html

[N11] 二叉树中序遍历
来源：http://hz.nanxinkj.top/gtvozazpwm.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.shzxlz.cn/gtwnelkrqp.html

PHP:  // 手写递归函数
来源：http://hz.shuidangran.top/gtlfigafbi.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhixingplan.top/gtzvbrwyph.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.xingfuxueyuan.xyz/gtgnbpkoyt.html

Java: // 手写递归
来源：http://hz.tianlin.xyz/gtztgdnyxb.html

Go:   // 手写递归
来源：http://hz.yj20258888.top/gtwcrkndla.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.gaohongyu789.top/gthlktatsx.html

C#:   // 手写递归
来源：http://hz.gzhubu.top/gttpahrulo.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.hnqzz.top/gtimlwnsfk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.yj20258.top/gttdqpjbqr.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.aibaodan.cn/gtscfirlst.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.nanxinkj.top/gtvvgpsxmq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.feifeiyinyue.top/gtlhkgtfmi.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ivvv.top/gtcpquwyjm.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.ywan-chungtsiang.top/gtybjyutht.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.cheryme.top/gtvasqvjqy.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.sysykeji.top/gtmwrveusd.html

================================================================================
来源：http://hz.9152youxi.cn/gtexjlcoox.html

O. 并发与异步
来源：http://hz.haohaochexian.top/gtkqeupgpd.html

================================================================================
来源：http://hz.birdmap.top/gtyjepaqpa.html

[O01] 启动一个线程
来源：http://hz.9152youxi.cn/gtttuzdoif.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.daria6918.cn/gtfzomuoid.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.jinyuanbaomall.cn/gtufmmldgb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.gzhubu.top/gtzhuyeelm.html

TS:   // 同 JS
来源：http://hz.xuanzx.com/gtannakrqu.html

Java: new Thread(() -> f()).start()
来源：http://hz.yvedp.cn/gtxnjpyqod.html

Go:   go f()
来源：http://hz.daria6918.cn/gtvesboyxy.html

Ruby: Thread.new { f }
来源：http://hz.c1oappe.top/gtwxjtuwtt.html

C#:   Task.Run(() => F());
来源：http://hz.shangyingyoupin.top/gtjqhbkrbo.html

[O02] 使用线程池
来源：http://hz.hammf.cn/gtkakirxbv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.xinyue.icu/gtzvubpbuw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.nwbrower.top/gtdrkmrafe.html

JS:   // worker_threads 线程池
来源：http://hz.ybcxt.top/gtqmjohona.html

TS:   // worker_threads 线程池
来源：http://hz.hysaishi.cn/gtrycqbnom.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.svipenyu.cn/gtcucpdvej.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.daria6918.cn/gtugrpsfis.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.wangdashe.top/gtlwhahkdz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.ywan-chungtsiang.top/gthxqimagv.html

[O03] 加锁保护共享数据
来源：http://hz.tanke756.top/gtblweecde.html

Py:   with lock: shared += 1
来源：http://hz.52xcode.cn/gtktdduqfx.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.jlsjyb.cn/gtanrcrkwl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.hywenlv.cn/gtvefbjdlo.html

TS:   // 同 JS
来源：http://hz.ywan-chungtsiang.top/gtonkwpaez.html

Java: synchronized (this) { shared++; }
来源：http://hz.jlsjyb.cn/gtztqyooso.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.shanyushiyangtech.top/gtnixruwtr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.ivvv.top/gtdedjwowf.html

C#:   lock (gate) { shared++; }
来源：http://hz.tianlin.xyz/gtpbvqjrdd.html

[O04] 定义异步函数并等待
来源：http://hz.c1oappe.top/gttkxfbcjj.html

Py:   async def f():⏎    await g()
来源：http://hz.yueranfly.top/gteuiwyiuh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.daxiang520.top/gtmaoqeitj.html

JS:   async function f() { await g(); }
来源：http://hz.yonumen.top/gtkzremgkb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.zycfv.cn/gtigrxfwip.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.yangfankeji.com/gthvmczngp.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.andypj.xyz/gtfamqimai.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.redwolf501.top/gtgumdtdbi.html

C#:   async Task F() { await G(); }
来源：http://hz.cashguo.top/gtjjkabxmm.html

[O05] 并发执行并等待全部完成
来源：http://hz.gzhubu.top/gtztdoyyvi.html

Py:   asyncio.gather(*tasks)
来源：http://hz.chenlongwang.top/gtgskicsaw.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.mhx1999.top/gthpkzdolq.html

JS:   await Promise.all(tasks)
来源：http://hz.yj202588.top/gtbkmatbzb.html

TS:   await Promise.all(tasks)
来源：http://hz.yueranfly.top/gtspufzinm.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.iojbl.cn/gtnjxxdjhs.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.guannengcc.top/gtsoktbwll.html

Ruby: threads.map(&:join)
来源：http://hz.guowangkeji.top/gtrcuwotrm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.bjfxy.top/gtcqkwbqud.html

[O06] 使用进程池
来源：http://hz.yangfankeji.com/gtgooshbgy.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.daxiang520.top/gtzonczlzl.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.yj20258888.top/gtvnlcmgeh.html

JS:   // child_process / cluster 模块
来源：http://hz.chenzaomai.com/gtbjneelct.html

TS:   // child_process / cluster 模块
来源：http://hz.ydjk.org.cn/gtuuodphel.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jqgfzy.top/gtxugutbih.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.yvedp.cn/gtsaztygga.html

Ruby: // fork 块
来源：http://hz.svipenyu.cn/gtpvmwjfvn.html

C#:   Parallel.For
来源：http://hz.hnxiangtu.top/gtuhovznqy.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtelrahudf.html

P. 常用工具函数
来源：http://hz.jinqigufen.top/gtxfgstdcz.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtfgllppei.html

[P01] 生成 UUID
来源：http://hz.316326.xyz/gtruclgzxh.html

Py:   str(uuid.uuid4())
来源：http://hz.ydzc1.top/gtpcncusjo.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.zhixingplan.top/gtsxcendhe.html

JS:   crypto.randomUUID()
来源：http://hz.xingfuxueyuan.xyz/gtvkrmgwef.html

TS:   crypto.randomUUID()
来源：http://hz.jqgufenzy.top/gteggdqbps.html

Java: UUID.randomUUID().toString()
来源：http://hz.svipenyu.cn/gtkajttqsl.html

Go:   // 用 github.com/google/uuid
来源：http://hz.jinqigufen.top/gtvhsltkff.html

Ruby: SecureRandom.uuid
来源：http://hz.dianchejie.cn/gtociyltlq.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.shanyushiyangtech.top/gtorafadum.html

[P02] MD5 / SHA256 摘要
来源：http://hz.wangdashe.top/gtazjjdqas.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.snrcjt.cn/gtukvfylnj.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.guannengcc.top/gtehbgnyvj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.zhijiandao.cn/gtfbojiake.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.hnqzz.top/gtpughpbgt.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.gzhubu.top/gtzlgngevp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.guowangkeji.top/gtbzgyrmcu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.xuanzx.com/gtrmhexxpf.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.jinyuanbaomall.cn/gtxfhokpbm.html

[P03] 生成短随机字符串
来源：http://hz.yueranfly.top/gtwsubhfny.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.shangyingyoupin.top/gthxgxhskq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.cashguo.top/gtefxnbnxk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yonumen.top/gtesjgkrpp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jqgufenzy.top/gtorlrmnjm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.quarkkingdee.top/gtqmejhbhs.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.hnxiangtu.top/gtchtqwwsp.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.xylfe.cn/gtmhmlhcvg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jinghuilouyu.cn/gtbxuapoks.html

[P04] 求长度
来源：http://hz.dashuyun.cn/gtvurdkhwx.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.sysykeji.top/gtspdmqsty.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yj202588.top/gtjulqzkua.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ehwqpu.com/gthajaiuph.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zycfv.cn/gtvmjjwwta.html

Java: list.size();  map.size();  s.length()
来源：http://hz.snrcjt.cn/gtzqxoblyf.html

Go:   len(arr);  len(m)
来源：http://hz.yonumen.top/gtvqpyaeqc.html

Ruby: x.length;  x.size
来源：http://hz.yj20258.top/gtwphbnrsj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.chenlongwang.top/gtmhrijipv.html

[P05] 判断两个对象内容是否相等
来源：http://hz.aizwys.cn/gteoaxaifj.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.yj20258.top/gtpnavmttc.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.zhoulong.xyz/gtqpzvgqns.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.jqgfzy.top/gtzmqxurcq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.tianlin.xyz/gtrdcprgqp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.yj202588.top/gtcwplywfx.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.vqdsnc.cn/gtpedrmasc.html

Ruby: a == b
来源：http://hz.sysykeji.top/gtagbwtbow.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.tianlin.xyz/gtoptqxanw.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.sxryk.cn/gtbneoevri.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.nwbrower.top/gtizbbpiuc.html

PHP:  if (empty($x)) {}
来源：http://hz.cheryme.top/gtvquugmxk.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.wangdashe.top/gtuqvgtoly.html

TS:   if (x == null) {}
来源：http://hz.jlsjyb.cn/gtagvsbaea.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.ivvv.top/gtebrnxmhd.html

Go:   if x == nil {}
来源：http://hz.nanxuanxn.top/gthgglzoan.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.shanyushiyangkeji.top/gtmedjhkwx.html

C#:   if (x is null) {}
来源：http://hz.yangfankeji.com/gtrqehbdlx.html

[P07] 防抖与节流
来源：http://hz.pycfn.com/gterautnjp.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.c1oappe.top/gtkejaltht.html

PHP:  // 手写时间戳比较
来源：http://hz.yonumen.top/gtmfccnhcj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.gaohongyu789.top/gtwfmlosyo.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shzxlz.cn/gtifbezknr.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.sysykeji.top/gtpffttfwi.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.cheryme.top/gtdropvsvg.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.sufxvd.cn/gtkaujzlmk.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.yuanzhike.top/gtnpszskbo.html

[P08] 处理浮点精度问题
来源：http://hz.nwbrower.top/gtzcttnxad.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jinqigufen.top/gthdxwaecg.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.redwolf501.top/gtvyaggxac.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.quarkkingdee.top/gtvhvdwtck.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.ehwqpu.com/gtjoysvsbz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.guannengcc.top/gtosdxguvb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.sweek.top/gthiukqhty.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.tanke756.top/gtwwcrlarh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.yj20258.top/gtmkxhdtuf.html

================================================================================
来源：http://hz.svipenyu.cn/gtdbjsryig.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.zhiwuduotai.top/gtnetamibg.html

================================================================================
来源：http://hz.ybcxt.top/gtjxjkoisv.html

[Q01] 创建表
来源：http://hz.yueranfly.top/gtthyfqayf.html

CREATE TABLE users (
来源：http://hz.wangdashe.top/gtdoszywrt.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xuetiantiany.cn/gtsgiumjvl.html

name VARCHAR(50) NOT NULL,
来源：http://hz.quarkkingdee.top/gtrwjatsjx.html

email VARCHAR(100) UNIQUE,
来源：http://hz.aibaodan.cn/gtnvdvpvhw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.daria6918.cn/gtnqqmceap.html

);
来源：http://hz.yangfankeji.com/gtjudjuoqr.html

[Q02] 创建带外键的表
来源：http://hz.andypj.xyz/gtbwoarshc.html

CREATE TABLE orders (
来源：http://hz.yongpay.top/gtiewxntno.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jinghuilouyu.cn/gtefumcjhv.html

user_id INT NOT NULL,
来源：http://hz.sysykeji.top/gtpvsvxgwb.html

amount DECIMAL(10, 2),
来源：http://hz.tanke756.top/gtzehqxilm.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.yuxming.cn/gtkdficjwo.html

);
来源：http://hz.chenjidiqi.icu/gtfbvnouav.html

[Q03] 增加列
来源：http://hz.zycfv.cn/gtqfoinnso.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.hnqzz.top/gtxlvpfadx.html

[Q04] 修改列类型
来源：http://hz.bjfxy.top/gtewxeqcyn.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.cdnleiting.top/gthpbsgtux.html

[Q05] 重命名列
来源：http://hz.daxiang520.top/gtnqbmxmfr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.jinqigfzy.top/gtlqganipr.html

[Q06] 删除列
来源：http://hz.chenjidiqi.icu/gtdrlpaovj.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.chenjidiqi.icu/gtocsnudtb.html

[Q07] 删除表
来源：http://hz.zhixingplan.top/gthdokitgn.html

DROP TABLE IF EXISTS orders;
来源：http://hz.tanke756.top/gtysobtyjv.html

[Q08] 创建普通索引
来源：http://hz.nwbrower.top/gtnclpoode.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.aibaodan.cn/gtqcvxkowd.html

[Q09] 创建唯一索引
来源：http://hz.meibo888.top/gtucbpqlgq.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.meibo888.top/gtxmhpvayq.html

[Q10] 插入单行
来源：http://hz.svipenyu.cn/gtlmgoraod.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.shuidangran.top/gtyvrtxrez.html

[Q11] 一次插入多行
来源：http://hz.zhiwuduotai.top/gtbrmdnfxi.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.jqgufenzy.top/gtdjnyzpjl.html

[Q12] 插入后取自增 ID
来源：http://hz.sysykeji.top/gtanmrrlbw.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.jiagoushi.top/gtwnoogdsi.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yvedp.cn/gtqhlgvwmj.html

[Q13] 忽略重复插入
来源：http://hz.birdmap.top/gtepcwaemt.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.shanyushiyangtech.top/gtoaovkqkm.html

[Q14] 存在则更新（upsert）
来源：http://hz.zhongyouzk.top/gtiqsxorwt.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.yj20258888.top/gtsxlkacbe.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.vqdsnc.cn/gtwozepwxz.html

[Q15] 查询全部
来源：http://hz.jlsjyb.cn/gtlycpeppe.html

SELECT * FROM users;
来源：http://hz.gotoacloud.top/gtnsnoejga.html

[Q16] 查询指定列
来源：http://hz.yuanzhike.top/gtyhdxhdlu.html

SELECT id, name FROM users;
来源：http://hz.hammf.cn/gtcvecbgse.html

[Q17] 条件查询
来源：http://hz.cucudq.cn/gtlipszotg.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.cqqwz.cn/gtqnegugcd.html

[Q18] 模糊匹配
来源：http://hz.hysaishi.cn/gtxbhqjpzu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.havefunace.top/gtjzkxmlhi.html

[Q19] 范围查询
来源：http://hz.xingfuxueyuan.xyz/gtccqzeupp.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.kuanghao11.cn/gtcymgntta.html

[Q20] IN 列表
来源：http://hz.xuanzx.com/gtdchciwlb.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yangfankeji.com/gtgdrlvngc.html

[Q21] 空值判断
来源：http://hz.feifeiyinyue.top/gthhywpimx.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.shanyushiyangkeji.top/gtfbzubfvq.html

[Q22] 排序
来源：http://hz.shuidangran.top/gtpzepjvvy.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.chenjidiqi.icu/gtbkqtzinx.html

[Q23] 分页
来源：http://hz.yj202588.top/gtorzmbyya.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yj20258.top/gtfuxilzjh.html

[Q24] 去重
来源：http://hz.haohaochexian.top/gtggfmxrde.html

SELECT DISTINCT city FROM users;
来源：http://hz.nanxinkj.top/gtzzcqoozj.html

[Q25] 只取前 N 条
来源：http://hz.daxiang520.top/gtrwfnrsyl.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.gotoacloud.top/gtumjidoof.html

[Q26] 计数
来源：http://hz.zdqjudy.top/gtawaosxgh.html

SELECT COUNT(*) FROM users;
来源：http://hz.sxryk.cn/gtdxirmycw.html

[Q27] 条件计数
来源：http://hz.0kj1m.cn/gtdvvuskry.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yj20258888.top/gtdtccjqag.html

[Q28] 求和与平均
来源：http://hz.yuxming.cn/gtglrxmqvu.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.shanyushiyangkeji.top/gtdgkpktwr.html

[Q29] 最大最小值
来源：http://hz.tanke756.top/gtzcbxhowh.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.tanke756.top/gttkaxemli.html

[Q30] 分组统计
来源：http://hz.xuetiantiany.cn/gtaqnmklvn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.dianchejie.cn/gtbmghkvwp.html

[Q31] 分组后过滤
来源：http://hz.haohaochexian.top/gtagmkuokb.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.sweek.top/gtjtmfjprm.html

[Q32] 分组拼接字符串
来源：http://hz.zycfv.cn/gtllpgocca.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.havefunace.top/gteguaumii.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.ydjk.org.cn/gttcbgvdhv.html

[Q33] 多列分组
来源：http://hz.316326.xyz/gtgzpzxetn.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.fengsongda.top/gtlpecdlcz.html

[Q34] 每组取第一条
来源：http://hz.aizwys.cn/gtdkcgfnae.html

SELECT * FROM (
来源：http://hz.c1oappe.top/gtoiapftxi.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.nwbrower.top/gtzuclubxu.html

) t WHERE rn = 1;
来源：http://hz.xinyue.icu/gtqfenntfu.html

[Q35] 内连接
来源：http://hz.ydzc1.top/gtwzvtmmrv.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhoulong.xyz/gtxmbuccrd.html

[Q36] 左连接
来源：http://hz.hysaishi.cn/gtwyefnuug.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.dashuyun.cn/gttyvhutuc.html

[Q37] 右连接
来源：http://hz.zhoulong.xyz/gtwrjaizxu.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.iojbl.cn/gtsoyynypt.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.yj202588.top/gtexmsdpnu.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.c1oappe.top/gtgubvljgi.html

[Q39] 自连接（查上下级）
来源：http://hz.guowangkeji.top/gtypyhvwch.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.meibo888.top/gtgkonenmx.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.dianchejie.cn/gtneaznyuy.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.tianlin.xyz/gteusgbyce.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.nanxinkj.top/gtxxngdfzz.html

[Q41] 多表连接
来源：http://hz.gaohongyu789.top/gtbntjjfil.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.zhongyouzk.top/gtbwpqyxag.html

JOIN users u ON u.id = o.user_id
来源：http://hz.c1oappe.top/gtqsopkrrk.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.ydjk.org.cn/gtxjalssms.html

[Q42] 连接条件附加过滤
来源：http://hz.zhaomingkeji.xyz/gtpvgpfwnj.html

SELECT u.name, o.amount FROM users u
来源：http://hz.svipenyu.cn/gtmyqktgbr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.hfpthk.cn/gtfuzqxlbc.html

[Q43] 标量子查询
来源：http://hz.jinqigufen.top/gtrbwsnfgn.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.shuidangran.top/gtrpgynumh.html

[Q44] IN 子查询
来源：http://hz.jqgufenzy.top/gtfcpmbilm.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.ivvv.top/gtvajkihuh.html

[Q45] EXISTS 判断存在
来源：http://hz.xuanzx.com/gtiloncwlw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.ydjk.org.cn/gtmurafzau.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.zhijiandao.cn/gtytiyzobc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.ivvv.top/gtteyiwnnk.html

[Q47] 与平均值比较
来源：http://hz.yvedp.cn/gtjjwlcufb.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jinqigufen.top/gtafcovgrj.html

[Q48] CTE 公用表表达式
来源：http://hz.316326.xyz/gtpjjctusr.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jinyuanbaomall.cn/gtimzoesgx.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.guowangkeji.top/gtqmrzfuyn.html

[Q49] 更新单行
来源：http://hz.andypj.xyz/gtwaxsamsv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yongpay.top/gtmvpnider.html

[Q50] 批量更新
来源：http://hz.yueranfly.top/gtkjsqcixk.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zhoulong.xyz/gtnepydpok.html

[Q51] 用子查询更新
来源：http://hz.chenlongwang.top/gtjpqpfzbu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.nanxuanxn.top/gtosttvgsx.html

[Q52] 删除指定行
来源：http://hz.wangdashe.top/gtwcvhwmez.html

DELETE FROM users WHERE id = 10;
来源：http://hz.xuanzx.com/gthdeirffa.html

[Q53] 按条件删除
来源：http://hz.havefunace.top/gtuahkksmq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.haohaochexian.top/gtbwplonxe.html

[Q54] 清空表
来源：http://hz.tian-w.cn/gtccdngemm.html

TRUNCATE TABLE logs;
来源：http://hz.jqgfzy.top/gtjtuconbc.html

[Q55] 排名（并列占位）
来源：http://hz.ppjwa.cn/gtaxbermyb.html


<!-- 参考信息 -->