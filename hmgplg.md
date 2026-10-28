代发 wailian999

[N09] 栈与队列
来源：http://hz.gotoacloud.top/gthjlikawv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.ydjk.org.cn/gtrwqqlcsk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.ybcxt.top/gtqliuzybc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.sufxvd.cn/gtaokmllyz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.pycfn.com/gtiyivqlvu.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.hysaishi.cn/gtmctufasm.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.cqqwz.cn/gtxiykossi.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.hongshengwenyu.top/gtadxytbeo.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.kuanghao11.cn/gthkvyjboa.html

[N10] 链表节点定义
来源：http://hz.shuidangran.top/gtffkipwui.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.bjfxy.top/gtluprwzfw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jiagoushi.top/gtuxxxgjsg.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.ybcxt.top/gtzzxdakfb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.cashguo.top/gtyscxyniv.html

Java: class Node { int v; Node next; }
来源：http://hz.gotoacloud.top/gtqcbrqqzl.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.fengsongda.top/gthykldujf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.tian-w.cn/gtegplmwcf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.meibo888.top/gtmtriaaft.html

[N11] 二叉树中序遍历
来源：http://hz.snrcjt.cn/gtmgqcbblq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.feifeiyinyue.top/gtoedqbdms.html

PHP:  // 手写递归函数
来源：http://hz.0kj1m.cn/gtcppnkzqx.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.shangyingyoupin.top/gtbifvnwku.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jinghuilouyu.cn/gtqsyohqfw.html

Java: // 手写递归
来源：http://hz.jinqigufen.top/gtetmzypek.html

Go:   // 手写递归
来源：http://hz.tian-w.cn/gtktrzjpou.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.0kj1m.cn/gtitasznst.html

C#:   // 手写递归
来源：http://hz.shzxlz.cn/gtklasbnwn.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.quarkkingdee.top/gtxfumlgcu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.yj20258.top/gtzhfjhivs.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.gaohongyu789.top/gtbaofvrkp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.wangshuangyany.cn/gtfacfkwwj.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yj202588.top/gtbumpokhw.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ehwqpu.com/gtxcfeskik.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.ppjwa.cn/gtnfdkmtrv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.zhaomingkeji.xyz/gtcmslfane.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.sysykeji.top/gtythwrgkv.html

================================================================================
来源：http://hz.nanxuanxn.top/gtelxgkkin.html

O. 并发与异步
来源：http://hz.shangyingyoupin.top/gtgsuhehtf.html

================================================================================
来源：http://hz.shuidangran.top/gtmpfutwha.html

[O01] 启动一个线程
来源：http://hz.cqqwz.cn/gtypkfkftf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.shzxlz.cn/gttolctxja.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yuanzhike.top/gtmtwzannr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.hammf.cn/gtftdqafzy.html

TS:   // 同 JS
来源：http://hz.vqdsnc.cn/gtullvlfjl.html

Java: new Thread(() -> f()).start()
来源：http://hz.ppjwa.cn/gtyrhwfyrl.html

Go:   go f()
来源：http://hz.xylfe.cn/gtlkeaamgb.html

Ruby: Thread.new { f }
来源：http://hz.birdmap.top/gtoobjrciq.html

C#:   Task.Run(() => F());
来源：http://hz.xuetiantiany.cn/gtfuyvgugm.html

[O02] 使用线程池
来源：http://hz.guannengcc.top/gtrcpzhgdc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.fzhhl.top/gtxybketcu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.guowangkeji.top/gtmiioftqk.html

JS:   // worker_threads 线程池
来源：http://hz.cashguo.top/gtwawcicvg.html

TS:   // worker_threads 线程池
来源：http://hz.ybcxt.top/gtzzofcslo.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.shanyushiyangkeji.top/gtxxwvjisa.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yongpay.top/gttdbpujgy.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.redwolf501.top/gtilwqzmwg.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.xinyue.icu/gtmdpwiemw.html

[O03] 加锁保护共享数据
来源：http://hz.cdnleiting.top/gtiosprfbk.html

Py:   with lock: shared += 1
来源：http://hz.hammf.cn/gtzzziyfyq.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.tian-w.cn/gtpexjauxd.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.cqqwz.cn/gtgzbztuhd.html

TS:   // 同 JS
来源：http://hz.jlsjyb.cn/gtbrouzmhf.html

Java: synchronized (this) { shared++; }
来源：http://hz.gotoacloud.top/gthefpdngd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.wangdashe.top/gtfjzvhacc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.yj20258.top/gtqbexzspy.html

