代发 wailian999

Go:   // 手写 map[int]int
来源：http://hz.mhx1999.top/gtcrzkrvpf.html

Ruby: // 手写 Hash
来源：http://hz.dashuyun.cn/gtkargnpnn.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.zhixingplan.top/gtbfnveomo.html

[N08] 生成全排列
来源：http://hz.hongshengwenyu.top/gtcskelfrb.html

Py:   itertools.permutations(arr)
来源：http://hz.cqqwz.cn/gttehhcnll.html

PHP:  // 手写递归交换
来源：http://hz.hammf.cn/gtypdqykeb.html

JS:   // 手写回溯递归
来源：http://hz.xinyue.icu/gtnntbnswo.html

TS:   // 手写回溯递归
来源：http://hz.iojbl.cn/gtdcfvfgbt.html

Java: // 手写回溯递归
来源：http://hz.sufxvd.cn/gtaglclfyv.html

Go:   // 手写回溯递归
来源：http://hz.birdmap.top/gtqskomawg.html

Ruby: arr.permutation.to_a
来源：http://hz.cucudq.cn/gtnjrohoag.html

C#:   // 手写回溯递归
来源：http://hz.9152youxi.cn/gtqfpygwhj.html

[N09] 栈与队列
来源：http://hz.chenlongwang.top/gtupwjllcp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.jlsjyb.cn/gtdnnbxybi.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.aizwys.cn/gtnxbevags.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zdqjudy.top/gtdkhjdxwq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jinqigufen.top/gtqlwoiyfc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.jinqigufen.top/gtdrptvaii.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.hnxiangtu.top/gtjqthaiuv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.hnqzz.top/gtiyxeemzw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.jqgfzy.top/gthveulrya.html

[N10] 链表节点定义
来源：http://hz.andypj.xyz/gtnbmjpgjx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.hnxiangtu.top/gtvukkonih.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.cqqwz.cn/gtridikwaa.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yj20258888.top/gtmezsuhwa.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.redwolf501.top/gtgmcznaue.html

Java: class Node { int v; Node next; }
来源：http://hz.hywenlv.cn/gtouksyhhd.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.wangshuangyany.cn/gtmlxeiozg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.yj20258888.top/gtszusutvo.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.gogol.net.cn/gthtkhpjwe.html

[N11] 二叉树中序遍历
来源：http://hz.shanyushiyangkeji.top/gtmcqktrri.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.jinghuilouyu.cn/gtlhuchbdo.html

PHP:  // 手写递归函数
来源：http://hz.zhoulong.xyz/gtkvmihhwe.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.cucudq.cn/gtwscyufci.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ydjk.org.cn/gtmtmkukkh.html

Java: // 手写递归
来源：http://hz.zhaomingkeji.xyz/gtzalvlnqs.html

Go:   // 手写递归
来源：http://hz.feifeiyinyue.top/gtvdsszkvv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.yj20258888.top/gtaqwphtan.html

C#:   // 手写递归
来源：http://hz.cqqwz.cn/gtolbhemlv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.haohaochexian.top/gtnhjamrjz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.gogol.net.cn/gtlmvswzlc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.hnqzz.top/gtkrcucuyk.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ppjwa.cn/gtfyynpnau.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xuetiantiany.cn/gtajunveqw.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.pengpengdd.cyou/gtzaxuwcvk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.quarkkingdee.top/gtwrvemvsc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.jianghu66.top/gtswroppna.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.c1oappe.top/gtgluoluxi.html

================================================================================
来源：http://hz.aibaodan.cn/gtvjmsydud.html

O. 并发与异步
来源：http://hz.havefunace.top/gtgokllonu.html

================================================================================
来源：http://hz.zycfv.cn/gtrfpndqkg.html

[O01] 启动一个线程
来源：http://hz.xylfe.cn/gtelbwftda.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.c1oappe.top/gtrbsztdgz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.gaohongyu789.top/gthpeudjpt.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.meibo888.top/gtavjmzmfq.html

TS:   // 同 JS
来源：http://hz.tian-w.cn/gtzplwwcnh.html

Java: new Thread(() -> f()).start()
来源：http://hz.316326.xyz/gthmshtmdo.html

Go:   go f()
来源：http://hz.yj20258.top/gtamsnugpy.html

Ruby: Thread.new { f }
来源：http://hz.cqqwz.cn/gthwpdmuyk.html

C#:   Task.Run(() => F());
来源：http://hz.ydjk.org.cn/gtdefxrrej.html

