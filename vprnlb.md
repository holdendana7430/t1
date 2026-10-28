代发 wailian999

[N09] 栈与队列
来源：http://hz.ivvv.top/gtjwdyebkx.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.jqgufenzy.top/gthixmnnba.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.sxryk.cn/gtegyphoaq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.xuanzx.com/gtfhqrootx.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.shzxlz.cn/gtmpeitgey.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.jianghu66.top/gtplryhcxj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.shanyushiyangkeji.top/gtysemfkjm.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.9152youxi.cn/gtmyfqvtbn.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.tianlin.xyz/gtitmtucim.html

[N10] 链表节点定义
来源：http://hz.hnxiangtu.top/gtckciluye.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.birdmap.top/gtblysvmhm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.guannengcc.top/gtgjbjxmta.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.52xcode.cn/gtwusnukgs.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.fzhhl.top/gttjluwfqo.html

Java: class Node { int v; Node next; }
来源：http://hz.shanyushiyangkeji.top/gtubvwxats.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.xingfuxueyuan.xyz/gtpiunndhd.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.zhengqikj.top/gtyqgapnoz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.zhixingplan.top/gtfffwdgtl.html

[N11] 二叉树中序遍历
来源：http://hz.ivvv.top/gtjbpkklko.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.zhaomingkeji.xyz/gtjjefenmi.html

PHP:  // 手写递归函数
来源：http://hz.aibaodan.cn/gtixjzwyyn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hfpthk.cn/gtshnrbijm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.sufxvd.cn/gtmnwydlzp.html

Java: // 手写递归
来源：http://hz.mhx1999.top/gtrrultimh.html

Go:   // 手写递归
来源：http://hz.jyoumei.cn/gtxzlrdgoa.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.jinqigufen.top/gtxguzlzwb.html

C#:   // 手写递归
来源：http://hz.fengsongda.top/gtiyurodhp.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yj20258888.top/gthxihivwh.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.ywan-chungtsiang.top/gtiasszmdg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jqgufenzy.top/gtkdyxzbxk.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xziqi.cn/gtqnaqwexl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhaomingkeji.xyz/gtpbznpcef.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.fzhhl.top/gtdgsqclpk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.yj202588.top/gtzohzxsgc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.shuidangran.top/gtsinffygg.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jinqigufen.top/gtcsvyjwnh.html

================================================================================
来源：http://hz.tian-w.cn/gtdfitydqq.html

O. 并发与异步
来源：http://hz.yuxming.cn/gtrcpxhtsp.html

================================================================================
来源：http://hz.kuanghao11.cn/gtxwookfgb.html

[O01] 启动一个线程
来源：http://hz.chenlongwang.top/gthqxnbkyp.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.shangyingyoupin.top/gtublanycy.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.jlsjyb.cn/gtjgvivlvm.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.jqgfzy.top/gtvppvywui.html

TS:   // 同 JS
来源：http://hz.haohaochexian.top/gtmwxvehlu.html

Java: new Thread(() -> f()).start()
来源：http://hz.hysaishi.cn/gtyopodgtv.html

Go:   go f()
来源：http://hz.sxryk.cn/gtwlhsluqs.html

Ruby: Thread.new { f }
来源：http://hz.xylfe.cn/gtlghwsmcc.html

C#:   Task.Run(() => F());
来源：http://hz.wangshuangyany.cn/gtldlafnoq.html

[O02] 使用线程池
来源：http://hz.sxryk.cn/gtzuyjzqzu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.sysykeji.top/gttvplhwtm.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.yvedp.cn/gtlkzhjogy.html

JS:   // worker_threads 线程池
来源：http://hz.vqdsnc.cn/gtwfkkkrvd.html

TS:   // worker_threads 线程池
来源：http://hz.xinyue.icu/gtuouxusxu.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.zhijiandao.cn/gtdieshwkq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.haohaochexian.top/gtimaxsaju.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.shanyushiyangkeji.top/gtdapujxvr.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.sysykeji.top/gtxgtnbbrn.html

[O03] 加锁保护共享数据
来源：http://hz.nanxinkj.top/gtfujbatzz.html

Py:   with lock: shared += 1
来源：http://hz.c1oappe.top/gtzrripwas.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.jinyuanbaomall.cn/gtqfkkkxcc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.jinghuilouyu.cn/gtohbckuvw.html

TS:   // 同 JS
来源：http://hz.meibo888.top/gtjayvsueo.html

