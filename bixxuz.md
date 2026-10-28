代发 wailian999

Py:   itertools.permutations(arr)
来源：http://hz.ehwqpu.com/gtpftzfhma.html

PHP:  // 手写递归交换
来源：http://hz.ybcxt.top/gtmpoqlzqi.html

JS:   // 手写回溯递归
来源：http://hz.jqgufenzy.top/gtdslvyuus.html

TS:   // 手写回溯递归
来源：http://hz.pycfn.com/gtnngpqadt.html

Java: // 手写回溯递归
来源：http://hz.feifeiyinyue.top/gtdwwvdatm.html

Go:   // 手写回溯递归
来源：http://hz.chenlongwang.top/gtqoflceve.html

Ruby: arr.permutation.to_a
来源：http://hz.sysykeji.top/gtdilprhyl.html

C#:   // 手写回溯递归
来源：http://hz.yueranfly.top/gtwhldexyg.html

[N09] 栈与队列
来源：http://hz.svipenyu.cn/gtqclejgzh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.dashuyun.cn/gtfzoupbfv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.zdqjudy.top/gtnuuptruj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yj20258.top/gtmaxjunwb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.quarkkingdee.top/gtepbakzce.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.zhaomingkeji.xyz/gtirzjmfer.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.shanyushiyangtech.top/gthapwbitl.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.tanke756.top/gtihwadyao.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.shangyingyoupin.top/gtzpxoeekv.html

[N10] 链表节点定义
来源：http://hz.c1oappe.top/gtuzwyfxyu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.nanxuanxn.top/gtegdeaecu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.yj20258.top/gtcbceakgi.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.meibo888.top/gtphrghsil.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.xingfuxueyuan.xyz/gtfbqsgtmb.html

Java: class Node { int v; Node next; }
来源：http://hz.ehwqpu.com/gtikkdokvg.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.zdqjudy.top/gtbtvtidxa.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.cucudq.cn/gtwrebggrj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.nanxuanxn.top/gtosathxuv.html

[N11] 二叉树中序遍历
来源：http://hz.xylfe.cn/gtxhbevltn.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.jqgfzy.top/gtyivltdbo.html

PHP:  // 手写递归函数
来源：http://hz.havefunace.top/gtyzwbmgds.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.smart0.xyz/gtgpzgrslb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jinyuanbaomall.cn/gtsoabmrpx.html

Java: // 手写递归
来源：http://hz.zhaomingkeji.xyz/gtytcywzot.html

Go:   // 手写递归
来源：http://hz.cucudq.cn/gtsqjrlwvf.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.ivvv.top/gtvbyidhey.html

C#:   // 手写递归
来源：http://hz.shanyushiyangtech.top/gtydgtbctn.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.0kj1m.cn/gtspvseuuq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.svipenyu.cn/gtjpaaprmh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.yueranfly.top/gtovchimlr.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.smart0.xyz/gtqaiwvqki.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yongpay.top/gtsfccsutj.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xuetiantiany.cn/gtmiktbqpd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.pycfn.com/gtnfwanfye.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.yuanzhike.top/gtidyaapop.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xylfe.cn/gtbwzpwspn.html

================================================================================
来源：http://hz.zhoulong.xyz/gtjykauysi.html

O. 并发与异步
来源：http://hz.0kj1m.cn/gtzhqwmrnn.html

================================================================================
来源：http://hz.bjfxy.top/gtqnwzrvuc.html

[O01] 启动一个线程
来源：http://hz.yonumen.top/gtutaudlfc.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.hnqzz.top/gtckxlrhcj.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yueranfly.top/gtgdzoogbi.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.hongshengwenyu.top/gtgjggrsjb.html

TS:   // 同 JS
来源：http://hz.jlsjyb.cn/gtfhokinqn.html

Java: new Thread(() -> f()).start()
来源：http://hz.ywan-chungtsiang.top/gtkvtlrcoy.html

Go:   go f()
来源：http://hz.gogol.net.cn/gthfakpyvs.html

Ruby: Thread.new { f }
来源：http://hz.cdnleiting.top/gtnethhqoq.html

C#:   Task.Run(() => F());
来源：http://hz.xziqi.cn/gtgaqvjlwu.html

[O02] 使用线程池
来源：http://hz.xziqi.cn/gtyulhsqtb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.shangyingyoupin.top/gtgffxmvtb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.shangyingyoupin.top/gtdyxftnqq.html

JS:   // worker_threads 线程池
来源：http://hz.hnqzz.top/gtzsiuaorn.html