[O02] 使用线程池
来源：http://hz.guannengcc.top/gtdcxefwos.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yueranfly.top/gtpfpixoxg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.guannengcc.top/gtxemblynh.html

JS:   // worker_threads 线程池
来源：http://hz.zycfv.cn/gtvakcvibt.html

TS:   // worker_threads 线程池
来源：http://hz.tian-w.cn/gtpmiwnvrf.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.aibaodan.cn/gtzlmygwol.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.redwolf501.top/gtnhpwxgax.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.hammf.cn/gtundqfexv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.xylfe.cn/gtipbpyebn.html

[O03] 加锁保护共享数据
来源：http://hz.bjfxy.top/gthbvsiwnd.html

Py:   with lock: shared += 1
来源：http://hz.jqgufenzy.top/gthubqtpef.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.fengsongda.top/gtnbjrerrg.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.cqqwz.cn/gtnjaskodv.html

TS:   // 同 JS
来源：http://hz.zycfv.cn/gtumyunfpw.html

Java: synchronized (this) { shared++; }
来源：http://hz.birdmap.top/gtdanqseag.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.daria6918.cn/gtneftjnzs.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.pengpengdd.cyou/gtihsxlpgy.html

C#:   lock (gate) { shared++; }
来源：http://hz.smart0.xyz/gtteufypzo.html

[O04] 定义异步函数并等待
来源：http://hz.snrcjt.cn/gtjypbewln.html

Py:   async def f():⏎    await g()
来源：http://hz.gzhubu.top/gtinlvxppj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jqgufenzy.top/gtueuyarqf.html

JS:   async function f() { await g(); }
来源：http://hz.chenlongwang.top/gtncvprsaa.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.gzhubu.top/gtvaorhnlm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.gogol.net.cn/gthptgtsdg.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.zhongyouzk.top/gtlwsjhixk.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.zhaomingkeji.xyz/gtusevsglk.html

C#:   async Task F() { await G(); }
来源：http://hz.hysaishi.cn/gtdlatyqio.html

[O05] 并发执行并等待全部完成
来源：http://hz.bjfxy.top/gtoloukrxw.html

Py:   asyncio.gather(*tasks)
来源：http://hz.hnxiangtu.top/gtjiipcyrp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.zhoulong.xyz/gtvmjwyuqz.html

JS:   await Promise.all(tasks)
来源：http://hz.chenlongwang.top/gtznwuphsy.html

TS:   await Promise.all(tasks)
来源：http://hz.shzxlz.cn/gthsycwaja.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.zhongyouzk.top/gtdufmznnq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.shanyushiyangkeji.top/gtnlhyivnl.html

Ruby: threads.map(&:join)
来源：http://hz.gotoacloud.top/gtrnoynmfr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.fengsongda.top/gtrrkzjmyf.html

[O06] 使用进程池
来源：http://hz.ydjk.org.cn/gtlovljohb.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.yonumen.top/gtavbuebwp.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.zhaomingkeji.xyz/gtuapvvwwe.html

JS:   // child_process / cluster 模块
来源：http://hz.haohaochexian.top/gtbkyqxnns.html

TS:   // child_process / cluster 模块
来源：http://hz.fzhhl.top/gtgkwtegjq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jlsjyb.cn/gtjoylrcba.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.zhongyouzk.top/gtrspchjnt.html

Ruby: // fork 块
来源：http://hz.aizwys.cn/gtodmjeecs.html

C#:   Parallel.For
来源：http://hz.cheryme.top/gtvmjpwxre.html

================================================================================
来源：http://hz.xuanzx.com/gtipeckybt.html

P. 常用工具函数
来源：http://hz.9152youxi.cn/gtokfgakfn.html

================================================================================
来源：http://hz.dashuyun.cn/gttbndllap.html

[P01] 生成 UUID
来源：http://hz.ehwqpu.com/gtjqdbutqc.html

Py:   str(uuid.uuid4())
来源：http://hz.ybcxt.top/gtztgqqrox.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jianghu66.top/gtusksjpza.html

JS:   crypto.randomUUID()
来源：http://hz.sweek.top/gtfflylpvq.html

TS:   crypto.randomUUID()
来源：http://hz.tianlin.xyz/gteezbtwvz.html

Java: UUID.randomUUID().toString()
来源：http://hz.mhx1999.top/gtelhdehcb.html

Go:   // 用 github.com/google/uuid
来源：http://hz.jinqigufen.top/gtkwixygwz.html