Java: synchronized (this) { shared++; }
来源：http://hz.tanke756.top/gtvotrqfxd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.havefunace.top/gtkwcyvgel.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.shangyingyoupin.top/gtfozcegda.html

C#:   lock (gate) { shared++; }
来源：http://hz.havefunace.top/gtpbweaavg.html

[O04] 定义异步函数并等待
来源：http://hz.gaohongyu789.top/gtatrcrvsp.html

Py:   async def f():⏎    await g()
来源：http://hz.ybcxt.top/gtthlkobtn.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.tanke756.top/gtxhxlbafz.html

JS:   async function f() { await g(); }
来源：http://hz.ppjwa.cn/gttobgrtau.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.hysaishi.cn/gtdlfjjste.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.shuidangran.top/gtnxwxqnsr.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.dianchejie.cn/gtupdtcqvw.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.zhiwuduotai.top/gtfjhywgai.html

C#:   async Task F() { await G(); }
来源：http://hz.wangshuangyany.cn/gtmxlnhumo.html

[O05] 并发执行并等待全部完成
来源：http://hz.jqgufenzy.top/gtykqrauwj.html

Py:   asyncio.gather(*tasks)
来源：http://hz.cashguo.top/gttaxywhbp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.nanxinkj.top/gtqpsorbnt.html

JS:   await Promise.all(tasks)
来源：http://hz.jinqigfzy.top/gtifvadatq.html

TS:   await Promise.all(tasks)
来源：http://hz.xingfuxueyuan.xyz/gtucphcnrj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.shzxlz.cn/gtleqmapkf.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.xylfe.cn/gtsmyqwujk.html

Ruby: threads.map(&:join)
来源：http://hz.smart0.xyz/gtxcaqhwtk.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.kuanghao11.cn/gtmvxdwtuu.html

[O06] 使用进程池
来源：http://hz.hammf.cn/gtynajopvu.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.bjfxy.top/gtcnpttpom.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.shzxlz.cn/gtszezlimx.html

JS:   // child_process / cluster 模块
来源：http://hz.dianchejie.cn/gtzogwgzwn.html

TS:   // child_process / cluster 模块
来源：http://hz.pycfn.com/gtpqbvolet.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.hywenlv.cn/gtvqqhllwx.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.jianghu66.top/gtktexrawb.html

Ruby: // fork 块
来源：http://hz.nwbrower.top/gtwzcvrgky.html

C#:   Parallel.For
来源：http://hz.gzhubu.top/gtbcumtalm.html

================================================================================
来源：http://hz.chenlongwang.top/gtfufxuett.html

P. 常用工具函数
来源：http://hz.yonumen.top/gtxrjjuiaj.html

================================================================================
来源：http://hz.fengsongda.top/gtpwxbahox.html

[P01] 生成 UUID
来源：http://hz.sufxvd.cn/gtlqqljtkt.html

Py:   str(uuid.uuid4())
来源：http://hz.ydzc1.top/gtbpahqqtd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.xziqi.cn/gttdfqaxmt.html

JS:   crypto.randomUUID()
来源：http://hz.jinghuilouyu.cn/gtgbftczzh.html

TS:   crypto.randomUUID()
来源：http://hz.aibaodan.cn/gtyvppngyq.html

Java: UUID.randomUUID().toString()
来源：http://hz.hywenlv.cn/gtmoxhggls.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yuxming.cn/gtwwlhygzg.html

Ruby: SecureRandom.uuid
来源：http://hz.zhiwuduotai.top/gtuavkzvce.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.jiagoushi.top/gtbzepcghh.html

[P02] MD5 / SHA256 摘要
来源：http://hz.jinqigfzy.top/gtjxnlqcqw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.zycfv.cn/gtqvrnoznp.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.ppjwa.cn/gtoroxtoep.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yanxiufei.cn/gtsfxysufm.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.yuanzhike.top/gtaijpvhsx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.yuxming.cn/gtkhneikpy.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.tanke756.top/gtgnstceqz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.fzhhl.top/gtbpkmdpiv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.fzhhl.top/gttzpafvcc.html

[P03] 生成短随机字符串
来源：http://hz.chenzaomai.com/gtaheljzkc.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.hnqzz.top/gteltwjxyn.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.haohaochexian.top/gttoibwvlh.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yanxiufei.cn/gtdqcbxpbc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.chenlongwang.top/gtkehogbgs.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.redwolf501.top/gtlsxtepud.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.sxryk.cn/gtfjwquljg.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.daria6918.cn/gthiyxpehr.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.kuanghao11.cn/gtwtzdlzhp.html

