代发 wailian999

Go:   // 手写 map[int]int
来源：http://hz.cqqwz.cn/gtxqztjljm.html

Ruby: // 手写 Hash
来源：http://hz.cheryme.top/gtfgrhjwee.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yuanzhike.top/gtbrkthnnw.html

[N08] 生成全排列
来源：http://hz.redwolf501.top/gtxeayiift.html

Py:   itertools.permutations(arr)
来源：http://hz.hnxiangtu.top/gtqvzxmcgi.html

PHP:  // 手写递归交换
来源：http://hz.ppjwa.cn/gtawzkuzad.html

JS:   // 手写回溯递归
来源：http://hz.svipenyu.cn/gtpghdbfvh.html

TS:   // 手写回溯递归
来源：http://hz.svipenyu.cn/gtdxqxpxja.html

Java: // 手写回溯递归
来源：http://hz.cucudq.cn/gtpdvbwkrt.html

Go:   // 手写回溯递归
来源：http://hz.yonumen.top/gtrawhnmth.html

Ruby: arr.permutation.to_a
来源：http://hz.hysaishi.cn/gtytpaalkb.html

C#:   // 手写回溯递归
来源：http://hz.dianchejie.cn/gtnajyyyfm.html

[N09] 栈与队列
来源：http://hz.daria6918.cn/gtiinwrhho.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yj202588.top/gtneehdddq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.pengpengdd.cyou/gtubqfnwmi.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zhoulong.xyz/gtbjhojizb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.xylfe.cn/gtolffreoa.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yuanzhike.top/gtscrvcurv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.svipenyu.cn/gtnurogdbu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.quarkkingdee.top/gtrdqjgrmz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.shzxlz.cn/gtaobxxxqf.html

[N10] 链表节点定义
来源：http://hz.jqgufenzy.top/gtrtpjpwnp.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.0kj1m.cn/gthdtohmjs.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.birdmap.top/gtnoxaltvr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.0kj1m.cn/gtflgdvxmq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.feifeiyinyue.top/gtzqmcqxdg.html

Java: class Node { int v; Node next; }
来源：http://hz.wangdashe.top/gtwvlxlnhy.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.sysykeji.top/gtybmlbrqb.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.aibaodan.cn/gtehkrpfge.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.ppjwa.cn/gthexvxqpy.html

[N11] 二叉树中序遍历
来源：http://hz.xuetiantiany.cn/gtbwfhcvvc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.jqgufenzy.top/gtvvksqdpo.html

PHP:  // 手写递归函数
来源：http://hz.shanyushiyangtech.top/gtesktqwte.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hnqzz.top/gtnxmemvjm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.guowangkeji.top/gtgtylklmd.html

Java: // 手写递归
来源：http://hz.zdqjudy.top/gtsaztqznd.html

Go:   // 手写递归
来源：http://hz.zhijiandao.cn/gtohcjnucu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.zycfv.cn/gtvdqqojep.html

C#:   // 手写递归
来源：http://hz.yueranfly.top/gtipgturkk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.0kj1m.cn/gttvsyhxmt.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.mhx1999.top/gtrjeobvje.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jinyuanbaomall.cn/gteefyshha.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.daria6918.cn/gtgbqmpulq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.dianchejie.cn/gtpsrkxnls.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.wangshuangyany.cn/gtosjdlevj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.dianchejie.cn/gtmajgifaw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.c1oappe.top/gtmbhvyfui.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.sysykeji.top/gttymrdomg.html

================================================================================
来源：http://hz.jyoumei.cn/gtxrahbruo.html

O. 并发与异步
来源：http://hz.hnqzz.top/gtecwzisif.html

================================================================================
来源：http://hz.cqqwz.cn/gtdemldobe.html

[O01] 启动一个线程
来源：http://hz.yueranfly.top/gtbowdcnuz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.ydzc1.top/gtfereyzgu.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.xinyue.icu/gtdmjknzfz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.ywan-chungtsiang.top/gtcqgiheoz.html

TS:   // 同 JS
来源：http://hz.xylfe.cn/gtrvdddmbi.html

Java: new Thread(() -> f()).start()
来源：http://hz.xziqi.cn/gtbghsvhru.html

Go:   go f()
来源：http://hz.shzxlz.cn/gtjyvsdghb.html

Ruby: Thread.new { f }
来源：http://hz.xuanzx.com/gtelbfjsbm.html

C#:   Task.Run(() => F());
来源：http://hz.aizwys.cn/gtcqvchhsw.html

