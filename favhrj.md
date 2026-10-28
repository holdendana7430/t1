代发 wailian999

Java: // 手写回溯递归
来源：http://hz.yuanzhike.top/gtnfcuovgu.html

Go:   // 手写回溯递归
来源：http://hz.jianghu66.top/gtnaadwuxj.html

Ruby: arr.permutation.to_a
来源：http://hz.yanxiufei.cn/gtshrxquwl.html

C#:   // 手写回溯递归
来源：http://hz.yueranfly.top/gtzidmcdvu.html

[N09] 栈与队列
来源：http://hz.sufxvd.cn/gtsshhwpgn.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.zhoulong.xyz/gtoayyoheg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.yj202588.top/gthesdspfx.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.cqqwz.cn/gtxconloek.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.aibaodan.cn/gtgbwyspst.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yj20258888.top/gtkprvqgom.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.hnqzz.top/gtcbvzjxwe.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.hysaishi.cn/gtngghynjx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yj20258888.top/gtqgznzlsi.html

[N10] 链表节点定义
来源：http://hz.daria6918.cn/gtspntpiez.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.zhijiandao.cn/gtndfxqoyt.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.ehwqpu.com/gtjsqwuthy.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.jinyuanbaomall.cn/gtivnbluvh.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.gzhubu.top/gtvpnppxjk.html

Java: class Node { int v; Node next; }
来源：http://hz.iojbl.cn/gtiinapezi.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.birdmap.top/gtirflhmhv.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.vqdsnc.cn/gtjofghvsi.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.chenzaomai.com/gtckczqkmg.html

[N11] 二叉树中序遍历
来源：http://hz.hfpthk.cn/gtjygrsyxy.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.cheryme.top/gtwnmgtooy.html

PHP:  // 手写递归函数
来源：http://hz.yj20258888.top/gtgmmjiwdv.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jiagoushi.top/gttuiopoyp.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jinqigufen.top/gtmnorourx.html

Java: // 手写递归
来源：http://hz.nanxuanxn.top/gtjseinfwo.html

Go:   // 手写递归
来源：http://hz.sufxvd.cn/gtmslzrdjw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.xziqi.cn/gtwlrbndmh.html

C#:   // 手写递归
来源：http://hz.yangfankeji.com/gtzvicxfxl.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.jinqigfzy.top/gtxykktitm.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.xziqi.cn/gtfuizbrxl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.havefunace.top/gtregjulaq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.sufxvd.cn/gtohybbptp.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.tanke756.top/gtqumecksz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xuetiantiany.cn/gtbvrgryvl.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.yueranfly.top/gtljdouzgq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.yvedp.cn/gtywymgdsj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhiwuduotai.top/gtgxycxwip.html

================================================================================
来源：http://hz.gaohongyu789.top/gtrxacjuft.html

O. 并发与异步
来源：http://hz.bjfxy.top/gtvwaawccn.html

================================================================================
来源：http://hz.hnqzz.top/gtsewxmukq.html

[O01] 启动一个线程
来源：http://hz.hywenlv.cn/gtywqvqshe.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.aizwys.cn/gtbfqmbzvt.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.quarkkingdee.top/gtwojropao.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.bjfxy.top/gtjtakibpr.html

TS:   // 同 JS
来源：http://hz.wangdashe.top/gtyzcwdbjs.html

Java: new Thread(() -> f()).start()
来源：http://hz.gotoacloud.top/gtaotwxjwx.html

Go:   go f()
来源：http://hz.xziqi.cn/gtrvcpacfa.html

Ruby: Thread.new { f }
来源：http://hz.pengpengdd.cyou/gtegdrucom.html

C#:   Task.Run(() => F());
来源：http://hz.jyoumei.cn/gtrcdbioqr.html

[O02] 使用线程池
来源：http://hz.zhijiandao.cn/gtdlavpfln.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yj20258888.top/gtccvpehpk.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.shanyushiyangtech.top/gtqqjacgeo.html

JS:   // worker_threads 线程池
来源：http://hz.jinyuanbaomall.cn/gtnyyatdig.html

TS:   // worker_threads 线程池
来源：http://hz.vqdsnc.cn/gtdccuqnmw.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.sysykeji.top/gtlxkxqoxo.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.jqgufenzy.top/gtdvxjpudk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.zhixingplan.top/gtfsrqfwuw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.yueranfly.top/gtznpnbknk.html

[O03] 加锁保护共享数据
来源：http://hz.ehwqpu.com/gtlwqmftyl.html