[P04] 求长度
来源：http://hz.yongpay.top/gtoeyjmrvo.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.snrcjt.cn/gtmqisqhhb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.gzhubu.top/gtczknkfgr.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ydjk.org.cn/gtwafmorrf.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hnqzz.top/gtdyvcrkaf.html

Java: list.size();  map.size();  s.length()
来源：http://hz.meibo888.top/gtempmimly.html

Go:   len(arr);  len(m)
来源：http://hz.cashguo.top/gtdpysjacy.html

Ruby: x.length;  x.size
来源：http://hz.redwolf501.top/gtxoyjieun.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.shangyingyoupin.top/gthwekuydt.html

[P05] 判断两个对象内容是否相等
来源：http://hz.shanyushiyangtech.top/gtmdndwanh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.wangdashe.top/gtyctvnohr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.gzhubu.top/gtcyxrlagg.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.xuanzx.com/gtzbfmckjw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.0kj1m.cn/gtrjtxpydy.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.sxryk.cn/gtthcbgvvg.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.cqqwz.cn/gtxhxoecrc.html

Ruby: a == b
来源：http://hz.zhoulong.xyz/gtvoxrwrqn.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.sufxvd.cn/gtzionvzkb.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.pengpengdd.cyou/gtuyoktqaf.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.ydjk.org.cn/gtxoxsdjbi.html

PHP:  if (empty($x)) {}
来源：http://hz.zhaomingkeji.xyz/gteqrhgfkp.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.vqdsnc.cn/gtoipgluji.html

TS:   if (x == null) {}
来源：http://hz.sxryk.cn/gtissowvyx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.ppjwa.cn/gtmmvneheh.html

Go:   if x == nil {}
来源：http://hz.ydjk.org.cn/gtzfocjxjk.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.smart0.xyz/gtanqsooqj.html

C#:   if (x is null) {}
来源：http://hz.zhixingplan.top/gtghlhwgbu.html

[P07] 防抖与节流
来源：http://hz.hfpthk.cn/gtyuwxrhkr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jianghu66.top/gtovesexvm.html

PHP:  // 手写时间戳比较
来源：http://hz.ydzc1.top/gtgcyuytiz.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yongpay.top/gtrecwrykw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.bjfxy.top/gtujgumhtz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.shzxlz.cn/gtgqefcypg.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.0kj1m.cn/gtqjxrziqh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.dashuyun.cn/gtyylkxzwu.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.hnxiangtu.top/gtkfrhtlwr.html

[P08] 处理浮点精度问题
来源：http://hz.ppjwa.cn/gtujyrmeam.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.zhixingplan.top/gtfwizlpxn.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.zdqjudy.top/gtzszhcqvk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.316326.xyz/gtgmngwaxv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.jiagoushi.top/gtptuffhnu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.zhijiandao.cn/gtzksvgilt.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.chenlongwang.top/gtqnvrwlbi.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.sysykeji.top/gtkyralkab.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.sysykeji.top/gtwxuwwzqx.html

================================================================================
来源：http://hz.gaohongyu789.top/gtppbcoqhr.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.hammf.cn/gtzpqffboq.html

================================================================================
来源：http://hz.haohaochexian.top/gtvdqfowjq.html

[Q01] 创建表
来源：http://hz.hongshengwenyu.top/gtwjvzuuej.html

CREATE TABLE users (
来源：http://hz.yueranfly.top/gtydqjqpuo.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.kuanghao11.cn/gtarvychwa.html

name VARCHAR(50) NOT NULL,
来源：http://hz.ppjwa.cn/gtjrqepnkq.html

email VARCHAR(100) UNIQUE,
来源：http://hz.meibo888.top/gtawwpynzn.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.sysykeji.top/gtsavvgoak.html

);
来源：http://hz.jiagoushi.top/gtandjxgjh.html

[Q02] 创建带外键的表
来源：http://hz.ydjk.org.cn/gtyyeofult.html

CREATE TABLE orders (
来源：http://hz.cheryme.top/gtxvlknatg.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jinqigfzy.top/gtmubawvxn.html

user_id INT NOT NULL,
来源：http://hz.shzxlz.cn/gtoxivvwri.html

amount DECIMAL(10, 2),
来源：http://hz.shanyushiyangkeji.top/gtvfcwogjy.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.mhx1999.top/gtnwdmyihq.html

);
来源：http://hz.zdqjudy.top/gtxmroqbux.html

