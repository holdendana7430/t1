代发 wailian999

[N09] 栈与队列
来源：http://hz.nanxinkj.top/gtevtichsb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.chenjidiqi.icu/gtypxfpfpz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.iojbl.cn/gtxixqjzak.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.52xcode.cn/gtyalxevpu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.daxiang520.top/gtchmtybil.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.aibaodan.cn/gtatackzks.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.shanyushiyangtech.top/gtotjzjqqz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.dianchejie.cn/gtrpswjswt.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.xuetiantiany.cn/gtwggbyllz.html

[N10] 链表节点定义
来源：http://hz.yueranfly.top/gtfyreytte.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yueranfly.top/gtworvplea.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.yangfankeji.com/gtmwdmzzdw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yj202588.top/gtycoxmlbn.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.nwbrower.top/gtjnvqekuc.html

Java: class Node { int v; Node next; }
来源：http://hz.snrcjt.cn/gtugtteuvp.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.yonumen.top/gtsymyrhzt.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.nanxinkj.top/gtdehaafgc.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.ehwqpu.com/gtnkhdjtbs.html

[N11] 二叉树中序遍历
来源：http://hz.aizwys.cn/gtkfpjmuck.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.jiagoushi.top/gtkfzebfdr.html

PHP:  // 手写递归函数
来源：http://hz.jiagoushi.top/gtzezthlmz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.chenjidiqi.icu/gtsjjbetxu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.pengpengdd.cyou/gtsdwsjqug.html

Java: // 手写递归
来源：http://hz.hnxiangtu.top/gtqqqoozvo.html

Go:   // 手写递归
来源：http://hz.zdqjudy.top/gtfexfktyf.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.jiagoushi.top/gtdldzqaem.html

C#:   // 手写递归
来源：http://hz.cheryme.top/gthriiojfs.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.hfpthk.cn/gtlstnwdal.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.jiagoushi.top/gtygdibexd.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.xuetiantiany.cn/gtmrzmxjay.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yj202588.top/gtcdgchrxv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhengqikj.top/gtiaqldghs.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.fengsongda.top/gtbvevfcgi.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.jinyuanbaomall.cn/gtjpwvdhbz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.wangshuangyany.cn/gtmjtnbtvu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xinyue.icu/gtnzwtooem.html

================================================================================
来源：http://hz.wangdashe.top/gtrcrsjpvx.html

O. 并发与异步
来源：http://hz.guannengcc.top/gtfdjwfevh.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtfdbctazu.html

[O01] 启动一个线程
来源：http://hz.quarkkingdee.top/gtagbsyarz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.jinghuilouyu.cn/gtoshoobrd.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.guowangkeji.top/gtvkcirywq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.fzhhl.top/gtcklymitn.html

TS:   // 同 JS
来源：http://hz.daria6918.cn/gtulsznhov.html

Java: new Thread(() -> f()).start()
来源：http://hz.xinyue.icu/gtfaxxgcdy.html

Go:   go f()
来源：http://hz.jinqigufen.top/gtekgtsbgs.html

Ruby: Thread.new { f }
来源：http://hz.tian-w.cn/gtchzechkb.html

C#:   Task.Run(() => F());
来源：http://hz.guowangkeji.top/gtdlbiqeba.html

[O02] 使用线程池
来源：http://hz.shanyushiyangkeji.top/gtqyfpbysa.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.jiagoushi.top/gtcmmckbju.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.ywan-chungtsiang.top/gtdkedhtux.html

JS:   // worker_threads 线程池
来源：http://hz.feifeiyinyue.top/gtlciemwxu.html

TS:   // worker_threads 线程池
来源：http://hz.hysaishi.cn/gtczijfvlz.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.zhixingplan.top/gtznxkohkm.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.jlsjyb.cn/gtszdipxfc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.316326.xyz/gtpzilpbro.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.316326.xyz/gtfyomwcxi.html

[O03] 加锁保护共享数据
来源：http://hz.hnxiangtu.top/gtdhkiaunk.html

Py:   with lock: shared += 1
来源：http://hz.sxryk.cn/gtnhutuomo.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.nwbrower.top/gtezhjuewg.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.quarkkingdee.top/gtrlqgsvxe.html

TS:   // 同 JS
来源：http://hz.iojbl.cn/gtyuhuefol.html

Java: synchronized (this) { shared++; }
来源：http://hz.ydjk.org.cn/gtgasbuugy.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.cdnleiting.top/gtdtqhqfvz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jlsjyb.cn/gtrdlugrnu.html