C#:   lock (gate) { shared++; }
来源：http://hz.pengpengdd.cyou/gtfffbumze.html

[O04] 定义异步函数并等待
来源：http://hz.sweek.top/gtgkudugbs.html

Py:   async def f():⏎    await g()
来源：http://hz.jyoumei.cn/gtkhynrzpv.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.zycfv.cn/gtlucokfby.html

JS:   async function f() { await g(); }
来源：http://hz.zycfv.cn/gtpzmhnpwf.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.fengsongda.top/gtqiibodqa.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.shanyushiyangtech.top/gtoexlrjer.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.yongpay.top/gtnitrqbrl.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.svipenyu.cn/gtihekgkea.html

C#:   async Task F() { await G(); }
来源：http://hz.pengpengdd.cyou/gthtzapupr.html

[O05] 并发执行并等待全部完成
来源：http://hz.sweek.top/gtvgdwojkx.html

Py:   asyncio.gather(*tasks)
来源：http://hz.tanke756.top/gtjxejvfbc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.snrcjt.cn/gtbfkiihgx.html

JS:   await Promise.all(tasks)
来源：http://hz.yongpay.top/gtjfanxdam.html

TS:   await Promise.all(tasks)
来源：http://hz.yuanzhike.top/gtnhyprfji.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.vqdsnc.cn/gtzcpcfziz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.jyoumei.cn/gtcgufpsls.html

Ruby: threads.map(&:join)
来源：http://hz.hfpthk.cn/gtqqktrlhf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.zhaomingkeji.xyz/gtftxbddvm.html

[O06] 使用进程池
来源：http://hz.hywenlv.cn/gtzfwvhggl.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.shanyushiyangtech.top/gtjrphualz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.pengpengdd.cyou/gtroswjggs.html

JS:   // child_process / cluster 模块
来源：http://hz.ydjk.org.cn/gtfdzffbfw.html

TS:   // child_process / cluster 模块
来源：http://hz.gogol.net.cn/gtfphwambg.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.chenjidiqi.icu/gtiyvjnoog.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.ehwqpu.com/gtefsfkoqh.html

Ruby: // fork 块
来源：http://hz.nanxuanxn.top/gtyuqzhlfa.html

C#:   Parallel.For
来源：http://hz.dianchejie.cn/gtbprtrjpa.html

================================================================================
来源：http://hz.jinqigfzy.top/gtkejzxjvy.html

P. 常用工具函数
来源：http://hz.jqgfzy.top/gtgfkgrqgo.html

================================================================================
来源：http://hz.cdnleiting.top/gtxzqmfwoi.html

[P01] 生成 UUID
来源：http://hz.zhixingplan.top/gtddzkcuem.html

Py:   str(uuid.uuid4())
来源：http://hz.jlsjyb.cn/gtttcadllp.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jiagoushi.top/gtftwfpgyb.html

JS:   crypto.randomUUID()
来源：http://hz.yuanzhike.top/gticghbmbq.html

TS:   crypto.randomUUID()
来源：http://hz.aizwys.cn/gtrvqadpip.html

Java: UUID.randomUUID().toString()
来源：http://hz.ywan-chungtsiang.top/gttyqdjbrp.html

Go:   // 用 github.com/google/uuid
来源：http://hz.ivvv.top/gtdeylnkzj.html

Ruby: SecureRandom.uuid
来源：http://hz.yanxiufei.cn/gtrmzlnrpx.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.wangshuangyany.cn/gtrfvncqrk.html

[P02] MD5 / SHA256 摘要
来源：http://hz.jyoumei.cn/gtkphtmkzn.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.shzxlz.cn/gtlbmxkulk.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.shzxlz.cn/gtdxtcyqxk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.mhx1999.top/gtcnmtpiov.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.zhoulong.xyz/gtvkrpcool.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.yueranfly.top/gteshybrkd.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.jinghuilouyu.cn/gtmjctymzq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.hywenlv.cn/gtemiaoyzq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.zhoulong.xyz/gtbmcrljra.html

[P03] 生成短随机字符串
来源：http://hz.ehwqpu.com/gtvvfmbbed.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.cqqwz.cn/gtjguxmgpi.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.ydjk.org.cn/gtzpazexvo.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.daxiang520.top/gtyvwqipjl.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.redwolf501.top/gtldushaua.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.daxiang520.top/gtdppmbtbm.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.cdnleiting.top/gtfvilinft.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.nanxinkj.top/gtkqljtdml.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.tian-w.cn/gthiqihkus.html