Ruby: SecureRandom.uuid
来源：http://hz.haohaochexian.top/gtyatrdyqk.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.shanyushiyangkeji.top/gtzptlsndz.html

[P02] MD5 / SHA256 摘要
来源：http://hz.sufxvd.cn/gtkgqlffzl.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.xingfuxueyuan.xyz/gtybqrnbsy.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.iojbl.cn/gthviygwtw.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.haohaochexian.top/gtixzqnkcr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.hnqzz.top/gtwicvddfa.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.daria6918.cn/gtrhtrxzqt.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.cqqwz.cn/gtrpvuxjhf.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.wangshuangyany.cn/gtwgzxvbnf.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.svipenyu.cn/gtmaujecnf.html

[P03] 生成短随机字符串
来源：http://hz.sweek.top/gtcymbeqzm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.aibaodan.cn/gtmfrmafkc.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.yj202588.top/gtverbqoed.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jqgufenzy.top/gtgnultllu.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhixingplan.top/gtxvjjvmmr.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.aibaodan.cn/gttqjqsqnm.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.snrcjt.cn/gtatzyztkl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jinqigufen.top/gtwxcyuwro.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jyoumei.cn/gtogvdwxad.html

[P04] 求长度
来源：http://hz.xuetiantiany.cn/gttyizbixc.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.yj20258.top/gtqqkoukmq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ywan-chungtsiang.top/gtqoccanhh.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.chenlongwang.top/gtzlhtipld.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.fengsongda.top/gtqcoisrtd.html

Java: list.size();  map.size();  s.length()
来源：http://hz.zhongyouzk.top/gtzldwhbcs.html

Go:   len(arr);  len(m)
来源：http://hz.jyoumei.cn/gtahqkpduk.html

Ruby: x.length;  x.size
来源：http://hz.yuxming.cn/gttnbgwajx.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.xuanzx.com/gtmgbkemfn.html

[P05] 判断两个对象内容是否相等
来源：http://hz.dashuyun.cn/gtpcukxjii.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.9152youxi.cn/gtondozkms.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.smart0.xyz/gtquobvhld.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.daxiang520.top/gthytjfyhi.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.aizwys.cn/gtswtseolq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.nanxuanxn.top/gtjeysfpnm.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.9152youxi.cn/gtuxsospla.html

Ruby: a == b
来源：http://hz.daxiang520.top/gtwiulxipq.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.tanke756.top/gtzfdgvyot.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.ybcxt.top/gtlywlafkh.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.wangdashe.top/gtmxxminqa.html

PHP:  if (empty($x)) {}
来源：http://hz.hfpthk.cn/gtcohhayrc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.ydzc1.top/gthgsyforq.html

TS:   if (x == null) {}
来源：http://hz.jinghuilouyu.cn/gtvmondsix.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.316326.xyz/gtbojygstk.html

Go:   if x == nil {}
来源：http://hz.zhiwuduotai.top/gtptbdeidb.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.ppjwa.cn/gthiqbpgxc.html

C#:   if (x is null) {}
来源：http://hz.chenzaomai.com/gtnkwrgudi.html

[P07] 防抖与节流
来源：http://hz.hywenlv.cn/gtdrfojgvt.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.iojbl.cn/gtnycuoiev.html

PHP:  // 手写时间戳比较
来源：http://hz.aizwys.cn/gtfosshyei.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.tian-w.cn/gtncthqucb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.daxiang520.top/gtbnluydqd.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.nwbrower.top/gtubyutsyd.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.gaohongyu789.top/gtuapmgwnp.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.0kj1m.cn/gtyxaaysrq.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.mhx1999.top/gtgvxrjmnp.html

[P08] 处理浮点精度问题
来源：http://hz.pengpengdd.cyou/gtnpiggyvf.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.wangdashe.top/gtcqtszmij.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.meibo888.top/gtdlcqxqaq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.hongshengwenyu.top/gtaoeukxrh.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.shanyushiyangtech.top/gtqyfclmxg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.xylfe.cn/gtbarennkl.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.zhixingplan.top/gttvxhugzj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.tianlin.xyz/gtzomaznhz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.aizwys.cn/gtubskxatr.html

================================================================================
来源：http://hz.ppjwa.cn/gtlazaqbxl.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.316326.xyz/gtyzdrwalg.html

================================================================================
来源：http://hz.jlsjyb.cn/gteocmwcqk.html

[Q01] 创建表
来源：http://hz.snrcjt.cn/gtnjodligh.html