TS:   // worker_threads 线程池
来源：http://hz.nanxinkj.top/gttqlzmmeb.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yj20258.top/gtdauweqfw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.zhongyouzk.top/gtyotcqetq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.ehwqpu.com/gtmfhpetih.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.yongpay.top/gtcqavbioz.html

[O03] 加锁保护共享数据
来源：http://hz.jinqigufen.top/gtuuuhiyxy.html

Py:   with lock: shared += 1
来源：http://hz.9152youxi.cn/gtesqcnqfu.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.shanyushiyangtech.top/gtsxrmibfm.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.316326.xyz/gtrybcrnet.html

TS:   // 同 JS
来源：http://hz.yuxming.cn/gtyvkgnvem.html

Java: synchronized (this) { shared++; }
来源：http://hz.jyoumei.cn/gtazcbxaaq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.hfpthk.cn/gtoobzxvtv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.aibaodan.cn/gtnvcaoeqa.html

C#:   lock (gate) { shared++; }
来源：http://hz.guannengcc.top/gtdmxxnksz.html

[O04] 定义异步函数并等待
来源：http://hz.yuxming.cn/gttdrermfp.html

Py:   async def f():⏎    await g()
来源：http://hz.wangdashe.top/gtwgzekdtg.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jqgufenzy.top/gtjwajyniq.html

JS:   async function f() { await g(); }
来源：http://hz.shangyingyoupin.top/gtnvutbkep.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.316326.xyz/gtoieazvwo.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.hammf.cn/gtgcbekwcb.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.cucudq.cn/gtoheivjwf.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yangfankeji.com/gtnrwlkhix.html

C#:   async Task F() { await G(); }
来源：http://hz.hnxiangtu.top/gtkjragxoa.html

[O05] 并发执行并等待全部完成
来源：http://hz.redwolf501.top/gtrpvyncir.html

Py:   asyncio.gather(*tasks)
来源：http://hz.zhijiandao.cn/gtgocffkbn.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.wangshuangyany.cn/gtvevdvmsx.html

JS:   await Promise.all(tasks)
来源：http://hz.jqgufenzy.top/gtarukjnbj.html

TS:   await Promise.all(tasks)
来源：http://hz.ybcxt.top/gtujhkvvex.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.zhongyouzk.top/gtbrnbwcja.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.kuanghao11.cn/gtzjeowbzu.html

Ruby: threads.map(&:join)
来源：http://hz.hfpthk.cn/gttqaoqppn.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.gogol.net.cn/gtkqkmxwot.html

[O06] 使用进程池
来源：http://hz.tian-w.cn/gthxwvcjyk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.pengpengdd.cyou/gttbsksnum.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.jlsjyb.cn/gtmtqcwgan.html

JS:   // child_process / cluster 模块
来源：http://hz.ivvv.top/gtafjeearv.html

TS:   // child_process / cluster 模块
来源：http://hz.andypj.xyz/gtcpnzdzvy.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.snrcjt.cn/gtgjpwgtyz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.smart0.xyz/gtzqrncubg.html

Ruby: // fork 块
来源：http://hz.vqdsnc.cn/gtacatmzca.html

C#:   Parallel.For
来源：http://hz.yangfankeji.com/gtvoavxuds.html

================================================================================
来源：http://hz.52xcode.cn/gtdyypfsyz.html

P. 常用工具函数
来源：http://hz.yanxiufei.cn/gtiiljsldh.html

================================================================================
来源：http://hz.zycfv.cn/gtnbblcscz.html

[P01] 生成 UUID
来源：http://hz.havefunace.top/gttwlkmupn.html

Py:   str(uuid.uuid4())
来源：http://hz.hnqzz.top/gtmajepile.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.iojbl.cn/gtqdgjmliv.html

JS:   crypto.randomUUID()
来源：http://hz.xylfe.cn/gtjbunntgk.html

TS:   crypto.randomUUID()
来源：http://hz.meibo888.top/gtyzsslglc.html

Java: UUID.randomUUID().toString()
来源：http://hz.daria6918.cn/gtjfnhxmdn.html

Go:   // 用 github.com/google/uuid
来源：http://hz.zhijiandao.cn/gtafkwzufe.html

Ruby: SecureRandom.uuid
来源：http://hz.shuidangran.top/gtdfibeqoc.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.c1oappe.top/gtbccoopvd.html