[P04] 求长度
来源：http://hz.jqgfzy.top/gtyoohuyzf.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.dashuyun.cn/gtfjlphgkh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jyoumei.cn/gtccscsbqi.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.aibaodan.cn/gtjlfmyhos.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.kuanghao11.cn/gtxenzmets.html

Java: list.size();  map.size();  s.length()
来源：http://hz.cucudq.cn/gtzzibtisn.html

Go:   len(arr);  len(m)
来源：http://hz.kuanghao11.cn/gtggkupsjg.html

Ruby: x.length;  x.size
来源：http://hz.cheryme.top/gtsfyqgmtx.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.haohaochexian.top/gtjqbumekq.html

[P05] 判断两个对象内容是否相等
来源：http://hz.chenzaomai.com/gtuhvawhzf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.sweek.top/gtiuuvjqvz.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.yvedp.cn/gtpzgjuufu.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.0kj1m.cn/gtkxtpsvux.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.shzxlz.cn/gtaacjmzhf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.0kj1m.cn/gtovopdmfu.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.hywenlv.cn/gtlwhaoawr.html

Ruby: a == b
来源：http://hz.ppjwa.cn/gtvkqanpnp.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.guowangkeji.top/gtaajrbbtg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.dashuyun.cn/gtpqsnbjws.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.shanyushiyangtech.top/gtcmznuduh.html

PHP:  if (empty($x)) {}
来源：http://hz.sweek.top/gtjtvwixwy.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.guowangkeji.top/gtuhnxhkok.html

TS:   if (x == null) {}
来源：http://hz.daxiang520.top/gtprbbmsze.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.yj202588.top/gtjgzzoqgc.html

Go:   if x == nil {}
来源：http://hz.zhongyouzk.top/gtgmocxgpv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.andypj.xyz/gtxdfsxpbr.html

C#:   if (x is null) {}
来源：http://hz.jyoumei.cn/gtkxpcdkyu.html

[P07] 防抖与节流
来源：http://hz.jlsjyb.cn/gtvvzxzglo.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yvedp.cn/gtenxaxwyw.html

PHP:  // 手写时间戳比较
来源：http://hz.feifeiyinyue.top/gtivdmfqwx.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hnqzz.top/gtmmrptazf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhengqikj.top/gtypwqrypi.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.shanyushiyangkeji.top/gtaxkwtuqw.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.gzhubu.top/gtetcehanm.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.wangshuangyany.cn/gtfywvxxdz.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.sweek.top/gtflczeqdd.html

[P08] 处理浮点精度问题
来源：http://hz.ybcxt.top/gtjbxcuiew.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.nwbrower.top/gtaxkysjks.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.9152youxi.cn/gtfnylwfjn.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.52xcode.cn/gtviousrlj.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.ppjwa.cn/gtvqreeaqa.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.zhiwuduotai.top/gtqwouwvrn.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.xylfe.cn/gtdfshcvpd.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.quarkkingdee.top/gtjvddanpx.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.yongpay.top/gtakaxdhoj.html

================================================================================
来源：http://hz.hnqzz.top/gtjzjgpuog.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.vqdsnc.cn/gtbwoqpzbd.html

================================================================================
来源：http://hz.meibo888.top/gthftizidr.html

[Q01] 创建表
来源：http://hz.tian-w.cn/gtphfkglre.html

CREATE TABLE users (
来源：http://hz.jinqigfzy.top/gttguyxken.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.nanxinkj.top/gtsrqmihoh.html

name VARCHAR(50) NOT NULL,
来源：http://hz.vqdsnc.cn/gttlfmptjm.html

email VARCHAR(100) UNIQUE,
来源：http://hz.fzhhl.top/gtozblisqw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.hysaishi.cn/gtxnruqtdi.html

);
来源：http://hz.0kj1m.cn/gtqjnrswdm.html

[Q02] 创建带外键的表
来源：http://hz.guowangkeji.top/gtewoecasq.html

CREATE TABLE orders (
来源：http://hz.quarkkingdee.top/gthewbdekv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.daxiang520.top/gtnqyyrebc.html

user_id INT NOT NULL,
来源：http://hz.yj20258.top/gtdsrvkdax.html

amount DECIMAL(10, 2),
来源：http://hz.zhongyouzk.top/gtiyhnsycd.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.shanyushiyangkeji.top/gtxcmeorkh.html

);
来源：http://hz.shangyingyoupin.top/gtdjpcotfv.html