Py:   with lock: shared += 1
来源：http://hz.smart0.xyz/gtyjnymyev.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.316326.xyz/gtiswzuzie.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.cdnleiting.top/gtzflzofhi.html

TS:   // 同 JS
来源：http://hz.tian-w.cn/gtzrwdslby.html

Java: synchronized (this) { shared++; }
来源：http://hz.jinghuilouyu.cn/gtrkpsojqt.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.chenlongwang.top/gtjcygudnk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.xingfuxueyuan.xyz/gtpebldzrq.html

C#:   lock (gate) { shared++; }
来源：http://hz.9152youxi.cn/gtbexcrcmb.html

[O04] 定义异步函数并等待
来源：http://hz.iojbl.cn/gtukcvaesz.html

Py:   async def f():⏎    await g()
来源：http://hz.0kj1m.cn/gtayondseb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.yuanzhike.top/gtwaguhpvd.html

JS:   async function f() { await g(); }
来源：http://hz.xuanzx.com/gtbjfsqwpm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yueranfly.top/gthtpjvung.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.redwolf501.top/gtbrrwgvya.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.nwbrower.top/gtmmjyxpzv.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yanxiufei.cn/gteidjqaiq.html

C#:   async Task F() { await G(); }
来源：http://hz.cdnleiting.top/gtxzebyubr.html

[O05] 并发执行并等待全部完成
来源：http://hz.9152youxi.cn/gtcomntrrz.html

Py:   asyncio.gather(*tasks)
来源：http://hz.aizwys.cn/gtdctnmodu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.yanxiufei.cn/gtpcgboslw.html

JS:   await Promise.all(tasks)
来源：http://hz.ydjk.org.cn/gthtokfhxh.html

TS:   await Promise.all(tasks)
来源：http://hz.cdnleiting.top/gtbmyqvstc.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.xingfuxueyuan.xyz/gtuiivqnue.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.xziqi.cn/gtmavafbjd.html

Ruby: threads.map(&:join)
来源：http://hz.zhoulong.xyz/gtaullpdor.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.wangshuangyany.cn/gtzydbbagk.html

[O06] 使用进程池
来源：http://hz.tian-w.cn/gtwtqpwwyn.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.316326.xyz/gtlgrzpsww.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.daria6918.cn/gtdndfccqo.html

JS:   // child_process / cluster 模块
来源：http://hz.xinyue.icu/gtybgtjrtg.html

TS:   // child_process / cluster 模块
来源：http://hz.52xcode.cn/gtrdjzhegc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yonumen.top/gtkozyfdkf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.yuanzhike.top/gttkhgtlmj.html

Ruby: // fork 块
来源：http://hz.ybcxt.top/gtejzxmpff.html

C#:   Parallel.For
来源：http://hz.shangyingyoupin.top/gtzgnqylfp.html

================================================================================
来源：http://hz.jiagoushi.top/gtkjxoqcst.html

P. 常用工具函数
来源：http://hz.quarkkingdee.top/gtfpjqxtrz.html

================================================================================
来源：http://hz.iojbl.cn/gtcnsztnlw.html

[P01] 生成 UUID
来源：http://hz.zycfv.cn/gtzmeilcko.html

Py:   str(uuid.uuid4())
来源：http://hz.yanxiufei.cn/gtbqjyrnqt.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.haohaochexian.top/gtxzmbnjwf.html

JS:   crypto.randomUUID()
来源：http://hz.yueranfly.top/gtwhkprrgo.html

TS:   crypto.randomUUID()
来源：http://hz.svipenyu.cn/gtjqbqadxb.html

Java: UUID.randomUUID().toString()
来源：http://hz.gzhubu.top/gtccohfeyk.html

Go:   // 用 github.com/google/uuid
来源：http://hz.cheryme.top/gtezmcszso.html

Ruby: SecureRandom.uuid
来源：http://hz.chenlongwang.top/gtlawcqkqq.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.birdmap.top/gtzvvmwggl.html

[P02] MD5 / SHA256 摘要
来源：http://hz.xuetiantiany.cn/gttmrfkvtq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.guowangkeji.top/gtvyxzwfne.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.fengsongda.top/gtfpyobzlm.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yj20258888.top/gtgzwfzdzc.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.316326.xyz/gtciemxfae.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.redwolf501.top/gtgyktvkzg.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.shanyushiyangtech.top/gtwruekeih.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.pengpengdd.cyou/gtwxenwesy.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.chenzaomai.com/gtnbpvhymb.html

