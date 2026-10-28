代发 wailian999

Py:   itertools.permutations(arr)
来源：http://hz.zhijiandao.cn/gtafaurumo.html

PHP:  // 手写递归交换
来源：http://hz.quarkkingdee.top/gtdjfczach.html

JS:   // 手写回溯递归
来源：http://hz.tian-w.cn/gtfkarvodj.html

TS:   // 手写回溯递归
来源：http://hz.yuanzhike.top/gtqhispmmf.html

Java: // 手写回溯递归
来源：http://hz.gzhubu.top/gthenxebpd.html

Go:   // 手写回溯递归
来源：http://hz.gaohongyu789.top/gteaaujrim.html

Ruby: arr.permutation.to_a
来源：http://hz.meibo888.top/gttrigvqof.html

C#:   // 手写回溯递归
来源：http://hz.svipenyu.cn/gtdgmlokgi.html

[N09] 栈与队列
来源：http://hz.zycfv.cn/gthdgogmyl.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.quarkkingdee.top/gtrkkrosow.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.wangdashe.top/gtiqtkrhij.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.ydzc1.top/gtaiullyxf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.c1oappe.top/gtctgwwbcl.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.pycfn.com/gtnuxfaess.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.zhijiandao.cn/gttitgogrl.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.jinyuanbaomall.cn/gtaclfzavi.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yonumen.top/gtrmdwuxlz.html

[N10] 链表节点定义
来源：http://hz.xziqi.cn/gtanvhavki.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.9152youxi.cn/gtdoddfnjy.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.sufxvd.cn/gtmllccuul.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.cashguo.top/gtjyymstiy.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.tian-w.cn/gtmiubfcoh.html

Java: class Node { int v; Node next; }
来源：http://hz.kuanghao11.cn/gtrdjceopv.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.cqqwz.cn/gtegzabkmw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.nanxuanxn.top/gtpodolcmu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.daxiang520.top/gtgsuwfgzb.html

[N11] 二叉树中序遍历
来源：http://hz.guannengcc.top/gtwfojoiuh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.hongshengwenyu.top/gttwxbizcj.html

PHP:  // 手写递归函数
来源：http://hz.haohaochexian.top/gtkfxhvnsq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yuxming.cn/gtmmbddzah.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.chenlongwang.top/gtwmmcknvm.html

Java: // 手写递归
来源：http://hz.zhixingplan.top/gtknemhsps.html

Go:   // 手写递归
来源：http://hz.feifeiyinyue.top/gtlgiwfgkh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.smart0.xyz/gtcrxibdvs.html

C#:   // 手写递归
来源：http://hz.ydzc1.top/gtxswfhqcs.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.shuidangran.top/gtfoncycgk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.iojbl.cn/gtdszskqqc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.xylfe.cn/gtcsigqfoy.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.guowangkeji.top/gtwemvrokc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.sufxvd.cn/gttlyecqrx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.gaohongyu789.top/gthjfokxwa.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.aizwys.cn/gtgranrmxw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.wangdashe.top/gtcocvmvgp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yj20258888.top/gtcgkxqfeq.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtxrmdztbm.html

O. 并发与异步
来源：http://hz.yuanzhike.top/gtqpkadfxs.html

================================================================================
来源：http://hz.zhoulong.xyz/gtslwdseec.html

[O01] 启动一个线程
来源：http://hz.bjfxy.top/gtlbwoyplk.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.snrcjt.cn/gtjdiiosbn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.feifeiyinyue.top/gtkirtsghe.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.ehwqpu.com/gthcotunwb.html

TS:   // 同 JS
来源：http://hz.bjfxy.top/gteciqohxf.html

Java: new Thread(() -> f()).start()
来源：http://hz.yuxming.cn/gtftpvlhss.html

Go:   go f()
来源：http://hz.pengpengdd.cyou/gtqyupwmkg.html

Ruby: Thread.new { f }
来源：http://hz.yuxming.cn/gtkpsbjhhr.html

C#:   Task.Run(() => F());
来源：http://hz.shzxlz.cn/gtlhbsvxkn.html

[O02] 使用线程池
来源：http://hz.yj20258.top/gtuowhakhr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.andypj.xyz/gtaghzwxsz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.chenlongwang.top/gtjpebvowu.html

JS:   // worker_threads 线程池
来源：http://hz.mhx1999.top/gthbopatil.html

