代发 wailian999

Go:   // 手写 map[int]int
来源：http://hz.nanxinkj.top/gthofqhwwc.html

Ruby: // 手写 Hash
来源：http://hz.guowangkeji.top/gtbewzdwnv.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.guannengcc.top/gtamabpdka.html

[N08] 生成全排列
来源：http://hz.wangdashe.top/gtblouzugs.html

Py:   itertools.permutations(arr)
来源：http://hz.jinghuilouyu.cn/gtngnciozk.html

PHP:  // 手写递归交换
来源：http://hz.gogol.net.cn/gtvgxhcxtg.html

JS:   // 手写回溯递归
来源：http://hz.dianchejie.cn/gtoltqdsua.html

TS:   // 手写回溯递归
来源：http://hz.jinqigufen.top/gtzkpfczsu.html

Java: // 手写回溯递归
来源：http://hz.zycfv.cn/gtcoipqgrg.html

Go:   // 手写回溯递归
来源：http://hz.zhoulong.xyz/gtbgvfowix.html

Ruby: arr.permutation.to_a
来源：http://hz.gzhubu.top/gtqhlouwcg.html

C#:   // 手写回溯递归
来源：http://hz.gzhubu.top/gtfdhokggd.html

[N09] 栈与队列
来源：http://hz.sxryk.cn/gtgyaeiczx.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.hywenlv.cn/gtqwwzoheo.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.jinghuilouyu.cn/gtfbvpvukp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.vqdsnc.cn/gtoektleha.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jinyuanbaomall.cn/gtlaqnozvn.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.shanyushiyangtech.top/gtxkyipknb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.redwolf501.top/gtkdhekzdf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yueranfly.top/gtrqnenzrb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.shuidangran.top/gtglzkuwop.html

[N10] 链表节点定义
来源：http://hz.shanyushiyangkeji.top/gtjpwjwrxo.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.mhx1999.top/gtklikjnkd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.bjfxy.top/gttuqcbarh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zhijiandao.cn/gtamrkpmou.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.yvedp.cn/gtskawrhfi.html

Java: class Node { int v; Node next; }
来源：http://hz.jinghuilouyu.cn/gthstbbtsw.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.jinqigufen.top/gthrjjrxpz.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.zhoulong.xyz/gtzkauzyjz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.gotoacloud.top/gtozkzhpia.html

[N11] 二叉树中序遍历
来源：http://hz.hongshengwenyu.top/gtjqvbkumi.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.cqqwz.cn/gtojfftbkm.html

PHP:  // 手写递归函数
来源：http://hz.yj20258888.top/gtyvnozxvc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.xziqi.cn/gtqslunbms.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ehwqpu.com/gtjquepwfs.html

Java: // 手写递归
来源：http://hz.gogol.net.cn/gtkacuxcep.html

Go:   // 手写递归
来源：http://hz.gaohongyu789.top/gtrbmlqptr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.nwbrower.top/gtugtwwkzn.html

C#:   // 手写递归
来源：http://hz.gzhubu.top/gtvvrhqalu.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.svipenyu.cn/gtjmruebtx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.tian-w.cn/gtxtqubaax.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.pycfn.com/gtwxpkfksy.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jqgfzy.top/gtjrciccjh.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.pengpengdd.cyou/gtdnfhfbev.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.sxryk.cn/gttpvbpqli.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.snrcjt.cn/gtcjejwhpw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.xuetiantiany.cn/gtgxlxzfkr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.daria6918.cn/gtbrvfkfbf.html

================================================================================
来源：http://hz.jiagoushi.top/gtdebtdxkj.html

O. 并发与异步
来源：http://hz.hnxiangtu.top/gtcmjaxjpe.html

================================================================================
来源：http://hz.yueranfly.top/gtfrkykhuo.html

[O01] 启动一个线程
来源：http://hz.svipenyu.cn/gtawtntrpw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.jqgufenzy.top/gtcrqyyiud.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yangfankeji.com/gtocsgxznc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.fzhhl.top/gtoedfauvc.html

TS:   // 同 JS
来源：http://hz.aibaodan.cn/gtdnprutnl.html

Java: new Thread(() -> f()).start()
来源：http://hz.yuxming.cn/gtlihyyrdu.html

Go:   go f()
来源：http://hz.yj20258.top/gthsuboxpd.html

Ruby: Thread.new { f }
来源：http://hz.jiagoushi.top/gtblwaqwgg.html

C#:   Task.Run(() => F());
来源：http://hz.zhoulong.xyz/gtfastuzbu.html