[O02] 使用线程池
来源：http://hz.yj202588.top/gtgwqnzraz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.snrcjt.cn/gtwwiugeeu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.andypj.xyz/gtcqmxtymk.html

JS:   // worker_threads 线程池
来源：http://hz.chenzaomai.com/gtnmnqjqzy.html

TS:   // worker_threads 线程池
来源：http://hz.jinghuilouyu.cn/gtmqjglbdf.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.hysaishi.cn/gtrxsgsawy.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.hongshengwenyu.top/gtgecvjloy.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.ppjwa.cn/gtoblstpso.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.guannengcc.top/gtuebwewho.html

[O03] 加锁保护共享数据
来源：http://hz.yj202588.top/gtefgwbyya.html

Py:   with lock: shared += 1
来源：http://hz.shanyushiyangtech.top/gtowdiqatx.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.yongpay.top/gtyvbwgbpu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.haohaochexian.top/gtdgosniqg.html

TS:   // 同 JS
来源：http://hz.316326.xyz/gtmeflqavp.html

Java: synchronized (this) { shared++; }
来源：http://hz.yj20258888.top/gtychpaiih.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yvedp.cn/gtbssuhhdq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.haohaochexian.top/gttrnvffzk.html

C#:   lock (gate) { shared++; }
来源：http://hz.yongpay.top/gtvdconlxm.html

[O04] 定义异步函数并等待
来源：http://hz.kuanghao11.cn/gtomnnqiko.html

Py:   async def f():⏎    await g()
来源：http://hz.meibo888.top/gthuficuaa.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.hnqzz.top/gtcfnodifz.html

JS:   async function f() { await g(); }
来源：http://hz.tian-w.cn/gtxbswnkpq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.ppjwa.cn/gtmkmtvbnm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.gzhubu.top/gtoshimqng.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.ppjwa.cn/gteigklqab.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yonumen.top/gtgmttmqjx.html

C#:   async Task F() { await G(); }
来源：http://hz.meibo888.top/gtczzamxns.html

[O05] 并发执行并等待全部完成
来源：http://hz.ivvv.top/gtldsmavzu.html

Py:   asyncio.gather(*tasks)
来源：http://hz.xuanzx.com/gtnvaxotdh.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.yj20258.top/gtghzixmkf.html

JS:   await Promise.all(tasks)
来源：http://hz.fengsongda.top/gtkfawqswv.html

TS:   await Promise.all(tasks)
来源：http://hz.sweek.top/gtudygrjul.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.yueranfly.top/gtxqasvomo.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.chenjidiqi.icu/gtjozqfois.html

Ruby: threads.map(&:join)
来源：http://hz.ywan-chungtsiang.top/gtbwpduznb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.svipenyu.cn/gtnniwwdoq.html

[O06] 使用进程池
来源：http://hz.tian-w.cn/gtomlduktc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.haohaochexian.top/gtyuldodpt.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.9152youxi.cn/gtkddnupie.html

JS:   // child_process / cluster 模块
来源：http://hz.nanxinkj.top/gtesrvnmmu.html

TS:   // child_process / cluster 模块
来源：http://hz.yonumen.top/gtzdpbifkt.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.shanyushiyangkeji.top/gtlqsixfup.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.0kj1m.cn/gtfsdrpede.html

Ruby: // fork 块
来源：http://hz.nwbrower.top/gtratlcnub.html

C#:   Parallel.For
来源：http://hz.ydjk.org.cn/gthapphoyk.html

================================================================================
来源：http://hz.xziqi.cn/gtlbiwshxq.html

P. 常用工具函数
来源：http://hz.zhijiandao.cn/gtwkgjtsoa.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtpywithli.html

[P01] 生成 UUID
来源：http://hz.sweek.top/gtzxsbugnu.html

Py:   str(uuid.uuid4())
来源：http://hz.yongpay.top/gttzlhiaaz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.hnqzz.top/gtmdyaxftx.html

JS:   crypto.randomUUID()
来源：http://hz.ivvv.top/gtyniibdzl.html

TS:   crypto.randomUUID()
来源：http://hz.ivvv.top/gtdvvingrj.html

Java: UUID.randomUUID().toString()
来源：http://hz.haohaochexian.top/gtgusioqlu.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yueranfly.top/gtdjmcaoeb.html

Ruby: SecureRandom.uuid
来源：http://hz.wangdashe.top/gttsyofexl.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.yj20258.top/gthecybwmf.html