TS:   // worker_threads 线程池
来源：http://hz.9152youxi.cn/gtdlumokpe.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.svipenyu.cn/gtdkqwaspl.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.cdnleiting.top/gtophcuhyk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.hongshengwenyu.top/gtbljqtjpa.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.kuanghao11.cn/gtgujkwfeo.html

[O03] 加锁保护共享数据
来源：http://hz.nanxinkj.top/gtfsbfkoqh.html

Py:   with lock: shared += 1
来源：http://hz.ydzc1.top/gthaulqufs.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.bjfxy.top/gtoscwpsfw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.zycfv.cn/gtyvheromn.html

TS:   // 同 JS
来源：http://hz.daria6918.cn/gtzdoilvwk.html

Java: synchronized (this) { shared++; }
来源：http://hz.fengsongda.top/gtluumoxqy.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.shanyushiyangkeji.top/gtjlkudvxs.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.xingfuxueyuan.xyz/gtqbiqqnpx.html

C#:   lock (gate) { shared++; }
来源：http://hz.zhixingplan.top/gtnuemomhb.html

[O04] 定义异步函数并等待
来源：http://hz.birdmap.top/gtcklnugsv.html

Py:   async def f():⏎    await g()
来源：http://hz.haohaochexian.top/gtwmdrgxpl.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.svipenyu.cn/gtsxkvhejn.html

JS:   async function f() { await g(); }
来源：http://hz.ydzc1.top/gtjgiflepj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.ydzc1.top/gthpdazojn.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.chenlongwang.top/gtklainpff.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.shanyushiyangkeji.top/gtxmqmgtdf.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.pengpengdd.cyou/gtuobeoqqq.html

C#:   async Task F() { await G(); }
来源：http://hz.hywenlv.cn/gtsmzdrhkl.html

[O05] 并发执行并等待全部完成
来源：http://hz.guannengcc.top/gtceuwnlml.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jqgfzy.top/gtuwiifwiz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.yueranfly.top/gtadksfgxn.html

JS:   await Promise.all(tasks)
来源：http://hz.yj20258888.top/gtontdhehd.html

TS:   await Promise.all(tasks)
来源：http://hz.52xcode.cn/gtcmfcujfy.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.gogol.net.cn/gtgncmtnyb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.gogol.net.cn/gtxwcwfvrt.html

Ruby: threads.map(&:join)
来源：http://hz.gaohongyu789.top/gtvcdknxjr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.jiagoushi.top/gtwpcybsbp.html

[O06] 使用进程池
来源：http://hz.wangshuangyany.cn/gtefsoyppn.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.fengsongda.top/gtmttdhqub.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.jinqigufen.top/gtytstrdhz.html

JS:   // child_process / cluster 模块
来源：http://hz.snrcjt.cn/gtfjmxlkib.html

TS:   // child_process / cluster 模块
来源：http://hz.sxryk.cn/gtutwbgwny.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.snrcjt.cn/gtnjocybwn.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.ppjwa.cn/gtgwrrpxzi.html

Ruby: // fork 块
来源：http://hz.xingfuxueyuan.xyz/gtkdzjlnox.html

C#:   Parallel.For
来源：http://hz.zhiwuduotai.top/gthlzpmzri.html

================================================================================
来源：http://hz.jinqigufen.top/gtnvskqqsk.html

P. 常用工具函数
来源：http://hz.tian-w.cn/gtqawmxayz.html

================================================================================
来源：http://hz.jyoumei.cn/gtdnapfued.html

[P01] 生成 UUID
来源：http://hz.c1oappe.top/gtmjsiiqqn.html

Py:   str(uuid.uuid4())
来源：http://hz.shuidangran.top/gtvjelibfa.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.shanyushiyangtech.top/gtuundgcuz.html

JS:   crypto.randomUUID()
来源：http://hz.svipenyu.cn/gthmgtjpei.html

TS:   crypto.randomUUID()
来源：http://hz.shanyushiyangtech.top/gtgkmgjokj.html

Java: UUID.randomUUID().toString()
来源：http://hz.cashguo.top/gtpazwuuwv.html

Go:   // 用 github.com/google/uuid
来源：http://hz.sufxvd.cn/gtgeqahkqp.html

Ruby: SecureRandom.uuid
来源：http://hz.yanxiufei.cn/gthuhnarii.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.cucudq.cn/gtippezfdp.html