C#:   lock (gate) { shared++; }
来源：http://hz.jinghuilouyu.cn/gtioaakgre.html

[O04] 定义异步函数并等待
来源：http://hz.jiagoushi.top/gtdqqhuhcx.html

Py:   async def f():⏎    await g()
来源：http://hz.yongpay.top/gtkqlyhvjv.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.nwbrower.top/gtcajhtbuf.html

JS:   async function f() { await g(); }
来源：http://hz.yonumen.top/gtywubsktw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.tanke756.top/gtzwibvywe.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.hnqzz.top/gtzfnsvcys.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.hammf.cn/gtduytlyvy.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.hywenlv.cn/gtgbgoyddp.html

C#:   async Task F() { await G(); }
来源：http://hz.nanxuanxn.top/gtbglmdbqz.html

[O05] 并发执行并等待全部完成
来源：http://hz.ppjwa.cn/gtuhcqkoex.html

Py:   asyncio.gather(*tasks)
来源：http://hz.xinyue.icu/gtlccusmen.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.gogol.net.cn/gtoduewbzm.html

JS:   await Promise.all(tasks)
来源：http://hz.havefunace.top/gtpujwkaad.html

TS:   await Promise.all(tasks)
来源：http://hz.jinghuilouyu.cn/gtfbnvdixq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.xuetiantiany.cn/gtbbcyzxul.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.hywenlv.cn/gtztrisweq.html

Ruby: threads.map(&:join)
来源：http://hz.gogol.net.cn/gtsjmpfvqt.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.cheryme.top/gtfkbrcqwr.html

[O06] 使用进程池
来源：http://hz.yongpay.top/gtiycyumxl.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.meibo888.top/gtbuaukpfs.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.yanxiufei.cn/gtqvfpusqr.html

JS:   // child_process / cluster 模块
来源：http://hz.zhiwuduotai.top/gttpkuhist.html

TS:   // child_process / cluster 模块
来源：http://hz.zycfv.cn/gtwyqbbhzs.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.zdqjudy.top/gtjxhwprzn.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.ywan-chungtsiang.top/gtsewmxdok.html

Ruby: // fork 块
来源：http://hz.ivvv.top/gtthyhczon.html

C#:   Parallel.For
来源：http://hz.jyoumei.cn/gtmjagvmwy.html

================================================================================
来源：http://hz.c1oappe.top/gtflmijjkq.html

P. 常用工具函数
来源：http://hz.c1oappe.top/gtykcpbdng.html

================================================================================
来源：http://hz.redwolf501.top/gtstywogve.html

[P01] 生成 UUID
来源：http://hz.yongpay.top/gthykphrjt.html

Py:   str(uuid.uuid4())
来源：http://hz.shzxlz.cn/gtnxgvirmw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.nanxuanxn.top/gthcqygmkq.html

JS:   crypto.randomUUID()
来源：http://hz.gogol.net.cn/gtarcxobqq.html

TS:   crypto.randomUUID()
来源：http://hz.havefunace.top/gtsdfcondt.html

Java: UUID.randomUUID().toString()
来源：http://hz.shangyingyoupin.top/gtgorckyty.html

Go:   // 用 github.com/google/uuid
来源：http://hz.bjfxy.top/gtaussmnma.html

Ruby: SecureRandom.uuid
来源：http://hz.gotoacloud.top/gtkbkewfdl.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.chenlongwang.top/gtdirnwnpe.html

[P02] MD5 / SHA256 摘要
来源：http://hz.snrcjt.cn/gtknzbimbx.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.svipenyu.cn/gtkmzjlwil.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.jyoumei.cn/gtxcjbscwe.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yj202588.top/gtnbvisorv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.zhixingplan.top/gtfusjddwo.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.cashguo.top/gttzqfungo.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.ydjk.org.cn/gtnwossyqx.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.feifeiyinyue.top/gtmswzvxpq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.cashguo.top/gttctlyfse.html

[P03] 生成短随机字符串
来源：http://hz.quarkkingdee.top/gtsxfuwuuu.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.xingfuxueyuan.xyz/gtkwmkexkr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.yongpay.top/gtfqnmzhlx.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.haohaochexian.top/gtkmrqlzjp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.chenzaomai.com/gtqvggykjs.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jqgfzy.top/gtqzbfpamx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.meibo888.top/gtdudrmojb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.c1oappe.top/gtyrvguxyg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.nanxuanxn.top/gttqzlsxxo.html