[P02] MD5 / SHA256 摘要
来源：http://hz.0kj1m.cn/gtajwvxwen.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.c1oappe.top/gthdzdwisw.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.wangdashe.top/gtzdhlceln.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.gotoacloud.top/gttpirooaw.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.hnqzz.top/gtaailvqsx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.jinqigfzy.top/gtgxubdfhj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.chenzaomai.com/gtxrdfwvar.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.wangdashe.top/gtlucmzymt.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.snrcjt.cn/gtngkplnuz.html

[P03] 生成短随机字符串
来源：http://hz.hnqzz.top/gtvctqvmhu.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.shanyushiyangtech.top/gtjakxmqub.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.tanke756.top/gtkghmiwxb.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xuetiantiany.cn/gtfqlndlgi.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.0kj1m.cn/gtwbtbkgfk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.sysykeji.top/gtzooqrfuy.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.shuidangran.top/gtcwbwtnao.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.haohaochexian.top/gtwptuldqw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.dashuyun.cn/gtqswyzovv.html

[P04] 求长度
来源：http://hz.havefunace.top/gtnzeeyxyr.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.gogol.net.cn/gtqxrslzjx.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shuidangran.top/gtaffrwzjs.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.fzhhl.top/gthxupaaeg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.daxiang520.top/gtwvcrqdza.html

Java: list.size();  map.size();  s.length()
来源：http://hz.sxryk.cn/gtnirpfnge.html

Go:   len(arr);  len(m)
来源：http://hz.0kj1m.cn/gtkqygdahq.html

Ruby: x.length;  x.size
来源：http://hz.bjfxy.top/gtaqumskpo.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.cashguo.top/gtrbcmiamo.html

[P05] 判断两个对象内容是否相等
来源：http://hz.shuidangran.top/gthegxckkf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.52xcode.cn/gtxhanrbml.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.shanyushiyangkeji.top/gtygcuhkze.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.birdmap.top/gtqjisjttz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yvedp.cn/gtildasxkv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.cheryme.top/gtratnscxs.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.guannengcc.top/gtppokzafd.html

Ruby: a == b
来源：http://hz.jinqigufen.top/gturkqqftw.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.jyoumei.cn/gtikrnhenn.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.fzhhl.top/gtbraokbpw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.shzxlz.cn/gtifizdymf.html

PHP:  if (empty($x)) {}
来源：http://hz.nanxuanxn.top/gtjimgbaow.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.ehwqpu.com/gtaurhhuek.html

TS:   if (x == null) {}
来源：http://hz.smart0.xyz/gtemqhwqdr.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.0kj1m.cn/gtxbefodqr.html

Go:   if x == nil {}
来源：http://hz.chenzaomai.com/gtcxklneap.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.wangdashe.top/gtoxsjvpvn.html

C#:   if (x is null) {}
来源：http://hz.ywan-chungtsiang.top/gtqmqkxflz.html

[P07] 防抖与节流
来源：http://hz.jlsjyb.cn/gtdrwqnahg.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.zhoulong.xyz/gtnqorqinv.html

PHP:  // 手写时间戳比较
来源：http://hz.0kj1m.cn/gtwbmkonio.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.meibo888.top/gtfuzutzru.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhongyouzk.top/gtdvcukwnf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.quarkkingdee.top/gtiamsojvj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.cashguo.top/gtuxycnemp.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.pengpengdd.cyou/gttvayulwa.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.xingfuxueyuan.xyz/gtgkhzuagt.html

[P08] 处理浮点精度问题
来源：http://hz.guowangkeji.top/gtcfjojhfm.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jinqigfzy.top/gtdtmzxghs.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.zhixingplan.top/gtlehwsxfq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.cheryme.top/gtlqelutke.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.redwolf501.top/gtadsrqogw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yj202588.top/gtwnccuzjg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.svipenyu.cn/gtrgdacvre.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.yj202588.top/gtqwghiksf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.dianchejie.cn/gtzuyvamkr.html

================================================================================
来源：http://hz.ppjwa.cn/gtihqjlpoy.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.vqdsnc.cn/gtkpfhqjxx.html

================================================================================
来源：http://hz.nwbrower.top/gtrmyeoozv.html

[Q01] 创建表
来源：http://hz.dashuyun.cn/gtqcepvrkf.html