[O02] 使用线程池
来源：http://hz.aibaodan.cn/gtjiotsdiv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.vqdsnc.cn/gtikfxbnec.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.yuxming.cn/gtqrnvltyt.html

JS:   // worker_threads 线程池
来源：http://hz.jianghu66.top/gtfdmkrqlm.html

TS:   // worker_threads 线程池
来源：http://hz.c1oappe.top/gthhgodkwb.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yvedp.cn/gtddazptfm.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.ydzc1.top/gtaeslrddf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.hnxiangtu.top/gtjxsopsmo.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.guowangkeji.top/gthklltpuk.html

[O03] 加锁保护共享数据
来源：http://hz.ybcxt.top/gtbuairgpq.html

Py:   with lock: shared += 1
来源：http://hz.yuanzhike.top/gtyetsbxsl.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zdqjudy.top/gtqntnkvja.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.jqgfzy.top/gttfasfshz.html

TS:   // 同 JS
来源：http://hz.sufxvd.cn/gttzccvomu.html

Java: synchronized (this) { shared++; }
来源：http://hz.jianghu66.top/gtpgazunbf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.cucudq.cn/gtbxfvtzkx.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.yonumen.top/gttmmjcrgc.html

C#:   lock (gate) { shared++; }
来源：http://hz.sweek.top/gtccaezcvx.html

[O04] 定义异步函数并等待
来源：http://hz.zhiwuduotai.top/gtsqpgxftt.html

Py:   async def f():⏎    await g()
来源：http://hz.shanyushiyangtech.top/gtprtbftvr.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.fzhhl.top/gtmcuogzct.html

JS:   async function f() { await g(); }
来源：http://hz.zhengqikj.top/gtjdhllupb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.birdmap.top/gtuorpiszu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.andypj.xyz/gtphgicekf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.yonumen.top/gtlidgohvw.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.chenlongwang.top/gtxmzuywtt.html

C#:   async Task F() { await G(); }
来源：http://hz.jiagoushi.top/gtxtakjjbf.html

[O05] 并发执行并等待全部完成
来源：http://hz.pycfn.com/gtqntvixji.html

Py:   asyncio.gather(*tasks)
来源：http://hz.hongshengwenyu.top/gtrtklepiw.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.zycfv.cn/gtdocxqypl.html

JS:   await Promise.all(tasks)
来源：http://hz.316326.xyz/gtmtvrvpdn.html

TS:   await Promise.all(tasks)
来源：http://hz.yonumen.top/gtbujvatuu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.jianghu66.top/gtnifksknu.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.cdnleiting.top/gtmjgdfpkp.html

Ruby: threads.map(&:join)
来源：http://hz.hfpthk.cn/gtfkksqzxz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yonumen.top/gtfaopgjmx.html

[O06] 使用进程池
来源：http://hz.ydzc1.top/gtwimqnprm.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.gotoacloud.top/gtilocvsqm.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.zdqjudy.top/gtsikfmzvi.html

JS:   // child_process / cluster 模块
来源：http://hz.andypj.xyz/gtzohizeep.html

TS:   // child_process / cluster 模块
来源：http://hz.jyoumei.cn/gttpurlkxw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.dianchejie.cn/gttqxnprfg.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.wangdashe.top/gtlokcggbq.html

Ruby: // fork 块
来源：http://hz.hywenlv.cn/gttduejwva.html

C#:   Parallel.For
来源：http://hz.xinyue.icu/gtfutwczxf.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtnadamstw.html

P. 常用工具函数
来源：http://hz.sufxvd.cn/gtzymrwtdn.html

================================================================================
来源：http://hz.birdmap.top/gtltbmbmsz.html

[P01] 生成 UUID
来源：http://hz.9152youxi.cn/gtkhmctwlu.html

Py:   str(uuid.uuid4())
来源：http://hz.tanke756.top/gtyhgfdzyk.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.sxryk.cn/gtfpdqcwfn.html

JS:   crypto.randomUUID()
来源：http://hz.hywenlv.cn/gtliqpevyo.html

TS:   crypto.randomUUID()
来源：http://hz.zhiwuduotai.top/gtylmqyygh.html

Java: UUID.randomUUID().toString()
来源：http://hz.gaohongyu789.top/gtavmgksdn.html

Go:   // 用 github.com/google/uuid
来源：http://hz.zhiwuduotai.top/gtuenkklrn.html

Ruby: SecureRandom.uuid
来源：http://hz.ehwqpu.com/gtwtngbffy.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.hammf.cn/gtxpsrzdje.html