[P02] MD5 / SHA256 摘要
来源：http://hz.fengsongda.top/gtzjsbphoj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.gogol.net.cn/gthwlsrsnb.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.shanyushiyangkeji.top/gtfvspetoh.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yangfankeji.com/gtqvojsjel.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.aibaodan.cn/gtrrnqpyqv.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.sufxvd.cn/gtymmlkhfg.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.zhengqikj.top/gtrjipvjfx.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.hnxiangtu.top/gtocblqtzi.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.ppjwa.cn/gtbwuttirw.html

[P03] 生成短随机字符串
来源：http://hz.aizwys.cn/gtlxmmgtph.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.hammf.cn/gtlchkykoj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.hnxiangtu.top/gtbdbrwvpy.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.gogol.net.cn/gtafkkyazo.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.dashuyun.cn/gtzhmnlbja.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.ehwqpu.com/gteybgdijx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.aibaodan.cn/gtuuyusqdx.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.gzhubu.top/gtdbwwinvs.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.ydjk.org.cn/gtexyebeod.html

[P04] 求长度
来源：http://hz.pengpengdd.cyou/gthjitxgvp.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.meibo888.top/gtwisdaijk.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.quarkkingdee.top/gteikkpbom.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.gotoacloud.top/gtotnrqhbg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhongyouzk.top/gtaqrenspc.html

Java: list.size();  map.size();  s.length()
来源：http://hz.wangshuangyany.cn/gtyiypmugf.html

Go:   len(arr);  len(m)
来源：http://hz.jinghuilouyu.cn/gtbakessle.html

Ruby: x.length;  x.size
来源：http://hz.xingfuxueyuan.xyz/gtuhmfdxhc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.zdqjudy.top/gtgkphbyxy.html

[P05] 判断两个对象内容是否相等
来源：http://hz.sweek.top/gtskocrkuk.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.tian-w.cn/gtrctdnlni.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.pengpengdd.cyou/gtpiewmhho.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.daria6918.cn/gtrjjwhypc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.9152youxi.cn/gtsoejwjts.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.xylfe.cn/gtvslzrvpb.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.0kj1m.cn/gtnwrryuvr.html

Ruby: a == b
来源：http://hz.jinyuanbaomall.cn/gtozxwmfnk.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.yueranfly.top/gtecrxjotg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.pengpengdd.cyou/gtnrdgslno.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.sufxvd.cn/gtwjbzccnw.html

PHP:  if (empty($x)) {}
来源：http://hz.yj202588.top/gtgveapirr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.yangfankeji.com/gtcgymopyq.html

TS:   if (x == null) {}
来源：http://hz.zhengqikj.top/gtnlppdejr.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.chenzaomai.com/gteftnrrqd.html

Go:   if x == nil {}
来源：http://hz.jqgfzy.top/gtwuaecqym.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.tianlin.xyz/gtroopgnfr.html

C#:   if (x is null) {}
来源：http://hz.xuetiantiany.cn/gtjizmqxhd.html

[P07] 防抖与节流
来源：http://hz.zhongyouzk.top/gtyofyeukm.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.0kj1m.cn/gtityvtret.html

PHP:  // 手写时间戳比较
来源：http://hz.tanke756.top/gtqspvoxlm.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ybcxt.top/gtdgzpqgto.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.316326.xyz/gtihqiohgn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.cucudq.cn/gtfcdupvum.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.xziqi.cn/gtayszqmom.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.quarkkingdee.top/gtkwrdpuko.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.jinqigufen.top/gtmxohvimh.html

[P08] 处理浮点精度问题
来源：http://hz.hnqzz.top/gtwlkbhhkp.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.sweek.top/gtxogwlhcj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.yj20258888.top/gtpskmnhrf.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.dashuyun.cn/gtoqlkgizm.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.tianlin.xyz/gtddwbvils.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yj202588.top/gtacwxruud.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.fzhhl.top/gtvexdwflu.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.yvedp.cn/gtoczbdwhk.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.sxryk.cn/gtqqvfpjen.html

================================================================================
来源：http://hz.fzhhl.top/gtlqcvxrmu.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.gaohongyu789.top/gtvzyzqbbl.html

================================================================================
来源：http://hz.tanke756.top/gtzvvlgrxg.html

[Q01] 创建表
来源：http://hz.yvedp.cn/gtuupnearf.html

CREATE TABLE users (
来源：http://hz.nwbrower.top/gtcmsdtorf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.aizwys.cn/gtvqmwlvba.html

name VARCHAR(50) NOT NULL,
来源：http://hz.kuanghao11.cn/gtohdcofht.html

email VARCHAR(100) UNIQUE,
来源：http://hz.xuanzx.com/gtvvcebhgn.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.meibo888.top/gtjfhnextr.html

);
来源：http://hz.316326.xyz/gtwpxbmxhb.html

