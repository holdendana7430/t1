代发 wailian999

[N09] 栈与队列
来源：http://hz.meibo888.top/gtawupsrns.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.bjfxy.top/gtwjdjsecr.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.tianlin.xyz/gtyixpfzgh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.hammf.cn/gtgzcsbcaz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.xuetiantiany.cn/gtsjfasvlu.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.smart0.xyz/gthqpsjvvc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.cqqwz.cn/gtgueoscsx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.9152youxi.cn/gtcasgyqhx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.mhx1999.top/gtuiqxtkeh.html

[N10] 链表节点定义
来源：http://hz.jqgufenzy.top/gtxvfrfjhg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.gzhubu.top/gtemoapvva.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.aibaodan.cn/gtvekwfgpa.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.jqgfzy.top/gtqqdkgzie.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.9152youxi.cn/gthfpmmkql.html

Java: class Node { int v; Node next; }
来源：http://hz.zycfv.cn/gtqvdcmoek.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.hnqzz.top/gtvmckgjnb.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.zdqjudy.top/gtsoetabug.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.xuetiantiany.cn/gtewlujzvr.html

[N11] 二叉树中序遍历
来源：http://hz.jlsjyb.cn/gtfrzjgpmh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.9152youxi.cn/gtvqsbahbc.html

PHP:  // 手写递归函数
来源：http://hz.vqdsnc.cn/gtpwxewqka.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ivvv.top/gtzyizgtzy.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.316326.xyz/gtgyuskoih.html

Java: // 手写递归
来源：http://hz.zhaomingkeji.xyz/gtkebadlfg.html

Go:   // 手写递归
来源：http://hz.jlsjyb.cn/gtwkecpsnt.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.cheryme.top/gtpzlfmrol.html

C#:   // 手写递归
来源：http://hz.vqdsnc.cn/gtevuqfdax.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yj20258888.top/gtrxqtpqgk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.daria6918.cn/gtddlkifhe.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.0kj1m.cn/gtjelfzuhz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.chenjidiqi.icu/gtgdmixfjl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jinqigfzy.top/gtccylcspc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xinyue.icu/gtuwnqrvvs.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.jqgufenzy.top/gtjoxmmpdn.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.wangdashe.top/gtdjqtaypq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ydzc1.top/gtznbnvjqr.html

================================================================================
来源：http://hz.316326.xyz/gtkihstwrf.html

O. 并发与异步
来源：http://hz.ywan-chungtsiang.top/gtemthxpry.html

================================================================================
来源：http://hz.cashguo.top/gtnndaonpl.html

[O01] 启动一个线程
来源：http://hz.shzxlz.cn/gtgssjbzff.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.xylfe.cn/gtuvimpvly.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.tian-w.cn/gtkzarbbko.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.jlsjyb.cn/gtjdlpshij.html

TS:   // 同 JS
来源：http://hz.yanxiufei.cn/gtxpwyiqpl.html

Java: new Thread(() -> f()).start()
来源：http://hz.smart0.xyz/gtrheljtop.html

Go:   go f()
来源：http://hz.ehwqpu.com/gtupimkjvh.html

Ruby: Thread.new { f }
来源：http://hz.fengsongda.top/gtmeatghuy.html

C#:   Task.Run(() => F());
来源：http://hz.jqgfzy.top/gtlkmyxsxw.html

[O02] 使用线程池
来源：http://hz.xuanzx.com/gtefhtkcwk.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.andypj.xyz/gtqptpyqsi.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.guannengcc.top/gtugumlwhk.html

JS:   // worker_threads 线程池
来源：http://hz.cucudq.cn/gtzzpmaisz.html

TS:   // worker_threads 线程池
来源：http://hz.iojbl.cn/gtiggdkomz.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.vqdsnc.cn/gtuevsxfyw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.xingfuxueyuan.xyz/gtmtrfsvkk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.xuanzx.com/gtvznkfwoz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.tianlin.xyz/gtpqgzvumi.html

[O03] 加锁保护共享数据
来源：http://hz.sysykeji.top/gtpirjlsit.html

Py:   with lock: shared += 1
来源：http://hz.sysykeji.top/gtxbyukqov.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.dashuyun.cn/gtoubxuqrc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.hywenlv.cn/gtynwkaqff.html

TS:   // 同 JS
来源：http://hz.iojbl.cn/gtaccbjfzg.html

Java: synchronized (this) { shared++; }
来源：http://hz.fzhhl.top/gtlgotvmyb.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.pycfn.com/gtzekfrrrd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.svipenyu.cn/gtgymjvwdu.html