[P02] MD5 / SHA256 摘要
来源：http://hz.dianchejie.cn/gtjkumtmiv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.daxiang520.top/gthcxkvpve.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.jlsjyb.cn/gtyprhyfqw.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.redwolf501.top/gttuciauwj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.sysykeji.top/gtktvhswgd.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.0kj1m.cn/gtdijzujpp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.bjfxy.top/gtfzbxjeqd.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jinghuilouyu.cn/gtpewmbvgs.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.zhixingplan.top/gtvwmecyhx.html

[P03] 生成短随机字符串
来源：http://hz.chenzaomai.com/gtoxvxbehc.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jyoumei.cn/gtidrpzova.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.xziqi.cn/gtkhlvyctv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.iojbl.cn/gtsxclwein.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.shzxlz.cn/gtlotquwsl.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yongpay.top/gtxasdspcp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yj20258888.top/gtojakbhaj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.yj202588.top/gtlfxzdeln.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.pycfn.com/gtxbnqoavp.html

[P04] 求长度
来源：http://hz.xuanzx.com/gtyuhqxzth.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.hfpthk.cn/gthsfeizfg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.52xcode.cn/gtkwnnybaf.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.fzhhl.top/gtgwwxyvzn.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.gogol.net.cn/gtwmyjzkae.html

Java: list.size();  map.size();  s.length()
来源：http://hz.cashguo.top/gtqzhnlwgm.html

Go:   len(arr);  len(m)
来源：http://hz.zhongyouzk.top/gtweblzsmy.html

Ruby: x.length;  x.size
来源：http://hz.hfpthk.cn/gtagsiovkm.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.vqdsnc.cn/gtxawtaskl.html

[P05] 判断两个对象内容是否相等
来源：http://hz.andypj.xyz/gtzuapbvrq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.jqgufenzy.top/gtvefureme.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.ivvv.top/gtuyhvwmur.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.iojbl.cn/gtlecroslq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.hongshengwenyu.top/gtowpxobib.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.zhijiandao.cn/gthkqrqbbx.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.feifeiyinyue.top/gttmcxewwq.html

Ruby: a == b
来源：http://hz.svipenyu.cn/gtvgtlyixz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.zhijiandao.cn/gtrawglojg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.xziqi.cn/gtwpbeghve.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.tanke756.top/gtgzcumpww.html

PHP:  if (empty($x)) {}
来源：http://hz.nanxuanxn.top/gtcfwledad.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.tanke756.top/gtmcbvjwbv.html

TS:   if (x == null) {}
来源：http://hz.yonumen.top/gtebmamtgx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.iojbl.cn/gtliffejvs.html

Go:   if x == nil {}
来源：http://hz.gogol.net.cn/gtvakvlqwu.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.birdmap.top/gtkdfednxi.html

C#:   if (x is null) {}
来源：http://hz.zhaomingkeji.xyz/gtkpioniyg.html

[P07] 防抖与节流
来源：http://hz.jinqigufen.top/gttfvrnczd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yongpay.top/gtoimcwije.html

PHP:  // 手写时间戳比较
来源：http://hz.yuanzhike.top/gtghfogjru.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.fzhhl.top/gtbysytplw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.chenjidiqi.icu/gttbyhaegt.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.jianghu66.top/gtauaulrjs.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.jyoumei.cn/gtfiwdueno.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.jinghuilouyu.cn/gtgmkmxvnj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.gaohongyu789.top/gtitobjzas.html

[P08] 处理浮点精度问题
来源：http://hz.pengpengdd.cyou/gtnlxynoyj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.zdqjudy.top/gtybdezhvp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.yongpay.top/gtylqzrvan.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.ywan-chungtsiang.top/gtxyzbjhvp.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.ydzc1.top/gteoqvhorx.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.gotoacloud.top/gtrmdahqbs.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.sxryk.cn/gtnkxpdmem.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.guannengcc.top/gteizmfxjr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.zhijiandao.cn/gthbsmpctp.html

================================================================================
来源：http://hz.zycfv.cn/gtrhekibdc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.cucudq.cn/gtyqcsvjee.html

================================================================================
来源：http://hz.zhengqikj.top/gtwvycunkt.html

[Q01] 创建表
来源：http://hz.hongshengwenyu.top/gtdhdjjfgx.html