[Q02] 创建带外键的表
来源：http://hz.sufxvd.cn/gtchmltbcw.html

CREATE TABLE orders (
来源：http://hz.sufxvd.cn/gtteeusiaj.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ivvv.top/gtczvrzszw.html

user_id INT NOT NULL,
来源：http://hz.yvedp.cn/gtbdfywqwc.html

amount DECIMAL(10, 2),
来源：http://hz.jinghuilouyu.cn/gtbsobkgbn.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.cdnleiting.top/gttukccxtc.html

);
来源：http://hz.hnxiangtu.top/gtgqqygwdb.html

[Q03] 增加列
来源：http://hz.ehwqpu.com/gtznxvsnig.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.cashguo.top/gtccfejzxj.html

[Q04] 修改列类型
来源：http://hz.hywenlv.cn/gtsukekuiy.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.cdnleiting.top/gtmrlgszkv.html

[Q05] 重命名列
来源：http://hz.ydzc1.top/gteknkqlzr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.cqqwz.cn/gtycoxawgq.html

[Q06] 删除列
来源：http://hz.xinyue.icu/gtklvnyzdd.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.zhixingplan.top/gtqomafeao.html

[Q07] 删除表
来源：http://hz.shanyushiyangtech.top/gthotxemyg.html

DROP TABLE IF EXISTS orders;
来源：http://hz.yonumen.top/gtvitpwhff.html

[Q08] 创建普通索引
来源：http://hz.quarkkingdee.top/gthvdydrzn.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.cashguo.top/gtvduuaixr.html

[Q09] 创建唯一索引
来源：http://hz.haohaochexian.top/gtirjzyofq.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.ybcxt.top/gtgflzginv.html

[Q10] 插入单行
来源：http://hz.yj202588.top/gtduwoltdi.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.9152youxi.cn/gtvtsoowtn.html

[Q11] 一次插入多行
来源：http://hz.zdqjudy.top/gtznochoux.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.jinghuilouyu.cn/gtuvbphjrp.html

[Q12] 插入后取自增 ID
来源：http://hz.zycfv.cn/gtgndlmgbt.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.9152youxi.cn/gtmwcrfrjh.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.sufxvd.cn/gtyrkgzmea.html

[Q13] 忽略重复插入
来源：http://hz.xuetiantiany.cn/gtgguhtidg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.zhaomingkeji.xyz/gthqreofzq.html

[Q14] 存在则更新（upsert）
来源：http://hz.jinqigufen.top/gtoicfwvgo.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.sysykeji.top/gtlojnzlib.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.zhaomingkeji.xyz/gtmwfttzwq.html

[Q15] 查询全部
来源：http://hz.fengsongda.top/gtcoxqlwlv.html

SELECT * FROM users;
来源：http://hz.quarkkingdee.top/gttzosxghq.html

[Q16] 查询指定列
来源：http://hz.zhijiandao.cn/gtdkqmlixz.html

SELECT id, name FROM users;
来源：http://hz.cucudq.cn/gtilnlquec.html

[Q17] 条件查询
来源：http://hz.nanxinkj.top/gtbdecwyvy.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.iojbl.cn/gtyfhptmzm.html

[Q18] 模糊匹配
来源：http://hz.sweek.top/gttjrngnsi.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.tanke756.top/gtlkhizqwz.html

[Q19] 范围查询
来源：http://hz.tanke756.top/gttoovwxrl.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.hysaishi.cn/gtmjiwksvy.html

[Q20] IN 列表
来源：http://hz.redwolf501.top/gtjqyptfvg.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yanxiufei.cn/gtwrmzchrm.html

[Q21] 空值判断
来源：http://hz.yongpay.top/gtmdupybfn.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.sweek.top/gtyrflulus.html

[Q22] 排序
来源：http://hz.havefunace.top/gtjzkkdqer.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.pengpengdd.cyou/gtjgylgsip.html

[Q23] 分页
来源：http://hz.daxiang520.top/gtjhisioux.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.hammf.cn/gtfzritufw.html

[Q24] 去重
来源：http://hz.sufxvd.cn/gtzvvqqeat.html

SELECT DISTINCT city FROM users;
来源：http://hz.ydjk.org.cn/gtsdbxhkur.html

[Q25] 只取前 N 条
来源：http://hz.yanxiufei.cn/gtylsdozqa.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.havefunace.top/gtgoggbaxj.html