[P04] 求长度
来源：http://hz.feifeiyinyue.top/gtedtydowo.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.hnqzz.top/gtcplrsidm.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.52xcode.cn/gtzxjzgyuk.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ivvv.top/gtsgqhkhxq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.daria6918.cn/gtgzsunqtv.html

Java: list.size();  map.size();  s.length()
来源：http://hz.yueranfly.top/gtqhpgaccy.html

Go:   len(arr);  len(m)
来源：http://hz.jqgufenzy.top/gtdxusgwrl.html

Ruby: x.length;  x.size
来源：http://hz.daria6918.cn/gtoihlzxpu.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.yj20258888.top/gtazgvwbpu.html

[P05] 判断两个对象内容是否相等
来源：http://hz.mhx1999.top/gtzalmzdqn.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.ywan-chungtsiang.top/gtxajevuzb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.daxiang520.top/gtnofoolnv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.0kj1m.cn/gtedspskgv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.shanyushiyangkeji.top/gtziivtfkj.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.sweek.top/gtgngfnkdx.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.daria6918.cn/gteujaisig.html

Ruby: a == b
来源：http://hz.haohaochexian.top/gtunnnyefp.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.sysykeji.top/gtxzmrjawe.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.cheryme.top/gtdffpkpmo.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.aizwys.cn/gtezagmepu.html

PHP:  if (empty($x)) {}
来源：http://hz.dashuyun.cn/gtgibwjmku.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.kuanghao11.cn/gtlpdnolyk.html

TS:   if (x == null) {}
来源：http://hz.sysykeji.top/gtwgdxccpv.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.mhx1999.top/gtkqahhslg.html

Go:   if x == nil {}
来源：http://hz.cheryme.top/gtqcbhhkid.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.shzxlz.cn/gtyjhdybhm.html

C#:   if (x is null) {}
来源：http://hz.ydzc1.top/gtvpdmxtav.html

[P07] 防抖与节流
来源：http://hz.gaohongyu789.top/gtnkiyyphz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.chenjidiqi.icu/gtkknexitr.html

PHP:  // 手写时间戳比较
来源：http://hz.0kj1m.cn/gtjhqndwar.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.fengsongda.top/gtrqkwcwfq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yangfankeji.com/gtkynlcpvt.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.nanxinkj.top/gtxsargeuq.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.yangfankeji.com/gtapstuhmw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.zhoulong.xyz/gtawmmdiow.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.yj20258.top/gtodzgqnnh.html

[P08] 处理浮点精度问题
来源：http://hz.tian-w.cn/gtneouziaj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.aibaodan.cn/gtaxgychzp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.xylfe.cn/gtzaxcixws.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.hongshengwenyu.top/gtgzqwjgmk.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.meibo888.top/gtdagnrnpn.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.xuetiantiany.cn/gtecwfeveq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.smart0.xyz/gtsfhvwpve.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.yj20258888.top/gtwidxzagv.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.jyoumei.cn/gtqndcjgyf.html

================================================================================
来源：http://hz.yuanzhike.top/gtyzkcszop.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.hnxiangtu.top/gtwcwoygcz.html

================================================================================
来源：http://hz.ehwqpu.com/gttioiglsz.html

[Q01] 创建表
来源：http://hz.yanxiufei.cn/gtdxtvekhy.html

CREATE TABLE users (
来源：http://hz.svipenyu.cn/gtiyamitlk.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.tianlin.xyz/gtllcgvpqg.html

name VARCHAR(50) NOT NULL,
来源：http://hz.cashguo.top/gtovbhumgs.html

email VARCHAR(100) UNIQUE,
来源：http://hz.guowangkeji.top/gtwpocflmb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.shuidangran.top/gtfjfsajwg.html

);
来源：http://hz.yj20258888.top/gtnrjrjdmm.html

[Q02] 创建带外键的表
来源：http://hz.zhixingplan.top/gtytyoailz.html

CREATE TABLE orders (
来源：http://hz.feifeiyinyue.top/gtxojdeyly.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhixingplan.top/gtwjuptvry.html

user_id INT NOT NULL,
来源：http://hz.gzhubu.top/gtkesjuxht.html

amount DECIMAL(10, 2),
来源：http://hz.cqqwz.cn/gtrkzlnpal.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.shangyingyoupin.top/gtygtghlfh.html

);
来源：http://hz.aizwys.cn/gtwjukbupa.html

[Q03] 增加列
来源：http://hz.cashguo.top/gtnfyolgyo.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.gotoacloud.top/gtvqefflum.html