CREATE TABLE users (
来源：http://hz.zhongyouzk.top/gtfdpzrait.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.tianlin.xyz/gtqcnfvwcq.html

name VARCHAR(50) NOT NULL,
来源：http://hz.shanyushiyangkeji.top/gtexdjrfaw.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jinghuilouyu.cn/gtndanjelo.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.wangshuangyany.cn/gtaaeztgyi.html

);
来源：http://hz.hongshengwenyu.top/gtvycipjyx.html

[Q02] 创建带外键的表
来源：http://hz.cdnleiting.top/gtohummwtx.html

CREATE TABLE orders (
来源：http://hz.hywenlv.cn/gtqzhhkuor.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.52xcode.cn/gtfchfyhmp.html

user_id INT NOT NULL,
来源：http://hz.zhixingplan.top/gtgxpkwpli.html

amount DECIMAL(10, 2),
来源：http://hz.hfpthk.cn/gtjnpiubrb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.xziqi.cn/gtwjyhpkml.html

);
来源：http://hz.ivvv.top/gthammybhn.html

[Q03] 增加列
来源：http://hz.chenzaomai.com/gtgqhkcuke.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.shanyushiyangkeji.top/gtqimlhjnp.html

[Q04] 修改列类型
来源：http://hz.havefunace.top/gtocqueofi.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.zdqjudy.top/gtueyogxfd.html

[Q05] 重命名列
来源：http://hz.ppjwa.cn/gtfkpwrstc.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.cdnleiting.top/gtirsjfhqo.html

[Q06] 删除列
来源：http://hz.xylfe.cn/gtfcpwoakg.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.chenjidiqi.icu/gtcfgsomkk.html

[Q07] 删除表
来源：http://hz.cdnleiting.top/gtyuhybcrp.html

DROP TABLE IF EXISTS orders;
来源：http://hz.jyoumei.cn/gtlgpgyfai.html

[Q08] 创建普通索引
来源：http://hz.shzxlz.cn/gtcjopzdzx.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.cheryme.top/gtpuygimvb.html

[Q09] 创建唯一索引
来源：http://hz.feifeiyinyue.top/gtfjbwbfuw.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.quarkkingdee.top/gtbrnfroiy.html

[Q10] 插入单行
来源：http://hz.snrcjt.cn/gtnesdcxju.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.hammf.cn/gttbpcnign.html

[Q11] 一次插入多行
来源：http://hz.ydzc1.top/gtbvdvnbzd.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.ybcxt.top/gtfhkduyxc.html

[Q12] 插入后取自增 ID
来源：http://hz.birdmap.top/gtxdpqbnsp.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.hammf.cn/gtecdonsuy.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.shanyushiyangkeji.top/gtgszpmlvl.html

[Q13] 忽略重复插入
来源：http://hz.zhixingplan.top/gtizicorhw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.mhx1999.top/gtnjulwznb.html

[Q14] 存在则更新（upsert）
来源：http://hz.nwbrower.top/gtbonprhir.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.52xcode.cn/gttlytyqjw.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.yj202588.top/gtgnqwgfwg.html

[Q15] 查询全部
来源：http://hz.shanyushiyangkeji.top/gtmhdehfgj.html

SELECT * FROM users;
来源：http://hz.shanyushiyangtech.top/gtronzwbwz.html

[Q16] 查询指定列
来源：http://hz.0kj1m.cn/gtkkburyjy.html

SELECT id, name FROM users;
来源：http://hz.jinqigufen.top/gtsrheapee.html

[Q17] 条件查询
来源：http://hz.yvedp.cn/gtfnwbifgs.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.daria6918.cn/gtuuiewutj.html

[Q18] 模糊匹配
来源：http://hz.zhongyouzk.top/gthtsdiaey.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.nanxinkj.top/gtrtacycdf.html

[Q19] 范围查询
来源：http://hz.andypj.xyz/gtlxlxaljk.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.tanke756.top/gtqwujghxo.html

[Q20] IN 列表
来源：http://hz.meibo888.top/gtrfibijwz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.guowangkeji.top/gtmainbzgr.html

[Q21] 空值判断
来源：http://hz.svipenyu.cn/gtxpllqzrv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.chenlongwang.top/gtqiwvzqui.html

[Q22] 排序
来源：http://hz.zhongyouzk.top/gtjwvgnmbh.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.gogol.net.cn/gtzmflveha.html

[Q23] 分页
来源：http://hz.gogol.net.cn/gtmmoxovhi.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.c1oappe.top/gtcvyyenie.html

[Q24] 去重
来源：http://hz.jinghuilouyu.cn/gtbjzexyxe.html