CREATE TABLE users (
来源：http://hz.ivvv.top/gtyhzqirwf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yangfankeji.com/gtnpdrwmpl.html

name VARCHAR(50) NOT NULL,
来源：http://hz.9152youxi.cn/gtlezlmhrk.html

email VARCHAR(100) UNIQUE,
来源：http://hz.andypj.xyz/gtlxhwzwit.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.zycfv.cn/gthrpjcoxg.html

);
来源：http://hz.jiagoushi.top/gtyaydukbc.html

[Q02] 创建带外键的表
来源：http://hz.nanxuanxn.top/gtdnyfswuy.html

CREATE TABLE orders (
来源：http://hz.shzxlz.cn/gtxxczcmir.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hysaishi.cn/gtdritzdvw.html

user_id INT NOT NULL,
来源：http://hz.sxryk.cn/gtdnqayltl.html

amount DECIMAL(10, 2),
来源：http://hz.cucudq.cn/gtlfhsdrxu.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.chenjidiqi.icu/gtccjebmzz.html

);
来源：http://hz.zhijiandao.cn/gttellvcey.html

[Q03] 增加列
来源：http://hz.guowangkeji.top/gtfiuqpnkc.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.zhoulong.xyz/gtfipxlpga.html

[Q04] 修改列类型
来源：http://hz.jyoumei.cn/gtbwfhvjrj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.gogol.net.cn/gtdflbfrpi.html

[Q05] 重命名列
来源：http://hz.daxiang520.top/gttxhkrcrt.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.hywenlv.cn/gtyyjaovvk.html

[Q06] 删除列
来源：http://hz.shuidangran.top/gtpurdmksy.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.havefunace.top/gtvfkbavvp.html

[Q07] 删除表
来源：http://hz.gotoacloud.top/gtepgmucqj.html

DROP TABLE IF EXISTS orders;
来源：http://hz.sufxvd.cn/gtorolurut.html

[Q08] 创建普通索引
来源：http://hz.hysaishi.cn/gtyjbqiuos.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.yueranfly.top/gtxmzqxggt.html

[Q09] 创建唯一索引
来源：http://hz.fengsongda.top/gtqnvabfmk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.yueranfly.top/gtfvvrgfxs.html

[Q10] 插入单行
来源：http://hz.daxiang520.top/gtifarjxcw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.yj20258888.top/gtsytcxzks.html

[Q11] 一次插入多行
来源：http://hz.yvedp.cn/gtinwpevly.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.svipenyu.cn/gtfaysqwca.html

[Q12] 插入后取自增 ID
来源：http://hz.zhixingplan.top/gtrnvxmara.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.pengpengdd.cyou/gtextqrcox.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.ydjk.org.cn/gthpritsfa.html

[Q13] 忽略重复插入
来源：http://hz.0kj1m.cn/gtktfrkpzh.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.chenlongwang.top/gtfoqtbazz.html

[Q14] 存在则更新（upsert）
来源：http://hz.9152youxi.cn/gtwjluelxr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.shanyushiyangtech.top/gtjmcopnxz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.gogol.net.cn/gtqhsapvkn.html

[Q15] 查询全部
来源：http://hz.ydjk.org.cn/gtwuwvtakv.html

SELECT * FROM users;
来源：http://hz.sysykeji.top/gtdxhxuekn.html

[Q16] 查询指定列
来源：http://hz.yanxiufei.cn/gtqynfjpjv.html

SELECT id, name FROM users;
来源：http://hz.xinyue.icu/gtjizarrbx.html

[Q17] 条件查询
来源：http://hz.snrcjt.cn/gtppetfvao.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.0kj1m.cn/gtxwvecegb.html

[Q18] 模糊匹配
来源：http://hz.c1oappe.top/gtfvcflsik.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.zhengqikj.top/gtxebsjboh.html

[Q19] 范围查询
来源：http://hz.nanxinkj.top/gttttbfzwq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.shuidangran.top/gtvssjnbsz.html

[Q20] IN 列表
来源：http://hz.wangdashe.top/gtivdcvtkv.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.ivvv.top/gtpteehhld.html

[Q21] 空值判断
来源：http://hz.zhongyouzk.top/gtqoicjhdx.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.xylfe.cn/gtkgpgcmtw.html

[Q22] 排序
来源：http://hz.gaohongyu789.top/gtxpcwsdsc.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.pycfn.com/gtpiiijpse.html

[Q23] 分页
来源：http://hz.ehwqpu.com/gtsmrdyhjq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.zycfv.cn/gtgwdfrhly.html

[Q24] 去重
来源：http://hz.xingfuxueyuan.xyz/gtmwphbcyh.html