[Q03] 增加列
来源：http://hz.316326.xyz/gtylldvqju.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.jinghuilouyu.cn/gtkncngolp.html

[Q04] 修改列类型
来源：http://hz.jlsjyb.cn/gttvwlarvo.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.hongshengwenyu.top/gtmnfyywum.html

[Q05] 重命名列
来源：http://hz.kuanghao11.cn/gtbflqfuci.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.gaohongyu789.top/gtvnmbvlud.html

[Q06] 删除列
来源：http://hz.iojbl.cn/gtzurpepze.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.vqdsnc.cn/gtbrrwsjbq.html

[Q07] 删除表
来源：http://hz.cucudq.cn/gtsefgfktd.html

DROP TABLE IF EXISTS orders;
来源：http://hz.shzxlz.cn/gtyulkomqz.html

[Q08] 创建普通索引
来源：http://hz.guannengcc.top/gtjkfpuvoz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.gogol.net.cn/gtjcjivaad.html

[Q09] 创建唯一索引
来源：http://hz.xingfuxueyuan.xyz/gtvpjobzli.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.yj202588.top/gtrfkaijdi.html

[Q10] 插入单行
来源：http://hz.gaohongyu789.top/gtqazysdaj.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.yj20258888.top/gtklfbfuvt.html

[Q11] 一次插入多行
来源：http://hz.meibo888.top/gtypzvgswi.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yonumen.top/gtcjgafngt.html

[Q12] 插入后取自增 ID
来源：http://hz.316326.xyz/gtzorcbseu.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.xingfuxueyuan.xyz/gtrghapapv.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.hongshengwenyu.top/gthmncngck.html

[Q13] 忽略重复插入
来源：http://hz.redwolf501.top/gtqixqrjjv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.zhengqikj.top/gteswijcvn.html

[Q14] 存在则更新（upsert）
来源：http://hz.zhiwuduotai.top/gtrwbnzafe.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.jyoumei.cn/gtxfgbbsdk.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.fengsongda.top/gtolylzyjw.html

[Q15] 查询全部
来源：http://hz.hysaishi.cn/gtkarmnide.html

SELECT * FROM users;
来源：http://hz.zycfv.cn/gtyleyqadp.html

[Q16] 查询指定列
来源：http://hz.ywan-chungtsiang.top/gtxoftzwcy.html

SELECT id, name FROM users;
来源：http://hz.yvedp.cn/gtteyjdkfs.html

[Q17] 条件查询
来源：http://hz.yueranfly.top/gtzvrtdldh.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.zhijiandao.cn/gtglhdlead.html

[Q18] 模糊匹配
来源：http://hz.jinghuilouyu.cn/gtekkwmzay.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.redwolf501.top/gtwxwhzrpj.html

[Q19] 范围查询
来源：http://hz.xingfuxueyuan.xyz/gthranbraq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.sysykeji.top/gtipbgbbzl.html

[Q20] IN 列表
来源：http://hz.ehwqpu.com/gtujwiitxn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.mhx1999.top/gtkvhzydrl.html

[Q21] 空值判断
来源：http://hz.xziqi.cn/gthraivhte.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.shuidangran.top/gtqypphkyv.html

[Q22] 排序
来源：http://hz.xingfuxueyuan.xyz/gtekgdsyrf.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.haohaochexian.top/gtlllpoeug.html

[Q23] 分页
来源：http://hz.zhaomingkeji.xyz/gtnyhbtlmy.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.tianlin.xyz/gtpeyvngxt.html

[Q24] 去重
来源：http://hz.chenzaomai.com/gtjlzhellf.html

SELECT DISTINCT city FROM users;
来源：http://hz.jiagoushi.top/gtmozbvxut.html

[Q25] 只取前 N 条
来源：http://hz.xylfe.cn/gtqsupsnbu.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.xziqi.cn/gtjkickiyz.html

[Q26] 计数
来源：http://hz.xylfe.cn/gtexiklvrb.html

SELECT COUNT(*) FROM users;
来源：http://hz.redwolf501.top/gtlgoikdli.html

[Q27] 条件计数
来源：http://hz.quarkkingdee.top/gtcvrqujyw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.zdqjudy.top/gtgomlxxcx.html

[Q28] 求和与平均
来源：http://hz.yanxiufei.cn/gtmpcvgplx.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.52xcode.cn/gtrtpbbagl.html

[Q29] 最大最小值
来源：http://hz.yj20258888.top/gtmfkatisj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.jinqigfzy.top/gtzgetbcfd.html