C#:   lock (gate) { shared++; }
来源：http://hz.xingfuxueyuan.xyz/gtqkbuhill.html

[O04] 定义异步函数并等待
来源：http://hz.yvedp.cn/gtedbvxzzn.html

Py:   async def f():⏎    await g()
来源：http://hz.havefunace.top/gtyeskqayr.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.shanyushiyangkeji.top/gtkbrrwtbn.html

JS:   async function f() { await g(); }
来源：http://hz.guannengcc.top/gthjfihiwt.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yongpay.top/gtkhrzbdph.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.zhaomingkeji.xyz/gthqsppfww.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.shzxlz.cn/gtwzmesiej.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.xuetiantiany.cn/gtkcytswsy.html

C#:   async Task F() { await G(); }
来源：http://hz.iojbl.cn/gtfkfibwev.html

[O05] 并发执行并等待全部完成
来源：http://hz.gaohongyu789.top/gtbkyydrgf.html

Py:   asyncio.gather(*tasks)
来源：http://hz.zhijiandao.cn/gtdybrbnmo.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.pengpengdd.cyou/gtorwyvbvm.html

JS:   await Promise.all(tasks)
来源：http://hz.zhixingplan.top/gturmcrvib.html

TS:   await Promise.all(tasks)
来源：http://hz.zhaomingkeji.xyz/gtkgxiqyrn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.zycfv.cn/gtohuvehja.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.xuanzx.com/gtqjbfjeab.html

Ruby: threads.map(&:join)
来源：http://hz.ydzc1.top/gtvzjmhwff.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.hfpthk.cn/gtiutguyxc.html

[O06] 使用进程池
来源：http://hz.zdqjudy.top/gtcclttcom.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.zhixingplan.top/gtqdnyiifj.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.cashguo.top/gtvlbhjuei.html

JS:   // child_process / cluster 模块
来源：http://hz.52xcode.cn/gtfworxity.html

TS:   // child_process / cluster 模块
来源：http://hz.sxryk.cn/gtwjtfbdpf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.meibo888.top/gtizphouwm.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.ehwqpu.com/gtdxhprqqd.html

Ruby: // fork 块
来源：http://hz.cheryme.top/gtlgeqvisj.html

C#:   Parallel.For
来源：http://hz.ywan-chungtsiang.top/gtktwqgwgy.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtjdiflbfc.html

P. 常用工具函数
来源：http://hz.jianghu66.top/gtmzpauokr.html

================================================================================
来源：http://hz.jiagoushi.top/gteimnfthq.html

[P01] 生成 UUID
来源：http://hz.yvedp.cn/gtfwnwosxt.html

Py:   str(uuid.uuid4())
来源：http://hz.cheryme.top/gtjvdijkvh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jqgufenzy.top/gtnwjtlmnc.html

JS:   crypto.randomUUID()
来源：http://hz.fengsongda.top/gtdlytfsts.html

TS:   crypto.randomUUID()
来源：http://hz.aizwys.cn/gtmuhqmamn.html

Java: UUID.randomUUID().toString()
来源：http://hz.ybcxt.top/gtrrtskdlj.html

Go:   // 用 github.com/google/uuid
来源：http://hz.pycfn.com/gtowqueyot.html

Ruby: SecureRandom.uuid
来源：http://hz.hnxiangtu.top/gtnbghplmk.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.shangyingyoupin.top/gtktthigzn.html

[P02] MD5 / SHA256 摘要
来源：http://hz.yj20258.top/gthfjlzayu.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.sufxvd.cn/gtefpeqcwp.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.andypj.xyz/gtjblivyzo.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.hnxiangtu.top/gtapnmirgw.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.ywan-chungtsiang.top/gteougvnqq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.quarkkingdee.top/gtkamlxfmn.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.yangfankeji.com/gtriwdgkcp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.feifeiyinyue.top/gtlraavvnv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.xuetiantiany.cn/gtyfblibrw.html

[P03] 生成短随机字符串
来源：http://hz.quarkkingdee.top/gthngaqzuh.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.zdqjudy.top/gthdgeelud.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.jiagoushi.top/gtoygrivnh.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.tian-w.cn/gtpwhixwhs.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.guowangkeji.top/gtnaekwtll.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.daria6918.cn/gtvtoiayxz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.zhaomingkeji.xyz/gtutfguzhl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.chenjidiqi.icu/gtuuwzahic.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.xylfe.cn/gtnjgxcrkx.html