[Q03] 增加列
来源：http://hz.haohaochexian.top/gtyzfczedq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.yongpay.top/gtvazzqmcn.html

[Q04] 修改列类型
来源：http://hz.xziqi.cn/gtgstjurom.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.smart0.xyz/gtjlxwpksr.html

[Q05] 重命名列
来源：http://hz.yuanzhike.top/gthpgxmhov.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.xziqi.cn/gthjqyjubk.html

[Q06] 删除列
来源：http://hz.yuanzhike.top/gtzetyonwc.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.yj202588.top/gtivuccihn.html

[Q07] 删除表
来源：http://hz.xuanzx.com/gtvtxaemcd.html

DROP TABLE IF EXISTS orders;
来源：http://hz.zdqjudy.top/gtnoldoiay.html

[Q08] 创建普通索引
来源：http://hz.yvedp.cn/gtwzsqghnk.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.0kj1m.cn/gtrdhfivlm.html

[Q09] 创建唯一索引
来源：http://hz.pycfn.com/gtklgjsstr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.xuetiantiany.cn/gtkzklobtg.html

[Q10] 插入单行
来源：http://hz.cheryme.top/gtgigzwbcz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.shanyushiyangkeji.top/gtkdeivgqa.html

[Q11] 一次插入多行
来源：http://hz.jianghu66.top/gtetzeycct.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.cucudq.cn/gtpykeerdg.html

[Q12] 插入后取自增 ID
来源：http://hz.zycfv.cn/gttrtmhxiz.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.cheryme.top/gtpqahbhjp.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.dianchejie.cn/gtctosngnt.html

[Q13] 忽略重复插入
来源：http://hz.sxryk.cn/gtvktmcsja.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.shanyushiyangkeji.top/gthqbhashs.html

[Q14] 存在则更新（upsert）
来源：http://hz.jiagoushi.top/gtizztwujv.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.yueranfly.top/gtpbvsqnxp.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.jlsjyb.cn/gtixxythgf.html

[Q15] 查询全部
来源：http://hz.vqdsnc.cn/gtfgpddbmt.html

SELECT * FROM users;
来源：http://hz.zhoulong.xyz/gtdbjkrpin.html

[Q16] 查询指定列
来源：http://hz.ydjk.org.cn/gtcgegfnve.html

SELECT id, name FROM users;
来源：http://hz.tanke756.top/gtzvpfqfap.html

[Q17] 条件查询
来源：http://hz.yanxiufei.cn/gtwysaosdc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.andypj.xyz/gtuqbnlpjx.html

[Q18] 模糊匹配
来源：http://hz.haohaochexian.top/gtjxfeycmo.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.daxiang520.top/gtzadskupf.html

[Q19] 范围查询
来源：http://hz.zhongyouzk.top/gttygmqcdt.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.sufxvd.cn/gtjlxfjlkd.html

[Q20] IN 列表
来源：http://hz.cheryme.top/gtquljeabm.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.0kj1m.cn/gtbgylyhrd.html

[Q21] 空值判断
来源：http://hz.sxryk.cn/gtzwzyvwaz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.guowangkeji.top/gtdfzlrnac.html

[Q22] 排序
来源：http://hz.chenlongwang.top/gtefpluhao.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.pycfn.com/gtinjryrer.html

[Q23] 分页
来源：http://hz.jinghuilouyu.cn/gtszohjlad.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yongpay.top/gtgrkkyswm.html

[Q24] 去重
来源：http://hz.hfpthk.cn/gtuhawdxoj.html

SELECT DISTINCT city FROM users;
来源：http://hz.xuanzx.com/gtvbhqqlrq.html

[Q25] 只取前 N 条
来源：http://hz.yj20258.top/gtgmnitltq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.svipenyu.cn/gtxtjnfzob.html

[Q26] 计数
来源：http://hz.chenzaomai.com/gtoykcnscx.html

SELECT COUNT(*) FROM users;
来源：http://hz.ywan-chungtsiang.top/gtrcxqdbrb.html

[Q27] 条件计数
来源：http://hz.gzhubu.top/gtdswiffji.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.redwolf501.top/gttmmeyaew.html

[Q28] 求和与平均
来源：http://hz.guannengcc.top/gtcteyphbd.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.zhaomingkeji.xyz/gtdjaevqif.html

[Q29] 最大最小值
来源：http://hz.jqgfzy.top/gtotzdtdpy.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.mhx1999.top/gtqvkmzmkv.html