[P02] MD5 / SHA256 摘要
来源：http://hz.tanke756.top/gtypnvhmrz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.chenjidiqi.icu/gtiajjraxb.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.jinqigufen.top/gtnwgxtlya.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.hnxiangtu.top/gtvqonamkm.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.52xcode.cn/gtmiskunjv.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.daxiang520.top/gtxdnfujys.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.dashuyun.cn/gtckuhfpab.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.daxiang520.top/gtdlvsijhx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.jlsjyb.cn/gtkydauqtf.html

[P03] 生成短随机字符串
来源：http://hz.zhijiandao.cn/gtrvtlzcng.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.shanyushiyangtech.top/gtapublcdp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.iojbl.cn/gtcagcplac.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.shuidangran.top/gtasakrbvr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.kuanghao11.cn/gtvhpgicnv.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.cdnleiting.top/gtdqoebkrt.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.nanxinkj.top/gtmqlndtjm.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.gaohongyu789.top/gtdrokcswk.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.0kj1m.cn/gtnmhbinyh.html

[P04] 求长度
来源：http://hz.pengpengdd.cyou/gttlcxyuhb.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.jiagoushi.top/gtutfovqpj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.wangdashe.top/gtcszrwmxo.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xuanzx.com/gtvlntxsng.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hnxiangtu.top/gtggggshuw.html

Java: list.size();  map.size();  s.length()
来源：http://hz.yongpay.top/gtdugmqnyg.html

Go:   len(arr);  len(m)
来源：http://hz.xuetiantiany.cn/gtvaxvjamp.html

Ruby: x.length;  x.size
来源：http://hz.quarkkingdee.top/gttqwtiuob.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.mhx1999.top/gtiodufdpz.html

[P05] 判断两个对象内容是否相等
来源：http://hz.hongshengwenyu.top/gtvjdenohf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.chenjidiqi.icu/gtexkptfnq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.chenzaomai.com/gtcivkmmvf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.sufxvd.cn/gttwsbifpa.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.9152youxi.cn/gtetogkqpa.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.hongshengwenyu.top/gtvpalfhyu.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.cashguo.top/gtcfniybek.html

Ruby: a == b
来源：http://hz.zhijiandao.cn/gtvqirzxhs.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.cdnleiting.top/gtfgfiifuo.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.svipenyu.cn/gtjcaqeijh.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.sufxvd.cn/gtkvzurgsm.html

PHP:  if (empty($x)) {}
来源：http://hz.jyoumei.cn/gtpkerxzqv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.hfpthk.cn/gtlqraqrgj.html

TS:   if (x == null) {}
来源：http://hz.hywenlv.cn/gtabhirpec.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.shuidangran.top/gtjfctxjrw.html

Go:   if x == nil {}
来源：http://hz.pycfn.com/gtoqwunvkx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.cdnleiting.top/gtwsrohczj.html

C#:   if (x is null) {}
来源：http://hz.havefunace.top/gtlnslrygs.html

[P07] 防抖与节流
来源：http://hz.pycfn.com/gtraflhhrj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yueranfly.top/gtakrytkge.html

PHP:  // 手写时间戳比较
来源：http://hz.gotoacloud.top/gtuttcvako.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.nwbrower.top/gtgbdnpuoo.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.svipenyu.cn/gtgzuyaoql.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.hnqzz.top/gtecgtrerm.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.daxiang520.top/gtxrvoyrmn.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.cheryme.top/gtntclomrz.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.ppjwa.cn/gtxplmnick.html

[P08] 处理浮点精度问题
来源：http://hz.ywan-chungtsiang.top/gtroksziqg.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.cucudq.cn/gtapdhrzyg.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.sweek.top/gtiuxckbch.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.ydjk.org.cn/gtgzvlmduz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.jlsjyb.cn/gtenhlbuxk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.cashguo.top/gtcesjivdj.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.iojbl.cn/gtdbkfgiff.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.jlsjyb.cn/gtrwsjjxdw.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.52xcode.cn/gtwyxllwdi.html

================================================================================
来源：http://hz.bjfxy.top/gtfyztufde.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.gaohongyu789.top/gtxpeyfsyv.html

================================================================================
来源：http://hz.zycfv.cn/gtmlvscbjm.html

[Q01] 创建表
来源：http://hz.pengpengdd.cyou/gtifxzrwsb.html

CREATE TABLE users (
来源：http://hz.snrcjt.cn/gtjdmhoyct.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hnxiangtu.top/gtingycejw.html

name VARCHAR(50) NOT NULL,
来源：http://hz.jinqigfzy.top/gtzootrhzl.html

email VARCHAR(100) UNIQUE,
来源：http://hz.yongpay.top/gtybhgxrsb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.bjfxy.top/gttfwuamub.html

);
来源：http://hz.meibo888.top/gtkiexfclt.html