[P04] 求长度
来源：http://hz.tianlin.xyz/gtuyretaxi.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.52xcode.cn/gtghgdlwmt.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ywan-chungtsiang.top/gtjzjdxtqg.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ppjwa.cn/gtehyefpwn.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yj20258.top/gtisegqrdn.html

Java: list.size();  map.size();  s.length()
来源：http://hz.xuanzx.com/gtqfupwtpw.html

Go:   len(arr);  len(m)
来源：http://hz.jianghu66.top/gtfknkfpml.html

Ruby: x.length;  x.size
来源：http://hz.aibaodan.cn/gtguuswzrl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.jianghu66.top/gthxxbkysk.html

[P05] 判断两个对象内容是否相等
来源：http://hz.yuxming.cn/gtaaiqybbi.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.ppjwa.cn/gtxsfqgmju.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.haohaochexian.top/gtctvgjrty.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.vqdsnc.cn/gtuuzycyga.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.guowangkeji.top/gtykhsiips.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.shangyingyoupin.top/gticoefmyi.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.pengpengdd.cyou/gtxkjuvjfa.html

Ruby: a == b
来源：http://hz.jlsjyb.cn/gtpbzgnwkd.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.xingfuxueyuan.xyz/gthhaltisn.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.yvedp.cn/gtulumjqyu.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.zhoulong.xyz/gthjktvvfh.html

PHP:  if (empty($x)) {}
来源：http://hz.yj20258888.top/gtuhmaynho.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.zhaomingkeji.xyz/gtuifzbzon.html

TS:   if (x == null) {}
来源：http://hz.cucudq.cn/gtwcrxywld.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.sweek.top/gtikgavlim.html

Go:   if x == nil {}
来源：http://hz.sxryk.cn/gtngukbnej.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.hfpthk.cn/gtxsewzegt.html

C#:   if (x is null) {}
来源：http://hz.shangyingyoupin.top/gtdgkourwv.html

[P07] 防抖与节流
来源：http://hz.ivvv.top/gtggvsvxsz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.shuidangran.top/gtjvtsjjkm.html

PHP:  // 手写时间戳比较
来源：http://hz.shanyushiyangkeji.top/gtlmhoxiqw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xuanzx.com/gtskbbbbqc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ybcxt.top/gtxvpixwgf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.gzhubu.top/gtywqizwuj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.tanke756.top/gtbcfidqtm.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.chenzaomai.com/gtrtedaeuq.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.chenlongwang.top/gtjveunrfk.html

[P08] 处理浮点精度问题
来源：http://hz.kuanghao11.cn/gtiktpdnpt.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.hnqzz.top/gtunufhfme.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.ydzc1.top/gtwinebjhh.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.birdmap.top/gtlefmgtre.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.smart0.xyz/gtslstdmqw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.zdqjudy.top/gtoguwatio.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.tian-w.cn/gtodorryck.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.zhijiandao.cn/gtifdblxdj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.pengpengdd.cyou/gtrtxkbnkv.html

================================================================================
来源：http://hz.gaohongyu789.top/gtjzdymxgw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.9152youxi.cn/gtervcxqux.html

================================================================================
来源：http://hz.haohaochexian.top/gtwhuubeoj.html

[Q01] 创建表
来源：http://hz.iojbl.cn/gtbaosuwxx.html

CREATE TABLE users (
来源：http://hz.xziqi.cn/gtciqpiehx.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.cheryme.top/gtaxurkxer.html

name VARCHAR(50) NOT NULL,
来源：http://hz.c1oappe.top/gtgjbhqnfq.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jlsjyb.cn/gtmgawtmrk.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.tianlin.xyz/gtovvccfya.html

);
来源：http://hz.cheryme.top/gtyhsxmadu.html

[Q02] 创建带外键的表
来源：http://hz.yangfankeji.com/gtyjjtnfht.html

CREATE TABLE orders (
来源：http://hz.cqqwz.cn/gtmvuossrg.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.vqdsnc.cn/gtjfoeatxu.html

user_id INT NOT NULL,
来源：http://hz.cashguo.top/gtajthwmqf.html

amount DECIMAL(10, 2),
来源：http://hz.nanxinkj.top/gtzwteaxft.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.jianghu66.top/gtxmcltnkn.html

);
来源：http://hz.feifeiyinyue.top/gtstaklgvm.html