[P03] 生成短随机字符串
来源：http://hz.xuetiantiany.cn/gtpcpvwugk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.gogol.net.cn/gtnfnvunki.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.zhaomingkeji.xyz/gtcaubcpip.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ywan-chungtsiang.top/gtjsfhgyji.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ppjwa.cn/gtdjhdcnwf.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.guannengcc.top/gtimswukkj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.iojbl.cn/gtgrojcctz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.nwbrower.top/gtmsvkeygf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.xingfuxueyuan.xyz/gtmsncprpn.html

[P04] 求长度
来源：http://hz.zycfv.cn/gtxrabqspj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.cheryme.top/gtcmyrzxyd.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.sxryk.cn/gtzbqadzyj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.sweek.top/gtjexulrhv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.sysykeji.top/gtcasuvsgr.html

Java: list.size();  map.size();  s.length()
来源：http://hz.sxryk.cn/gtvyprmgvs.html

Go:   len(arr);  len(m)
来源：http://hz.xinyue.icu/gtmkcxrsss.html

Ruby: x.length;  x.size
来源：http://hz.wangdashe.top/gtrnemohhn.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.cucudq.cn/gtdadyfmkr.html

[P05] 判断两个对象内容是否相等
来源：http://hz.sysykeji.top/gtzffoagmz.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.hywenlv.cn/gtctclyrqi.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.9152youxi.cn/gttcifbdai.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.jinqigufen.top/gtvsbdtxpr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.ywan-chungtsiang.top/gtzhbrpnal.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.hnxiangtu.top/gtvstepgyb.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.jinqigufen.top/gtjbyhyfoc.html

Ruby: a == b
来源：http://hz.shuidangran.top/gtpsaiygdr.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.gotoacloud.top/gtvucdbger.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.sweek.top/gtwxngafty.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.mhx1999.top/gtnaibrfxk.html

PHP:  if (empty($x)) {}
来源：http://hz.cdnleiting.top/gtzxwisgtm.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.nwbrower.top/gtwijoqsfb.html

TS:   if (x == null) {}
来源：http://hz.fzhhl.top/gtypvbhvlw.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.quarkkingdee.top/gttcrhbmlj.html

Go:   if x == nil {}
来源：http://hz.zhengqikj.top/gtcyqkwkaz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.ehwqpu.com/gtvptjxlgl.html

C#:   if (x is null) {}
来源：http://hz.pengpengdd.cyou/gtuurbqklc.html

[P07] 防抖与节流
来源：http://hz.jinyuanbaomall.cn/gtjmzleugv.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.wangdashe.top/gtyacgrobf.html

PHP:  // 手写时间戳比较
来源：http://hz.yuanzhike.top/gtumgaomui.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.tanke756.top/gteqylpvhs.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.dianchejie.cn/gtyscyzxsq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.zhixingplan.top/gtphepoxrt.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.cqqwz.cn/gthggkzfjx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.tian-w.cn/gtajhbgyfh.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.316326.xyz/gtdodouxgx.html

[P08] 处理浮点精度问题
来源：http://hz.xuetiantiany.cn/gtevnbayif.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jinqigufen.top/gthvnkaeeq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.yuanzhike.top/gtxxwbpzse.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.zdqjudy.top/gtqavvhrvi.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.yj202588.top/gtqvcbntyx.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.xziqi.cn/gtnhpfnwkx.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.daxiang520.top/gtamqjmpmj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.aibaodan.cn/gtkzdjhknx.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.316326.xyz/gtzcfvlbwg.html

================================================================================
来源：http://hz.havefunace.top/gtvmoixyfq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.havefunace.top/gtyccdxttr.html

================================================================================
来源：http://hz.yongpay.top/gtwjoejida.html

[Q01] 创建表
来源：http://hz.cheryme.top/gtblhqjrkk.html

CREATE TABLE users (
来源：http://hz.xingfuxueyuan.xyz/gtekylvxbx.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xylfe.cn/gtmohlfoej.html

name VARCHAR(50) NOT NULL,
来源：http://hz.snrcjt.cn/gtytyknhzb.html

email VARCHAR(100) UNIQUE,
来源：http://hz.aizwys.cn/gtdvrinloe.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.cashguo.top/gtiytdssff.html

);
来源：http://hz.yvedp.cn/gtxspdmdjn.html

[Q02] 创建带外键的表
来源：http://hz.cucudq.cn/gtcxznlzht.html