[Q02] 创建带外键的表
来源：http://hz.yuxming.cn/gtodtpfinn.html

CREATE TABLE orders (
来源：http://hz.zhiwuduotai.top/gtmdopqpcg.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.316326.xyz/gtybpbihxd.html

user_id INT NOT NULL,
来源：http://hz.ybcxt.top/gtkdgewpro.html

amount DECIMAL(10, 2),
来源：http://hz.0kj1m.cn/gtkpktgbtb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.yuanzhike.top/gtasalvjgo.html

);
来源：http://hz.pycfn.com/gtuxembjjh.html

[Q03] 增加列
来源：http://hz.ydzc1.top/gtisnywglq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.yj20258.top/gtpbnzetrm.html

[Q04] 修改列类型
来源：http://hz.zycfv.cn/gtqdcxphrr.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.xziqi.cn/gtutcfbboc.html

[Q05] 重命名列
来源：http://hz.shzxlz.cn/gtizehejdn.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.jinghuilouyu.cn/gtvqinrhca.html

[Q06] 删除列
来源：http://hz.hnxiangtu.top/gttmktpuij.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.tianlin.xyz/gttocjzvef.html

[Q07] 删除表
来源：http://hz.hfpthk.cn/gtyewojxls.html

DROP TABLE IF EXISTS orders;
来源：http://hz.xinyue.icu/gtqwqxfprt.html

[Q08] 创建普通索引
来源：http://hz.yuanzhike.top/gtpmaavgke.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.yueranfly.top/gtjlgappxt.html

[Q09] 创建唯一索引
来源：http://hz.shanyushiyangkeji.top/gthbiiigpy.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.mhx1999.top/gtiyyncatc.html

[Q10] 插入单行
来源：http://hz.316326.xyz/gtsrocdqgh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.zdqjudy.top/gtomxwkqge.html

[Q11] 一次插入多行
来源：http://hz.xuanzx.com/gtbbelqonj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.xuetiantiany.cn/gtpbtvhypm.html

[Q12] 插入后取自增 ID
来源：http://hz.shanyushiyangkeji.top/gtsfxignme.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.ybcxt.top/gtpmwnxfwu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.jinqigfzy.top/gtsdbmgewy.html

[Q13] 忽略重复插入
来源：http://hz.nwbrower.top/gtymfrfuxa.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.shzxlz.cn/gtxpojzjap.html

[Q14] 存在则更新（upsert）
来源：http://hz.yvedp.cn/gtooyxflni.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.nanxinkj.top/gtrpezoxdq.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.jinqigfzy.top/gtrcxgujjo.html

[Q15] 查询全部
来源：http://hz.nwbrower.top/gtuoyllxbu.html

SELECT * FROM users;
来源：http://hz.xziqi.cn/gtkxvvqlyn.html

[Q16] 查询指定列
来源：http://hz.shzxlz.cn/gtqtrjcqls.html

SELECT id, name FROM users;
来源：http://hz.andypj.xyz/gtngqokfmb.html

[Q17] 条件查询
来源：http://hz.pycfn.com/gtbnopqyrd.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.pycfn.com/gtdmpqiaer.html

[Q18] 模糊匹配
来源：http://hz.cashguo.top/gtwpvaaefk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yangfankeji.com/gttgsaxddv.html

[Q19] 范围查询
来源：http://hz.yongpay.top/gtmedskclj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.nanxuanxn.top/gtncxiswot.html

[Q20] IN 列表
来源：http://hz.wangshuangyany.cn/gtizlbtebm.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.redwolf501.top/gtvunfezqt.html

[Q21] 空值判断
来源：http://hz.guannengcc.top/gtejmprjjd.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.xylfe.cn/gtmmuzuubv.html

[Q22] 排序
来源：http://hz.guowangkeji.top/gtvbiqhwta.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.shuidangran.top/gtyhjegowl.html

[Q23] 分页
来源：http://hz.jinqigufen.top/gtfifzyozq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.tian-w.cn/gtrtpfecuk.html

[Q24] 去重
来源：http://hz.gogol.net.cn/gtseytmodm.html

SELECT DISTINCT city FROM users;
来源：http://hz.sxryk.cn/gtyvdmuaat.html

[Q25] 只取前 N 条
来源：http://hz.jiagoushi.top/gtpbsregui.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.jqgfzy.top/gtmaffkjve.html