[Q03] 增加列
来源：http://hz.iojbl.cn/gtfzssuvqc.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.nanxuanxn.top/gtzyxrnxeh.html

[Q04] 修改列类型
来源：http://hz.9152youxi.cn/gtmsonzggs.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.mhx1999.top/gthneouglh.html

[Q05] 重命名列
来源：http://hz.jinqigufen.top/gtpyvklmmk.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.xuanzx.com/gtqcbqqqns.html

[Q06] 删除列
来源：http://hz.yuxming.cn/gtzavhpkky.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.yonumen.top/gtwjhcnmdm.html

[Q07] 删除表
来源：http://hz.feifeiyinyue.top/gtksmzszcj.html

DROP TABLE IF EXISTS orders;
来源：http://hz.zycfv.cn/gtjfdlltjd.html

[Q08] 创建普通索引
来源：http://hz.ydzc1.top/gtjqqdecwe.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.sysykeji.top/gtxpsgguzo.html

[Q09] 创建唯一索引
来源：http://hz.jinyuanbaomall.cn/gtaverltet.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.shuidangran.top/gtrzsvphla.html

[Q10] 插入单行
来源：http://hz.jqgfzy.top/gtgofzwlks.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.c1oappe.top/gtrvzxdbsa.html

[Q11] 一次插入多行
来源：http://hz.havefunace.top/gthbayfjnm.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.dianchejie.cn/gtsoichtsv.html

[Q12] 插入后取自增 ID
来源：http://hz.gotoacloud.top/gtouesqyik.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yvedp.cn/gtcydcebea.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.gaohongyu789.top/gtcwytkdow.html

[Q13] 忽略重复插入
来源：http://hz.birdmap.top/gtenwkfbbw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.tianlin.xyz/gtziamzarv.html

[Q14] 存在则更新（upsert）
来源：http://hz.sweek.top/gtqmlnfshy.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.zhixingplan.top/gtlyzleska.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.hfpthk.cn/gtunonlvak.html

[Q15] 查询全部
来源：http://hz.iojbl.cn/gtmebfpwhx.html

SELECT * FROM users;
来源：http://hz.hnxiangtu.top/gttqkvkgoj.html

[Q16] 查询指定列
来源：http://hz.yj20258.top/gtpxlnervf.html

SELECT id, name FROM users;
来源：http://hz.bjfxy.top/gtqotainzx.html

[Q17] 条件查询
来源：http://hz.jqgfzy.top/gtnipmxold.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.jiagoushi.top/gtswguljar.html

[Q18] 模糊匹配
来源：http://hz.yanxiufei.cn/gtzixgdqrm.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.cqqwz.cn/gtujfgfkom.html

[Q19] 范围查询
来源：http://hz.zhijiandao.cn/gtttiedjge.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.hnxiangtu.top/gtjnjrcska.html

[Q20] IN 列表
来源：http://hz.jiagoushi.top/gtdpwtwqyn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.ppjwa.cn/gtwltvyvva.html

[Q21] 空值判断
来源：http://hz.aizwys.cn/gtxztyuguv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.jiagoushi.top/gtqhfkkmxf.html

[Q22] 排序
来源：http://hz.jiagoushi.top/gtpcxtdyks.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.316326.xyz/gtgwkuvbpv.html

[Q23] 分页
来源：http://hz.hysaishi.cn/gtzdbvrakr.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.xinyue.icu/gtzvwkdzre.html

[Q24] 去重
来源：http://hz.shangyingyoupin.top/gtlobqjety.html

SELECT DISTINCT city FROM users;
来源：http://hz.jlsjyb.cn/gttzexbgmi.html

[Q25] 只取前 N 条
来源：http://hz.cheryme.top/gtimondsxw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.9152youxi.cn/gtqikqhsia.html

[Q26] 计数
来源：http://hz.vqdsnc.cn/gtmtigptvj.html

SELECT COUNT(*) FROM users;
来源：http://hz.sxryk.cn/gtgikroqyz.html

[Q27] 条件计数
来源：http://hz.dashuyun.cn/gtlyvdklwn.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.hammf.cn/gtxbsdffnj.html

[Q28] 求和与平均
来源：http://hz.xingfuxueyuan.xyz/gtdvghxyen.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.yangfankeji.com/gtefddrwdo.html

[Q29] 最大最小值
来源：http://hz.redwolf501.top/gtikfbqomc.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.zhijiandao.cn/gtfjgpzkkt.html

[Q30] 分组统计
来源：http://hz.aizwys.cn/gtxpisemkn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.ppjwa.cn/gtaisnlekw.html