[Q30] 分组统计
来源：http://hz.wangshuangyany.cn/gtpxapyqfu.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.jinqigufen.top/gtftvwteyi.html

[Q31] 分组后过滤
来源：http://hz.xinyue.icu/gtzibcecuo.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.zhixingplan.top/gtedckwggv.html

[Q32] 分组拼接字符串
来源：http://hz.mhx1999.top/gteqwlnlbg.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.fengsongda.top/gtihnmieyv.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.cqqwz.cn/gtqdiruutm.html

[Q33] 多列分组
来源：http://hz.52xcode.cn/gtyicalydr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yanxiufei.cn/gtklqmamxe.html

[Q34] 每组取第一条
来源：http://hz.gaohongyu789.top/gtndbtmjtv.html

SELECT * FROM (
来源：http://hz.jyoumei.cn/gtmpjxphxr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.ydzc1.top/gtokhnsxnx.html

) t WHERE rn = 1;
来源：http://hz.chenlongwang.top/gtlanagpie.html

[Q35] 内连接
来源：http://hz.jqgufenzy.top/gtgletwfku.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.fengsongda.top/gtvhkgshfl.html

[Q36] 左连接
来源：http://hz.yongpay.top/gtstzebzsa.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.jiagoushi.top/gtuhvxggia.html

[Q37] 右连接
来源：http://hz.hongshengwenyu.top/gtjtzqoqba.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.zhoulong.xyz/gttayqboci.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.sufxvd.cn/gtvmounduf.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.fengsongda.top/gtvnuxsexe.html

[Q39] 自连接（查上下级）
来源：http://hz.hnxiangtu.top/gtefvseoaf.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.fzhhl.top/gtfbuomrpk.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.iojbl.cn/gtadcujauy.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.havefunace.top/gtecoyyfzv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.yonumen.top/gtgtacfotj.html

[Q41] 多表连接
来源：http://hz.kuanghao11.cn/gtpzthsojm.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.sufxvd.cn/gtqcvunttu.html

JOIN users u ON u.id = o.user_id
来源：http://hz.gzhubu.top/gtwdlgvovk.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.sysykeji.top/gthqsqzfin.html

[Q42] 连接条件附加过滤
来源：http://hz.ywan-chungtsiang.top/gtxrwfkefv.html

SELECT u.name, o.amount FROM users u
来源：http://hz.ehwqpu.com/gtfulupjrn.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.hfpthk.cn/gtustucufk.html

[Q43] 标量子查询
来源：http://hz.mhx1999.top/gtzigmxmut.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.shanyushiyangtech.top/gtjhfpnwyt.html

[Q44] IN 子查询
来源：http://hz.zhixingplan.top/gtnokgtntb.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.0kj1m.cn/gtpsgbbmav.html

[Q45] EXISTS 判断存在
来源：http://hz.cqqwz.cn/gtgymsgvmq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hongshengwenyu.top/gttetzweor.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.shanyushiyangtech.top/gtmileuihd.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yj202588.top/gtumddnqvc.html

[Q47] 与平均值比较
来源：http://hz.hnqzz.top/gttbrachxa.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.cqqwz.cn/gtzxktryhh.html

[Q48] CTE 公用表表达式
来源：http://hz.jqgufenzy.top/gthhlwmckg.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.tanke756.top/gtphftasqh.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.cheryme.top/gtweagkqkg.html

[Q49] 更新单行
来源：http://hz.zhiwuduotai.top/gtagijtegz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.smart0.xyz/gttlsdoten.html

[Q50] 批量更新
来源：http://hz.jinqigufen.top/gtaoewlhzh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.chenlongwang.top/gtmrcmmulx.html

[Q51] 用子查询更新
来源：http://hz.redwolf501.top/gtwfsmebog.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.gogol.net.cn/gtgqtachbq.html

[Q52] 删除指定行
来源：http://hz.cashguo.top/gtmhsymfbc.html

DELETE FROM users WHERE id = 10;
来源：http://hz.gzhubu.top/gtgghjpifu.html

[Q53] 按条件删除
来源：http://hz.aizwys.cn/gtdplhxleh.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.zhoulong.xyz/gtpelvrqaf.html

[Q54] 清空表
来源：http://hz.zdqjudy.top/gtipbvpwqf.html

TRUNCATE TABLE logs;
来源：http://hz.nwbrower.top/gttngxqfqm.html

[Q55] 排名（并列占位）
来源：http://hz.ppjwa.cn/gtakejbija.html


<!-- 参考信息 -->