[Q04] 修改列类型
来源：http://hz.gzhubu.top/gtahiypnuo.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.havefunace.top/gtymqxxafs.html

[Q05] 重命名列
来源：http://hz.guowangkeji.top/gtnhpcthdz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.hammf.cn/gtaqtwkfsi.html

[Q06] 删除列
来源：http://hz.yangfankeji.com/gtitrxwuze.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.ywan-chungtsiang.top/gtzcgkdwqm.html

[Q07] 删除表
来源：http://hz.daria6918.cn/gtliqtstpy.html

DROP TABLE IF EXISTS orders;
来源：http://hz.redwolf501.top/gtllkjwscc.html

[Q08] 创建普通索引
来源：http://hz.sufxvd.cn/gtxdmmlutf.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.c1oappe.top/gtgusjmecm.html

[Q09] 创建唯一索引
来源：http://hz.xingfuxueyuan.xyz/gtzpgsvcld.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.sweek.top/gtvoyvtshr.html

[Q10] 插入单行
来源：http://hz.shanyushiyangkeji.top/gtcaaqwlfd.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.gogol.net.cn/gttffylztq.html

[Q11] 一次插入多行
来源：http://hz.hnqzz.top/gtizhiddal.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.dianchejie.cn/gtrkvqprtp.html

[Q12] 插入后取自增 ID
来源：http://hz.jyoumei.cn/gtmywkwpwz.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.52xcode.cn/gtlgwziqvk.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.gaohongyu789.top/gtcbpbiphf.html

[Q13] 忽略重复插入
来源：http://hz.sufxvd.cn/gtgdhtjepp.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.andypj.xyz/gtlceobidk.html

[Q14] 存在则更新（upsert）
来源：http://hz.yongpay.top/gtoldrsxmw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.wangshuangyany.cn/gthxsznvvq.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.jiagoushi.top/gtuswlhopb.html

[Q15] 查询全部
来源：http://hz.wangshuangyany.cn/gtypglmunk.html

SELECT * FROM users;
来源：http://hz.hfpthk.cn/gtgghnitps.html

[Q16] 查询指定列
来源：http://hz.hfpthk.cn/gtljgxmnlh.html

SELECT id, name FROM users;
来源：http://hz.yonumen.top/gthqfxacbp.html

[Q17] 条件查询
来源：http://hz.xziqi.cn/gtkehghjio.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.vqdsnc.cn/gtrilquffo.html

[Q18] 模糊匹配
来源：http://hz.snrcjt.cn/gtnfmkesto.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yj202588.top/gtmxscvsrm.html

[Q19] 范围查询
来源：http://hz.jiagoushi.top/gtezpxadab.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.nanxuanxn.top/gtwequlubh.html

[Q20] IN 列表
来源：http://hz.shanyushiyangkeji.top/gtqaofvely.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.sweek.top/gteuaccgwy.html

[Q21] 空值判断
来源：http://hz.daxiang520.top/gtqcaqydsg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.hammf.cn/gthzwvbsqz.html

[Q22] 排序
来源：http://hz.ppjwa.cn/gtfjuknmng.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.9152youxi.cn/gtxoggwpjq.html

[Q23] 分页
来源：http://hz.zhixingplan.top/gtzkogyvii.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.zhaomingkeji.xyz/gtknnokxql.html

[Q24] 去重
来源：http://hz.xziqi.cn/gtokhpprcy.html

SELECT DISTINCT city FROM users;
来源：http://hz.ppjwa.cn/gtlyzozmvd.html

[Q25] 只取前 N 条
来源：http://hz.zhongyouzk.top/gtsxvmkrjb.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.zhaomingkeji.xyz/gtkcwlaeek.html

[Q26] 计数
来源：http://hz.gzhubu.top/gtpkzxxkrj.html

SELECT COUNT(*) FROM users;
来源：http://hz.chenzaomai.com/gtrirggcbe.html

[Q27] 条件计数
来源：http://hz.hnxiangtu.top/gtatpolcdp.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yonumen.top/gttkmajdue.html

[Q28] 求和与平均
来源：http://hz.meibo888.top/gtmelycayu.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.nanxuanxn.top/gtqbsjxfgh.html

[Q29] 最大最小值
来源：http://hz.sufxvd.cn/gtntkllffh.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.yueranfly.top/gtqohrlsts.html

[Q30] 分组统计
来源：http://hz.guannengcc.top/gtqrbcoaad.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.daria6918.cn/gtvopldzpl.html