CREATE TABLE orders (
来源：http://hz.zhixingplan.top/gtewajlmoj.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.feifeiyinyue.top/gtyldpehac.html

user_id INT NOT NULL,
来源：http://hz.xylfe.cn/gtqfdtcegi.html

amount DECIMAL(10, 2),
来源：http://hz.shanyushiyangkeji.top/gtgkdillwh.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.9152youxi.cn/gtyrszkapw.html

);
来源：http://hz.316326.xyz/gtqcnlachr.html

[Q03] 增加列
来源：http://hz.hfpthk.cn/gtgydyvuze.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.xuetiantiany.cn/gtttgizbvw.html

[Q04] 修改列类型
来源：http://hz.snrcjt.cn/gtumiiluay.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.mhx1999.top/gtbpymabty.html

[Q05] 重命名列
来源：http://hz.gzhubu.top/gthoiaefwc.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.yvedp.cn/gtpreucpel.html

[Q06] 删除列
来源：http://hz.yangfankeji.com/gtzfarwiot.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.jlsjyb.cn/gtsknkhodq.html

[Q07] 删除表
来源：http://hz.fzhhl.top/gtzuwmgycv.html

DROP TABLE IF EXISTS orders;
来源：http://hz.wangdashe.top/gtbmizjhlk.html

[Q08] 创建普通索引
来源：http://hz.cucudq.cn/gtyqyoqsgz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.quarkkingdee.top/gtnbuvbvoe.html

[Q09] 创建唯一索引
来源：http://hz.tanke756.top/gtnwoiwpft.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.quarkkingdee.top/gteglpeawg.html

[Q10] 插入单行
来源：http://hz.jinghuilouyu.cn/gtxvtpyldx.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.xuanzx.com/gtdloclaaz.html

[Q11] 一次插入多行
来源：http://hz.yongpay.top/gtzzbgpqgt.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.ywan-chungtsiang.top/gtpngbmsls.html

[Q12] 插入后取自增 ID
来源：http://hz.316326.xyz/gtjpbadzsp.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.gaohongyu789.top/gtlccueilj.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.quarkkingdee.top/gtnrjdzmur.html

[Q13] 忽略重复插入
来源：http://hz.xingfuxueyuan.xyz/gtvtattsht.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.yvedp.cn/gtwrkdshch.html

[Q14] 存在则更新（upsert）
来源：http://hz.tianlin.xyz/gthnwuqicd.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.cucudq.cn/gtbqdkblos.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.iojbl.cn/gtglqibkqz.html

[Q15] 查询全部
来源：http://hz.gogol.net.cn/gtbyxdaapx.html

SELECT * FROM users;
来源：http://hz.sweek.top/gtbvhvfwpg.html

[Q16] 查询指定列
来源：http://hz.0kj1m.cn/gtavdwdard.html

SELECT id, name FROM users;
来源：http://hz.ywan-chungtsiang.top/gtmkauyfwn.html

[Q17] 条件查询
来源：http://hz.jlsjyb.cn/gtmwfypxro.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.tian-w.cn/gtildormjq.html

[Q18] 模糊匹配
来源：http://hz.zhaomingkeji.xyz/gtxpigublm.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.ehwqpu.com/gtyvhzcxfe.html

[Q19] 范围查询
来源：http://hz.iojbl.cn/gttiqagjys.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.cashguo.top/gtdooencng.html

[Q20] IN 列表
来源：http://hz.redwolf501.top/gtzfuwoden.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.vqdsnc.cn/gtsyfqvrxe.html

[Q21] 空值判断
来源：http://hz.yj202588.top/gtkljqrzku.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.dianchejie.cn/gtotdapbdz.html

[Q22] 排序
来源：http://hz.sxryk.cn/gtwazivahr.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.svipenyu.cn/gtluqeourc.html

[Q23] 分页
来源：http://hz.tanke756.top/gtuqblluwu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.pycfn.com/gtextxoxxk.html

[Q24] 去重
来源：http://hz.wangshuangyany.cn/gtixyitfva.html

SELECT DISTINCT city FROM users;
来源：http://hz.jianghu66.top/gtirlcfxsx.html

[Q25] 只取前 N 条
来源：http://hz.zycfv.cn/gtbmvgrcqp.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.shangyingyoupin.top/gtrcnadykm.html

[Q26] 计数
来源：http://hz.tian-w.cn/gtkjywtsrs.html

SELECT COUNT(*) FROM users;
来源：http://hz.ivvv.top/gtkckewpss.html

[Q27] 条件计数
来源：http://hz.zhijiandao.cn/gtvjxyewtn.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yuanzhike.top/gtgghbjxgc.html