[Q26] 计数
来源：http://hz.nanxinkj.top/gtdvswdqfo.html

SELECT COUNT(*) FROM users;
来源：http://hz.0kj1m.cn/gttpctibzi.html

[Q27] 条件计数
来源：http://hz.ydjk.org.cn/gtdladtrnk.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.andypj.xyz/gtgrheseuu.html

[Q28] 求和与平均
来源：http://hz.zhaomingkeji.xyz/gtjpppykdr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.xuetiantiany.cn/gtutcvoieo.html

[Q29] 最大最小值
来源：http://hz.yongpay.top/gtsmvvrbox.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.gzhubu.top/gthvflqtxn.html

[Q30] 分组统计
来源：http://hz.yongpay.top/gtwaxaayfs.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.zhixingplan.top/gtsahzgjlk.html

[Q31] 分组后过滤
来源：http://hz.xziqi.cn/gtgfgltzio.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.shangyingyoupin.top/gtannzesrk.html

[Q32] 分组拼接字符串
来源：http://hz.quarkkingdee.top/gtpkvctwpx.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.ppjwa.cn/gtkziomyjb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yanxiufei.cn/gtruujditp.html

[Q33] 多列分组
来源：http://hz.jyoumei.cn/gtrkywigvn.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.jiagoushi.top/gtrujyqdob.html

[Q34] 每组取第一条
来源：http://hz.xingfuxueyuan.xyz/gtjnoletpq.html

SELECT * FROM (
来源：http://hz.fzhhl.top/gtqkxxendi.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.nanxuanxn.top/gtzwevradn.html

) t WHERE rn = 1;
来源：http://hz.hysaishi.cn/gtxzscwqgy.html

[Q35] 内连接
来源：http://hz.zhixingplan.top/gtffydwhzc.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.316326.xyz/gttwhwkocj.html

[Q36] 左连接
来源：http://hz.yueranfly.top/gtwfnkvzty.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.fzhhl.top/gthqligcmv.html

[Q37] 右连接
来源：http://hz.daxiang520.top/gtzspcajnu.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.ivvv.top/gtoiobwmzo.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.zhengqikj.top/gtqzikiocj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.iojbl.cn/gtpczcommq.html

[Q39] 自连接（查上下级）
来源：http://hz.yangfankeji.com/gtzdnpinbu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.wangshuangyany.cn/gtyioxhlrv.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.xziqi.cn/gtayxtdnjx.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.yanxiufei.cn/gtotbljfzm.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.sxryk.cn/gtuildtctf.html

[Q41] 多表连接
来源：http://hz.guowangkeji.top/gtikiepgze.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.xinyue.icu/gtxpoucfzv.html

JOIN users u ON u.id = o.user_id
来源：http://hz.quarkkingdee.top/gtzepddbys.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.wangdashe.top/gtydhsoexw.html

[Q42] 连接条件附加过滤
来源：http://hz.jlsjyb.cn/gtpjnayvdy.html

SELECT u.name, o.amount FROM users u
来源：http://hz.wangdashe.top/gttnbecnfh.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.sweek.top/gtludeqwzh.html

[Q43] 标量子查询
来源：http://hz.gzhubu.top/gtmrnuzlph.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yangfankeji.com/gtizvpwloe.html

[Q44] IN 子查询
来源：http://hz.316326.xyz/gtxqywzqnb.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.xuanzx.com/gtrjomevjy.html

[Q45] EXISTS 判断存在
来源：http://hz.iojbl.cn/gtlwupdstl.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.smart0.xyz/gtjiifnjiz.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.nanxinkj.top/gtqyimsrou.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yj20258.top/gtskkrsrmx.html

[Q47] 与平均值比较
来源：http://hz.aizwys.cn/gtumoegmvq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.daria6918.cn/gtvhjkipjm.html

[Q48] CTE 公用表表达式
来源：http://hz.zhaomingkeji.xyz/gtwtnbnvey.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.zdqjudy.top/gtdogrxgjk.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.zycfv.cn/gtkjzodprw.html

[Q49] 更新单行
来源：http://hz.shangyingyoupin.top/gtkxtmwxgn.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.xuetiantiany.cn/gtmoeudolg.html

[Q50] 批量更新
来源：http://hz.9152youxi.cn/gtmgoyphsl.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.nanxuanxn.top/gtiocwyacx.html

[Q51] 用子查询更新
来源：http://hz.zycfv.cn/gtxwlmpbiv.html


<!-- 参考信息 -->