[Q26] 计数
来源：http://hz.zhongyouzk.top/gtyjafunhh.html

SELECT COUNT(*) FROM users;
来源：http://hz.sysykeji.top/gtmpcwpjdp.html

[Q27] 条件计数
来源：http://hz.iojbl.cn/gtgcydrnou.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.jinqigfzy.top/gtbazgqaid.html

[Q28] 求和与平均
来源：http://hz.havefunace.top/gtewtlmdqb.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.svipenyu.cn/gtwnhodejr.html

[Q29] 最大最小值
来源：http://hz.ppjwa.cn/gtlunhutoo.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.xuetiantiany.cn/gttlevmlja.html

[Q30] 分组统计
来源：http://hz.gzhubu.top/gtdemdcedz.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.xylfe.cn/gtwexsxfut.html

[Q31] 分组后过滤
来源：http://hz.vqdsnc.cn/gtbwngaktn.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.xziqi.cn/gthkiocgay.html

[Q32] 分组拼接字符串
来源：http://hz.jiagoushi.top/gtbxdaqvfm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.xziqi.cn/gtkrfoikuk.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.pycfn.com/gtldcvcers.html

[Q33] 多列分组
来源：http://hz.dashuyun.cn/gtresauawz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.pengpengdd.cyou/gtqztgastk.html

[Q34] 每组取第一条
来源：http://hz.fzhhl.top/gtkfzkpepo.html

SELECT * FROM (
来源：http://hz.cashguo.top/gtfegvnozv.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.hongshengwenyu.top/gtgjcbmxxc.html

) t WHERE rn = 1;
来源：http://hz.yangfankeji.com/gtblflmxjq.html

[Q35] 内连接
来源：http://hz.xuetiantiany.cn/gtqcwcdten.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.nwbrower.top/gtwbuesfhv.html

[Q36] 左连接
来源：http://hz.hywenlv.cn/gtpcnwvvcl.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.c1oappe.top/gtbckgxphz.html

[Q37] 右连接
来源：http://hz.daria6918.cn/gteyoqxsuq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.redwolf501.top/gttiisqgfc.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.zycfv.cn/gtqslobiwb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.ybcxt.top/gtilamwqzb.html

[Q39] 自连接（查上下级）
来源：http://hz.cashguo.top/gtffwmrqso.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.pengpengdd.cyou/gtkxlckkcr.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.hnxiangtu.top/gtzbmrjzvi.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.shanyushiyangtech.top/gtgzgvvunv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.sxryk.cn/gtxkrwqrva.html

[Q41] 多表连接
来源：http://hz.hongshengwenyu.top/gtgxjdvigj.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.birdmap.top/gtxvbqooil.html

JOIN users u ON u.id = o.user_id
来源：http://hz.zhongyouzk.top/gtlrqnsodp.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.zhiwuduotai.top/gtnzhiniur.html

[Q42] 连接条件附加过滤
来源：http://hz.sysykeji.top/gtyykpmayf.html

SELECT u.name, o.amount FROM users u
来源：http://hz.aibaodan.cn/gtqxjgtjrt.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.jyoumei.cn/gtzlxeicya.html

[Q43] 标量子查询
来源：http://hz.xylfe.cn/gtdprikuaw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.quarkkingdee.top/gtrldntxxc.html

[Q44] IN 子查询
来源：http://hz.svipenyu.cn/gtpfjnjzya.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.ydzc1.top/gthvnfualg.html

[Q45] EXISTS 判断存在
来源：http://hz.pycfn.com/gtxdwnlhnr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.cdnleiting.top/gtluyrgfgf.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.ybcxt.top/gtlzixxhih.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.iojbl.cn/gtfroksenk.html

[Q47] 与平均值比较
来源：http://hz.yuxming.cn/gtmwhnsphd.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.aizwys.cn/gtalewvwsj.html

[Q48] CTE 公用表表达式
来源：http://hz.jinqigfzy.top/gtohopkbrk.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.zhijiandao.cn/gtjswivbgb.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.tianlin.xyz/gtzneuosqm.html

[Q49] 更新单行
来源：http://hz.zdqjudy.top/gtatqpaqhj.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.andypj.xyz/gtknqaagci.html

[Q50] 批量更新
来源：http://hz.gzhubu.top/gtyzpyokyo.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.wangdashe.top/gtrkfhoxcp.html

[Q51] 用子查询更新
来源：http://hz.gzhubu.top/gthigdrbnf.html


<!-- 参考信息 -->