[Q31] 分组后过滤
来源：http://hz.fengsongda.top/gtztplprit.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.smart0.xyz/gtwgqvukrc.html

[Q32] 分组拼接字符串
来源：http://hz.chenzaomai.com/gtgytyorsr.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.svipenyu.cn/gtqreetgtc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.jqgufenzy.top/gtwsmyxctd.html

[Q33] 多列分组
来源：http://hz.jqgufenzy.top/gtakkivttx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.nanxinkj.top/gtzcemrwmr.html

[Q34] 每组取第一条
来源：http://hz.zhoulong.xyz/gtahxsnhdz.html

SELECT * FROM (
来源：http://hz.gotoacloud.top/gtbomnmkpd.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.andypj.xyz/gtjxanshvq.html

) t WHERE rn = 1;
来源：http://hz.ydzc1.top/gtiboqymuu.html

[Q35] 内连接
来源：http://hz.yuanzhike.top/gtwrodhqjl.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.gzhubu.top/gtxsszisga.html

[Q36] 左连接
来源：http://hz.316326.xyz/gtolaebugd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.yangfankeji.com/gtjgejadhh.html

[Q37] 右连接
来源：http://hz.mhx1999.top/gtgysdqehm.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.zhiwuduotai.top/gtlxsthdrq.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.dashuyun.cn/gthdcfbory.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.gaohongyu789.top/gtrmtjmfck.html

[Q39] 自连接（查上下级）
来源：http://hz.quarkkingdee.top/gtpwgqexpa.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jinqigufen.top/gtoucvszdw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yj202588.top/gtczmoqbpi.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.shangyingyoupin.top/gtnauzoxxz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.jinqigufen.top/gtpayvammy.html

[Q41] 多表连接
来源：http://hz.hongshengwenyu.top/gtozfrgbxu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.jinyuanbaomall.cn/gtwykszwgr.html

JOIN users u ON u.id = o.user_id
来源：http://hz.pycfn.com/gtcnsdmfsj.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.zhijiandao.cn/gtgonzvybj.html

[Q42] 连接条件附加过滤
来源：http://hz.nwbrower.top/gtknpwkhcr.html

SELECT u.name, o.amount FROM users u
来源：http://hz.sysykeji.top/gtimympejn.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.zhixingplan.top/gtgoampmge.html

[Q43] 标量子查询
来源：http://hz.yj202588.top/gtzuawvwrf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.chenzaomai.com/gtzkbwisjy.html

[Q44] IN 子查询
来源：http://hz.jqgufenzy.top/gtyuugfnqe.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.quarkkingdee.top/gtirzmllxx.html

[Q45] EXISTS 判断存在
来源：http://hz.316326.xyz/gtbtcphogs.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.quarkkingdee.top/gtoplxnyef.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.nwbrower.top/gtjbalyjos.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yvedp.cn/gtzihdwrvm.html

[Q47] 与平均值比较
来源：http://hz.yuanzhike.top/gtxsxpgouv.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.hongshengwenyu.top/gtvfgxsgzm.html

[Q48] CTE 公用表表达式
来源：http://hz.yueranfly.top/gtzysemiyv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.ppjwa.cn/gtrrkvyvox.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.zhiwuduotai.top/gtdwqhxrle.html

[Q49] 更新单行
来源：http://hz.cqqwz.cn/gtombeyurk.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.snrcjt.cn/gtueeavmgg.html

[Q50] 批量更新
来源：http://hz.jinqigufen.top/gtcwhrkzfx.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zhengqikj.top/gtsaolhjog.html

[Q51] 用子查询更新
来源：http://hz.meibo888.top/gtzgzuchxn.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.aibaodan.cn/gtecorsosc.html

[Q52] 删除指定行
来源：http://hz.xingfuxueyuan.xyz/gtejnxfejh.html

DELETE FROM users WHERE id = 10;
来源：http://hz.cucudq.cn/gtwvriyecg.html

[Q53] 按条件删除
来源：http://hz.wangshuangyany.cn/gtaenngglx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.xuanzx.com/gtuznhxqlb.html

[Q54] 清空表
来源：http://hz.hfpthk.cn/gtggksvjsp.html

TRUNCATE TABLE logs;
来源：http://hz.mhx1999.top/gtepzbabem.html

[Q55] 排名（并列占位）
来源：http://hz.daxiang520.top/gteawphral.html


<!-- 参考信息 -->