[Q30] 分组统计
来源：http://hz.ydzc1.top/gtfdhdthtt.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.hysaishi.cn/gtwzbpsmlh.html

[Q31] 分组后过滤
来源：http://hz.cqqwz.cn/gtgceaxcdf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.kuanghao11.cn/gtcssnrysr.html

[Q32] 分组拼接字符串
来源：http://hz.fengsongda.top/gtnonxtfkj.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.bjfxy.top/gtgcnsklvx.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.daxiang520.top/gtbcllvbpz.html

[Q33] 多列分组
来源：http://hz.mhx1999.top/gtgdssucdj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.aibaodan.cn/gtumlltheu.html

[Q34] 每组取第一条
来源：http://hz.yonumen.top/gtaowjjwyj.html

SELECT * FROM (
来源：http://hz.svipenyu.cn/gtebhuojax.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.birdmap.top/gtcpxsigre.html

) t WHERE rn = 1;
来源：http://hz.ydzc1.top/gtscmujwwc.html

[Q35] 内连接
来源：http://hz.hongshengwenyu.top/gtjuigljli.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.ppjwa.cn/gtuiijhyrb.html

[Q36] 左连接
来源：http://hz.dianchejie.cn/gtescqclio.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.hongshengwenyu.top/gtyqzzapwu.html

[Q37] 右连接
来源：http://hz.daria6918.cn/gtqumgkgmo.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.andypj.xyz/gtotqyevhh.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.pengpengdd.cyou/gtglxdsfae.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.jinqigufen.top/gtovikwven.html

[Q39] 自连接（查上下级）
来源：http://hz.tianlin.xyz/gtmbxcizpm.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.hysaishi.cn/gtunyroiwu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.pycfn.com/gtzrcqkmio.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.ppjwa.cn/gtjrcqjoks.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.zhoulong.xyz/gtoemfcgyr.html

[Q41] 多表连接
来源：http://hz.yongpay.top/gtfeqjkafe.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.shuidangran.top/gtogqtetix.html

JOIN users u ON u.id = o.user_id
来源：http://hz.wangdashe.top/gtbjcapmgx.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.cucudq.cn/gtfpbpxffy.html

[Q42] 连接条件附加过滤
来源：http://hz.yvedp.cn/gtkedtodgv.html

SELECT u.name, o.amount FROM users u
来源：http://hz.zhongyouzk.top/gtofczwpkp.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.ywan-chungtsiang.top/gtiudffion.html

[Q43] 标量子查询
来源：http://hz.dashuyun.cn/gtcboiwrxi.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.sufxvd.cn/gtadbnlwis.html

[Q44] IN 子查询
来源：http://hz.dianchejie.cn/gtlclgmhki.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.iojbl.cn/gtcylfgtmg.html

[Q45] EXISTS 判断存在
来源：http://hz.shuidangran.top/gtvatasozb.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.quarkkingdee.top/gtoldivqfq.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.ppjwa.cn/gtjbfikcny.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yj202588.top/gttujopvis.html

[Q47] 与平均值比较
来源：http://hz.jinyuanbaomall.cn/gtgwdamboi.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.havefunace.top/gtvifvqsab.html

[Q48] CTE 公用表表达式
来源：http://hz.gzhubu.top/gthcjaxnsf.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.zhengqikj.top/gtbggfyuzf.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.fzhhl.top/gtcihjtusw.html

[Q49] 更新单行
来源：http://hz.9152youxi.cn/gtjpjmycgq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.aibaodan.cn/gtgyyozctl.html

[Q50] 批量更新
来源：http://hz.hnxiangtu.top/gtwoqkgrix.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.cashguo.top/gtmmjtqimn.html

[Q51] 用子查询更新
来源：http://hz.zdqjudy.top/gtwsqabuew.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.aizwys.cn/gtpwzuuhmy.html

[Q52] 删除指定行
来源：http://hz.dianchejie.cn/gtamhweiqf.html

DELETE FROM users WHERE id = 10;
来源：http://hz.cdnleiting.top/gtuaxtiudp.html

[Q53] 按条件删除
来源：http://hz.yanxiufei.cn/gtkkqgkokr.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.jiagoushi.top/gtieiqzdss.html

[Q54] 清空表
来源：http://hz.cashguo.top/gtoqjqctfj.html

TRUNCATE TABLE logs;
来源：http://hz.yongpay.top/gthilqcgqw.html

[Q55] 排名（并列占位）
来源：http://hz.shzxlz.cn/gtgoblkdqk.html


<!-- 参考信息 -->