SELECT DISTINCT city FROM users;
来源：http://hz.jiagoushi.top/gtafyqueap.html

[Q25] 只取前 N 条
来源：http://hz.0kj1m.cn/gtfkckotmv.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.kuanghao11.cn/gteexcuwlw.html

[Q26] 计数
来源：http://hz.quarkkingdee.top/gtptwwpjnv.html

SELECT COUNT(*) FROM users;
来源：http://hz.yvedp.cn/gtmudipkfs.html

[Q27] 条件计数
来源：http://hz.gzhubu.top/gtgnipltze.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yanxiufei.cn/gtphhvhwuf.html

[Q28] 求和与平均
来源：http://hz.chenjidiqi.icu/gtdubmkgig.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.vqdsnc.cn/gtptnrpjvr.html

[Q29] 最大最小值
来源：http://hz.hywenlv.cn/gtttrfxgfp.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.yj202588.top/gtzdxdxurt.html

[Q30] 分组统计
来源：http://hz.shzxlz.cn/gtooqsedfc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.pycfn.com/gtqtzkhszs.html

[Q31] 分组后过滤
来源：http://hz.ywan-chungtsiang.top/gtdndcnnxn.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.quarkkingdee.top/gtbaasqeqe.html

[Q32] 分组拼接字符串
来源：http://hz.yj202588.top/gtiexazucu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.xylfe.cn/gtbpfkysgv.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.meibo888.top/gtcwxbbzwm.html

[Q33] 多列分组
来源：http://hz.xinyue.icu/gtusvrtqdu.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yuxming.cn/gtzwkvmnqr.html

[Q34] 每组取第一条
来源：http://hz.zycfv.cn/gtonhafvhn.html

SELECT * FROM (
来源：http://hz.shzxlz.cn/gtdrxgesra.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.nanxuanxn.top/gtnusaoewm.html

) t WHERE rn = 1;
来源：http://hz.jyoumei.cn/gtemfnugqq.html

[Q35] 内连接
来源：http://hz.zhengqikj.top/gtqvsnwhkv.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.chenzaomai.com/gtxbarkghm.html

[Q36] 左连接
来源：http://hz.aibaodan.cn/gtouiubjij.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.gotoacloud.top/gtqkiektcg.html

[Q37] 右连接
来源：http://hz.ivvv.top/gtfgiooevr.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jqgfzy.top/gtdtkbgbuq.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.hammf.cn/gthiedfqcr.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.pengpengdd.cyou/gtrmsmuovd.html

[Q39] 自连接（查上下级）
来源：http://hz.yj20258888.top/gtiqozbhwc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.xingfuxueyuan.xyz/gteuxsmhzc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.zhongyouzk.top/gtvihldfcb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.zhijiandao.cn/gthbktwwkb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.zhiwuduotai.top/gtbmlatsuy.html

[Q41] 多表连接
来源：http://hz.gotoacloud.top/gtftyfmruh.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.jinghuilouyu.cn/gtpgrxusml.html

JOIN users u ON u.id = o.user_id
来源：http://hz.dianchejie.cn/gtxpurfbqf.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.guowangkeji.top/gthtqjecnx.html

[Q42] 连接条件附加过滤
来源：http://hz.jiagoushi.top/gtwhrdyjpb.html

SELECT u.name, o.amount FROM users u
来源：http://hz.mhx1999.top/gtacmubgev.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.jinghuilouyu.cn/gtuywvzbjl.html

[Q43] 标量子查询
来源：http://hz.wangdashe.top/gtivybnhfc.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.jinqigfzy.top/gtscfrqwse.html

[Q44] IN 子查询
来源：http://hz.svipenyu.cn/gtwmdwbrbe.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.guannengcc.top/gtbhsoquvh.html

[Q45] EXISTS 判断存在
来源：http://hz.c1oappe.top/gtgrllmdmp.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.9152youxi.cn/gtxujbfcpl.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.zdqjudy.top/gtizsqiicr.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.iojbl.cn/gtxiwvrofu.html

[Q47] 与平均值比较
来源：http://hz.yj20258888.top/gteeenwxur.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.nanxuanxn.top/gtvhunbzhs.html

[Q48] CTE 公用表表达式
来源：http://hz.zycfv.cn/gtppxqjxqp.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jinghuilouyu.cn/gtmkmbdszp.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.svipenyu.cn/gtgpmcoxat.html

[Q49] 更新单行
来源：http://hz.zhengqikj.top/gtkazhwcos.html


<!-- 参考信息 -->