CREATE TABLE users (
来源：http://hz.yj20258.top/gtnqwwxzuf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hfpthk.cn/gtrydjnzid.html

name VARCHAR(50) NOT NULL,
来源：http://hz.sxryk.cn/gtydynmfjr.html

email VARCHAR(100) UNIQUE,
来源：http://hz.yangfankeji.com/gtgbvtwtlr.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.ydjk.org.cn/gtjncosgdv.html

);
来源：http://hz.zhaomingkeji.xyz/gtabmenizu.html

[Q02] 创建带外键的表
来源：http://hz.jlsjyb.cn/gtynexmwrs.html

CREATE TABLE orders (
来源：http://hz.vqdsnc.cn/gtvvafugie.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jinqigufen.top/gtpzljvlba.html

user_id INT NOT NULL,
来源：http://hz.zhengqikj.top/gtfkueqhch.html

amount DECIMAL(10, 2),
来源：http://hz.tanke756.top/gtjpnzugym.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.hammf.cn/gtaoclmeee.html

);
来源：http://hz.hysaishi.cn/gtyiiltklp.html

[Q03] 增加列
来源：http://hz.ppjwa.cn/gthwfqbrsb.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.gaohongyu789.top/gtijuiwlla.html

[Q04] 修改列类型
来源：http://hz.nanxuanxn.top/gtjlgaunkn.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.cqqwz.cn/gtwbmagklz.html

[Q05] 重命名列
来源：http://hz.hongshengwenyu.top/gtzdvhdgfd.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.zhengqikj.top/gtlksgqmag.html

[Q06] 删除列
来源：http://hz.iojbl.cn/gtrwegelgr.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.xinyue.icu/gtrfsytwla.html

[Q07] 删除表
来源：http://hz.gzhubu.top/gtgzbzkyai.html

DROP TABLE IF EXISTS orders;
来源：http://hz.xuanzx.com/gtjavqtjwy.html

[Q08] 创建普通索引
来源：http://hz.hongshengwenyu.top/gtcksuoevv.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.ydzc1.top/gtorzprhno.html

[Q09] 创建唯一索引
来源：http://hz.fengsongda.top/gtcteyifvm.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.pengpengdd.cyou/gtbpxlovbk.html

[Q10] 插入单行
来源：http://hz.gaohongyu789.top/gtpcrdwngg.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.vqdsnc.cn/gtlgmosylt.html

[Q11] 一次插入多行
来源：http://hz.jqgfzy.top/gtutejlakn.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.daria6918.cn/gthfzgzufi.html

[Q12] 插入后取自增 ID
来源：http://hz.52xcode.cn/gtxbhzjvyd.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yj202588.top/gtvduyrbgl.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.zycfv.cn/gtwybpslae.html

[Q13] 忽略重复插入
来源：http://hz.tianlin.xyz/gtltgbutvo.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jinqigfzy.top/gtnhwdifzj.html

[Q14] 存在则更新（upsert）
来源：http://hz.ppjwa.cn/gtpakmpzye.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.xingfuxueyuan.xyz/gtgnfoexch.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.feifeiyinyue.top/gtlmmgruva.html

[Q15] 查询全部
来源：http://hz.yj20258.top/gtopxegabu.html

SELECT * FROM users;
来源：http://hz.nanxuanxn.top/gtclxcmkrp.html

[Q16] 查询指定列
来源：http://hz.ywan-chungtsiang.top/gtvrbxdape.html

SELECT id, name FROM users;
来源：http://hz.c1oappe.top/gtlplgehif.html

[Q17] 条件查询
来源：http://hz.ybcxt.top/gtlhkisbrm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.havefunace.top/gtgtqxyraj.html

[Q18] 模糊匹配
来源：http://hz.smart0.xyz/gtnwcfdoeo.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.sysykeji.top/gttentpjdz.html

[Q19] 范围查询
来源：http://hz.ydzc1.top/gtepeyjltk.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.gotoacloud.top/gtshqnfcju.html

[Q20] IN 列表
来源：http://hz.wangshuangyany.cn/gtdeydxvvr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yanxiufei.cn/gtmzchkoef.html

[Q21] 空值判断
来源：http://hz.c1oappe.top/gtutqqvmvs.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.ehwqpu.com/gtbuifijre.html

[Q22] 排序
来源：http://hz.chenlongwang.top/gtcyymypks.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.svipenyu.cn/gtoillkjex.html

[Q23] 分页
来源：http://hz.yuxming.cn/gtwrxxirsm.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.zhijiandao.cn/gtfwmjpbnp.html

[Q24] 去重
来源：http://hz.cashguo.top/gtwgobnjyb.html