SELECT DISTINCT city FROM users;
来源：http://hz.yj20258.top/gtmhxsgguc.html

[Q25] 只取前 N 条
来源：http://hz.jqgufenzy.top/gtomfsopmn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.jinyuanbaomall.cn/gtpnretsnr.html

[Q26] 计数
来源：http://hz.dashuyun.cn/gtponqawqi.html

SELECT COUNT(*) FROM users;
来源：http://hz.ydjk.org.cn/gtvrvihcsz.html

[Q27] 条件计数
来源：http://hz.52xcode.cn/gtwmvvqucw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.zhaomingkeji.xyz/gtisgxaqij.html

[Q28] 求和与平均
来源：http://hz.shanyushiyangkeji.top/gtplxxpauq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.iojbl.cn/gtktrvgpfs.html

[Q29] 最大最小值
来源：http://hz.hammf.cn/gtdaafezvi.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.jyoumei.cn/gtoybqfans.html

[Q30] 分组统计
来源：http://hz.jqgufenzy.top/gtfsjwogxx.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.zhaomingkeji.xyz/gtzgyicjvd.html

[Q31] 分组后过滤
来源：http://hz.tian-w.cn/gtyktfbmsh.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.xuanzx.com/gtshyrvonz.html

[Q32] 分组拼接字符串
来源：http://hz.ywan-chungtsiang.top/gtgrkoudyv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.birdmap.top/gtpbdvrmqd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.mhx1999.top/gtprxcbgrh.html

[Q33] 多列分组
来源：http://hz.52xcode.cn/gtslpmwydo.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.andypj.xyz/gtvhsopctg.html

[Q34] 每组取第一条
来源：http://hz.cashguo.top/gtauhpnsja.html

SELECT * FROM (
来源：http://hz.cheryme.top/gtckdjqytm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.yj202588.top/gtbmqyxeqm.html

) t WHERE rn = 1;
来源：http://hz.meibo888.top/gtburmkxji.html

[Q35] 内连接
来源：http://hz.shuidangran.top/gtagkpyvie.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.yuanzhike.top/gtwtjvqhaw.html

[Q36] 左连接
来源：http://hz.hammf.cn/gtgttqqycf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.hysaishi.cn/gtsbgfbtjb.html

[Q37] 右连接
来源：http://hz.hammf.cn/gtnuajojar.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.shanyushiyangtech.top/gtycbbfdcz.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.yonumen.top/gthuroldne.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.yj202588.top/gtjjcqzclt.html

[Q39] 自连接（查上下级）
来源：http://hz.shanyushiyangtech.top/gtwxrqnopr.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.tianlin.xyz/gtzkutwkbb.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.ivvv.top/gtvgpidqcg.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.jiagoushi.top/gtoxbbycph.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.andypj.xyz/gtzpvyrtbw.html

[Q41] 多表连接
来源：http://hz.gotoacloud.top/gtvrxutybz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.tanke756.top/gtlvornjpp.html

JOIN users u ON u.id = o.user_id
来源：http://hz.chenlongwang.top/gtncrfqfmb.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.gogol.net.cn/gtbzpkqevn.html

[Q42] 连接条件附加过滤
来源：http://hz.0kj1m.cn/gtkbtbkfvm.html

SELECT u.name, o.amount FROM users u
来源：http://hz.zhengqikj.top/gtegekfmlt.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.zhongyouzk.top/gtwzzdcaxe.html

[Q43] 标量子查询
来源：http://hz.ywan-chungtsiang.top/gtcrsshbkl.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.jinqigfzy.top/gthvsuzduy.html

[Q44] IN 子查询
来源：http://hz.ydzc1.top/gtmeujywym.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.dashuyun.cn/gtiuiealwo.html

[Q45] EXISTS 判断存在
来源：http://hz.andypj.xyz/gtpyqhjugq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.ivvv.top/gtplolayky.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yanxiufei.cn/gtmtukhuyy.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hfpthk.cn/gtbsserjhd.html

[Q47] 与平均值比较
来源：http://hz.fzhhl.top/gtcwqmsvic.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.sysykeji.top/gtfrtihdqr.html

[Q48] CTE 公用表表达式
来源：http://hz.gogol.net.cn/gtjxklnsmh.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.cqqwz.cn/gtzecnxawc.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.xziqi.cn/gtcawejwvi.html

[Q49] 更新单行
来源：http://hz.guowangkeji.top/gtpmowrorp.html


<!-- 参考信息 -->