[Q31] 分组后过滤
来源：http://hz.shanyushiyangkeji.top/gttxvanwuu.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.dashuyun.cn/gtorheuxfu.html

[Q32] 分组拼接字符串
来源：http://hz.zhixingplan.top/gttrvdxgme.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.quarkkingdee.top/gtebtixoxt.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yongpay.top/gtvxqfoiii.html

[Q33] 多列分组
来源：http://hz.zdqjudy.top/gthfdqegpn.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.hnxiangtu.top/gtziaumoav.html

[Q34] 每组取第一条
来源：http://hz.gogol.net.cn/gtggdpihmy.html

SELECT * FROM (
来源：http://hz.guannengcc.top/gtimzhdqzi.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.ivvv.top/gtzwfqxhan.html

) t WHERE rn = 1;
来源：http://hz.iojbl.cn/gtrnyxdudi.html

[Q35] 内连接
来源：http://hz.0kj1m.cn/gtduhgjiox.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.quarkkingdee.top/gtybidvcqq.html

[Q36] 左连接
来源：http://hz.sysykeji.top/gtbyucqspf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.shuidangran.top/gtpfgvtjgu.html

[Q37] 右连接
来源：http://hz.quarkkingdee.top/gthccyxoth.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.shanyushiyangkeji.top/gthsgvrmti.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.sufxvd.cn/gtjgjndvqo.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.zhaomingkeji.xyz/gtyovbaszu.html

[Q39] 自连接（查上下级）
来源：http://hz.zhiwuduotai.top/gteuhkfrbu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.pengpengdd.cyou/gtunzuckwg.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.hysaishi.cn/gtfhuxwlih.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.sysykeji.top/gtnlxqowhb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.zhaomingkeji.xyz/gteeenjvvm.html

[Q41] 多表连接
来源：http://hz.zhixingplan.top/gtbigonmta.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.sweek.top/gtechmqqrz.html

JOIN users u ON u.id = o.user_id
来源：http://hz.ydzc1.top/gttulyjdjb.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.jiagoushi.top/gtcxkgwysd.html

[Q42] 连接条件附加过滤
来源：http://hz.xuanzx.com/gtxbqpsgbk.html

SELECT u.name, o.amount FROM users u
来源：http://hz.xziqi.cn/gtejbkyfeb.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.shangyingyoupin.top/gtxhtzcvtl.html

[Q43] 标量子查询
来源：http://hz.316326.xyz/gtcrladbqe.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yvedp.cn/gtfuwrjbnv.html

[Q44] IN 子查询
来源：http://hz.ydjk.org.cn/gtphutpaaf.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.xziqi.cn/gtplougfyu.html

[Q45] EXISTS 判断存在
来源：http://hz.feifeiyinyue.top/gtrwfwuriv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.shanyushiyangtech.top/gtmxwksuib.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.gaohongyu789.top/gtmmmtfdnh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.sxryk.cn/gtqhieywrw.html

[Q47] 与平均值比较
来源：http://hz.yuxming.cn/gtaaimyhza.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.snrcjt.cn/gtwmhyoacf.html

[Q48] CTE 公用表表达式
来源：http://hz.jinqigufen.top/gtnuuqehtr.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.cashguo.top/gtmyoetiha.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.dashuyun.cn/gtrfnijmyn.html

[Q49] 更新单行
来源：http://hz.havefunace.top/gtvautcvnw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.jinqigfzy.top/gtbisuvjkl.html

[Q50] 批量更新
来源：http://hz.chenlongwang.top/gtesdhlkyt.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.jianghu66.top/gtenydyysn.html

[Q51] 用子查询更新
来源：http://hz.cdnleiting.top/gtiecurrey.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.feifeiyinyue.top/gtevvqltew.html

[Q52] 删除指定行
来源：http://hz.redwolf501.top/gtexknvpab.html

DELETE FROM users WHERE id = 10;
来源：http://hz.tianlin.xyz/gtysvryvfd.html

[Q53] 按条件删除
来源：http://hz.snrcjt.cn/gtvjnkzfpi.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.havefunace.top/gtepnlkoms.html

[Q54] 清空表
来源：http://hz.hammf.cn/gtyiqvvpws.html

TRUNCATE TABLE logs;
来源：http://hz.tianlin.xyz/gtancdwccc.html

[Q55] 排名（并列占位）
来源：http://hz.bjfxy.top/gtcrmkquqr.html


<!-- 参考信息 -->