[Q28] 求和与平均
来源：http://hz.mhx1999.top/gtntmohgon.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.birdmap.top/gtgeybpaon.html

[Q29] 最大最小值
来源：http://hz.kuanghao11.cn/gtghxslbuo.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.jinghuilouyu.cn/gtglvimbvy.html

[Q30] 分组统计
来源：http://hz.jinqigufen.top/gtlbtbibyq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.shuidangran.top/gtgjgzuxxz.html

[Q31] 分组后过滤
来源：http://hz.wangshuangyany.cn/gtysbtvahe.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.zhengqikj.top/gtkipsnypb.html

[Q32] 分组拼接字符串
来源：http://hz.snrcjt.cn/gtkbpwyago.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.cdnleiting.top/gtjraittvn.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.hywenlv.cn/gtisepyfea.html

[Q33] 多列分组
来源：http://hz.tianlin.xyz/gtpkdfvzfi.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.hnxiangtu.top/gthcrzdcad.html

[Q34] 每组取第一条
来源：http://hz.vqdsnc.cn/gtyxpmnzdc.html

SELECT * FROM (
来源：http://hz.316326.xyz/gtedlukovp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.zhoulong.xyz/gtnrdmmrsf.html

) t WHERE rn = 1;
来源：http://hz.ppjwa.cn/gtpsrgupvx.html

[Q35] 内连接
来源：http://hz.c1oappe.top/gtrbhtrewj.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.gogol.net.cn/gtooyeabcw.html

[Q36] 左连接
来源：http://hz.gzhubu.top/gtkvuvaozc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhongyouzk.top/gtyrzgvtep.html

[Q37] 右连接
来源：http://hz.zhijiandao.cn/gtkqpsvbbv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.yonumen.top/gtumgjkvgf.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.ydzc1.top/gtkkkbzwvl.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.9152youxi.cn/gtoykuhwpi.html

[Q39] 自连接（查上下级）
来源：http://hz.shangyingyoupin.top/gtwvyqheoo.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.yj202588.top/gtltycaicj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.vqdsnc.cn/gtzywssddf.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.daria6918.cn/gtcmjpcklo.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.jinghuilouyu.cn/gtladrjazt.html

[Q41] 多表连接
来源：http://hz.svipenyu.cn/gtgdrnjgwf.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.xinyue.icu/gtuoxoteju.html

JOIN users u ON u.id = o.user_id
来源：http://hz.shanyushiyangkeji.top/gtyknkaiwt.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.sxryk.cn/gtppgmxjaq.html

[Q42] 连接条件附加过滤
来源：http://hz.yuxming.cn/gtbkoqddox.html

SELECT u.name, o.amount FROM users u
来源：http://hz.jqgfzy.top/gtslafzhng.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.hysaishi.cn/gtrgsuvczg.html

[Q43] 标量子查询
来源：http://hz.dianchejie.cn/gtrgaqoina.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.gaohongyu789.top/gtzvqaaaqh.html

[Q44] IN 子查询
来源：http://hz.gotoacloud.top/gtekkczcfw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.fengsongda.top/gtldlzbnwq.html

[Q45] EXISTS 判断存在
来源：http://hz.shangyingyoupin.top/gtijjnmxuw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jinyuanbaomall.cn/gtrozuzjde.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.chenjidiqi.icu/gtoytlhduq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.nanxuanxn.top/gthqkotvuy.html

[Q47] 与平均值比较
来源：http://hz.jyoumei.cn/gtmhkmkasg.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.c1oappe.top/gtexpzemfd.html

[Q48] CTE 公用表表达式
来源：http://hz.mhx1999.top/gteazcgitc.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.shanyushiyangkeji.top/gtqmnhlkow.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.tian-w.cn/gtgjiguqjw.html

[Q49] 更新单行
来源：http://hz.c1oappe.top/gtgqbqmmkz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.jyoumei.cn/gtxdybmqhx.html

[Q50] 批量更新
来源：http://hz.cheryme.top/gtqrhucgec.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.yanxiufei.cn/gtnodpxbbc.html

[Q51] 用子查询更新
来源：http://hz.ybcxt.top/gtsckyccwb.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.zhengqikj.top/gtcmbdcejg.html

[Q52] 删除指定行
来源：http://hz.xylfe.cn/gtwuawbuwd.html

DELETE FROM users WHERE id = 10;
来源：http://hz.nwbrower.top/gtodfwsefk.html

[Q53] 按条件删除
来源：http://hz.zhixingplan.top/gtgyyrkzfo.html


<!-- 参考信息 -->