SELECT DISTINCT city FROM users;
来源：http://hz.snrcjt.cn/gtebzmasty.html

[Q25] 只取前 N 条
来源：http://hz.ivvv.top/gtkokhvksh.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.sweek.top/gtvxhpbfly.html

[Q26] 计数
来源：http://hz.daxiang520.top/gtrapsbsaj.html

SELECT COUNT(*) FROM users;
来源：http://hz.cqqwz.cn/gtxecntwfy.html

[Q27] 条件计数
来源：http://hz.c1oappe.top/gttzvofckf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yuanzhike.top/gtbziugfep.html

[Q28] 求和与平均
来源：http://hz.jinghuilouyu.cn/gthbgfatyy.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.hnqzz.top/gtrvblalqk.html

[Q29] 最大最小值
来源：http://hz.hnxiangtu.top/gtbeyagrju.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.tianlin.xyz/gtjgjkfqyk.html

[Q30] 分组统计
来源：http://hz.zhongyouzk.top/gtpbtvkppv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.ydjk.org.cn/gtkxwqvjxc.html

[Q31] 分组后过滤
来源：http://hz.yonumen.top/gtemhpfhmp.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.chenjidiqi.icu/gtqwdobebk.html

[Q32] 分组拼接字符串
来源：http://hz.hysaishi.cn/gtxhousdxo.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.redwolf501.top/gtxdxqbodx.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yj20258888.top/gtvfpvrorx.html

[Q33] 多列分组
来源：http://hz.tianlin.xyz/gtyqrrmonb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.jlsjyb.cn/gtbgjahmet.html

[Q34] 每组取第一条
来源：http://hz.fzhhl.top/gtnfwgxrpn.html

SELECT * FROM (
来源：http://hz.jinghuilouyu.cn/gtjywsefor.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.wangdashe.top/gtemvvarmq.html

) t WHERE rn = 1;
来源：http://hz.shuidangran.top/gtvdvoqzck.html

[Q35] 内连接
来源：http://hz.ydjk.org.cn/gtkkimzkvl.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.shanyushiyangtech.top/gtkstmvttw.html

[Q36] 左连接
来源：http://hz.hywenlv.cn/gtyvdhyltn.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.cdnleiting.top/gtteoycijx.html

[Q37] 右连接
来源：http://hz.sufxvd.cn/gtohimxtek.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.haohaochexian.top/gtswtqejhx.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.yueranfly.top/gtumzicszh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.vqdsnc.cn/gtldogheoh.html

[Q39] 自连接（查上下级）
来源：http://hz.jinyuanbaomall.cn/gtcodxfgsr.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.bjfxy.top/gtatpolxnq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.guannengcc.top/gtgzhssyeu.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.chenjidiqi.icu/gtzmkvizpr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.52xcode.cn/gtsqmuunvo.html

[Q41] 多表连接
来源：http://hz.shangyingyoupin.top/gtvxnydurz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.sxryk.cn/gtlqjxrfhr.html

JOIN users u ON u.id = o.user_id
来源：http://hz.yvedp.cn/gtegosovdx.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.316326.xyz/gtbmmolvhz.html

[Q42] 连接条件附加过滤
来源：http://hz.ppjwa.cn/gtnwkcdlmd.html

SELECT u.name, o.amount FROM users u
来源：http://hz.ydzc1.top/gttqhsshbf.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.nanxinkj.top/gtevgorqov.html

[Q43] 标量子查询
来源：http://hz.ppjwa.cn/gtebjcnwfu.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.pengpengdd.cyou/gtwuqfevpy.html

[Q44] IN 子查询
来源：http://hz.9152youxi.cn/gtsvqiygvd.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.sweek.top/gthqtfwjay.html

[Q45] EXISTS 判断存在
来源：http://hz.wangshuangyany.cn/gtokhsytrg.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.mhx1999.top/gtazimiwix.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.fengsongda.top/gtknlgizxo.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.pengpengdd.cyou/gtysvcfjdh.html

[Q47] 与平均值比较
来源：http://hz.pengpengdd.cyou/gtlzulodtm.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.hnqzz.top/gtazdehkmq.html

[Q48] CTE 公用表表达式
来源：http://hz.zdqjudy.top/gtrgghhqki.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.yanxiufei.cn/gtcvrzkire.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.xziqi.cn/gtspaeikaz.html

[Q49] 更新单行
来源：http://hz.ehwqpu.com/gtefeoysyv.html


<!-- 参考信息 -->