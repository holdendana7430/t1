代发 wailian999

Go:   // 手写 map[int]int
来源：http://hz.meibo888.top/gtbqikeorj.html

Ruby: // 手写 Hash
来源：http://hz.hywenlv.cn/gtkwcpwvya.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yuxming.cn/gtxyhbzejd.html

[N08] 生成全排列
来源：http://hz.yongpay.top/gtifcyzhyi.html

Py:   itertools.permutations(arr)
来源：http://hz.bjfxy.top/gtlwcfippf.html

PHP:  // 手写递归交换
来源：http://hz.xinyue.icu/gtdterylcx.html

JS:   // 手写回溯递归
来源：http://hz.feifeiyinyue.top/gtghfvarae.html

TS:   // 手写回溯递归
来源：http://hz.zhongyouzk.top/gtcbcirowp.html

Java: // 手写回溯递归
来源：http://hz.xylfe.cn/gtvcujagae.html

Go:   // 手写回溯递归
来源：http://hz.jianghu66.top/gteiidvewp.html

Ruby: arr.permutation.to_a
来源：http://hz.quarkkingdee.top/gtxxxwzlob.html

C#:   // 手写回溯递归
来源：http://hz.xuanzx.com/gttwyssorz.html

[N09] 栈与队列
来源：http://hz.yanxiufei.cn/gtjhrjxjvp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.sysykeji.top/gtesjhnbfe.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.zhongyouzk.top/gtakypcppq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.ywan-chungtsiang.top/gttrkcicjj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yj20258888.top/gtbnczkycs.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.ydjk.org.cn/gtfsfrnhly.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.yanxiufei.cn/gtpsfqiwoc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.dashuyun.cn/gtcgjxgidy.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.kuanghao11.cn/gtyfgtgumf.html

[N10] 链表节点定义
来源：http://hz.jqgufenzy.top/gtuoqddjpv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.ydjk.org.cn/gtoxnhewcx.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.yangfankeji.com/gtzgedeags.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.mhx1999.top/gtbejejgje.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.yongpay.top/gtaophrnsc.html

Java: class Node { int v; Node next; }
来源：http://hz.yuanzhike.top/gtojvksmkk.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.zhongyouzk.top/gtipjtnztt.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.meibo888.top/gtvtvrjzqp.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.chenjidiqi.icu/gthzpofwcb.html

[N11] 二叉树中序遍历
来源：http://hz.fengsongda.top/gtjhpaezrd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.chenlongwang.top/gtlcgnljgj.html

PHP:  // 手写递归函数
来源：http://hz.0kj1m.cn/gtjgqvhfxr.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jqgfzy.top/gtnjwlirkq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yvedp.cn/gtxutbhloc.html

Java: // 手写递归
来源：http://hz.ivvv.top/gtutrsfdha.html

Go:   // 手写递归
来源：http://hz.hongshengwenyu.top/gtydazrkcb.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.jinghuilouyu.cn/gthbojyxky.html

C#:   // 手写递归
来源：http://hz.shuidangran.top/gtjnikykty.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.sysykeji.top/gtorxgqkqw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.haohaochexian.top/gttquxxzog.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.xingfuxueyuan.xyz/gtbblmzcpx.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ydzc1.top/gtjwzvjmfr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.gogol.net.cn/gtiepimmuz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ivvv.top/gtkzszcstg.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.zhengqikj.top/gtasklckne.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.yj20258888.top/gthkzanzrc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.andypj.xyz/gthxqldbef.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtvlrlxmpl.html

O. 并发与异步
来源：http://hz.nanxinkj.top/gtmwgvzgcx.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtbqjgpors.html

[O01] 启动一个线程
来源：http://hz.xuanzx.com/gtqselszrt.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.meibo888.top/gtyotsowzq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yvedp.cn/gtcwmuyddj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.yangfankeji.com/gtmleayeug.html

TS:   // 同 JS
来源：http://hz.hywenlv.cn/gtfafhlvme.html

Java: new Thread(() -> f()).start()
来源：http://hz.nwbrower.top/gtgcimrqkg.html

Go:   go f()
来源：http://hz.smart0.xyz/gtfmhxgmhg.html

Ruby: Thread.new { f }
来源：http://hz.pycfn.com/gtfsabkxkw.html

C#:   Task.Run(() => F());
来源：http://hz.ywan-chungtsiang.top/gtiscjgvtu.html

[O02] 使用线程池
来源：http://hz.zhijiandao.cn/gtapiwoojj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yvedp.cn/gtiozgnfex.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.hysaishi.cn/gtxudekjdc.html

JS:   // worker_threads 线程池
来源：http://hz.zhixingplan.top/gtatojpebz.html

TS:   // worker_threads 线程池
来源：http://hz.bjfxy.top/gtiyiigmdg.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.wangshuangyany.cn/gtsaoxzheo.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.shanyushiyangkeji.top/gtesktpnpc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.zycfv.cn/gtqwolabio.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.aizwys.cn/gthawtqafj.html

[O03] 加锁保护共享数据
来源：http://hz.dianchejie.cn/gtiludpkhs.html

Py:   with lock: shared += 1
来源：http://hz.cqqwz.cn/gtmgcwdzum.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.quarkkingdee.top/gtvhrbprtw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.sxryk.cn/gtthrkcuyt.html

TS:   // 同 JS
来源：http://hz.xuetiantiany.cn/gteyosuxok.html

Java: synchronized (this) { shared++; }
来源：http://hz.zhaomingkeji.xyz/gtenjbwvbf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.chenjidiqi.icu/gtrjiktckm.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.xuetiantiany.cn/gttmnzldqk.html

C#:   lock (gate) { shared++; }
来源：http://hz.guowangkeji.top/gtzlkhvtsg.html

[O04] 定义异步函数并等待
来源：http://hz.jinghuilouyu.cn/gtkugdxldx.html

Py:   async def f():⏎    await g()
来源：http://hz.andypj.xyz/gtpabwpvfm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.tanke756.top/gtwqigesvr.html

JS:   async function f() { await g(); }
来源：http://hz.yangfankeji.com/gtiffetgni.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.ivvv.top/gtxjvwngzw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.ywan-chungtsiang.top/gtgjxapefj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.quarkkingdee.top/gtrgahdmsm.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.fengsongda.top/gtlhrnzgid.html

C#:   async Task F() { await G(); }
来源：http://hz.cqqwz.cn/gtzpfkjxtz.html

[O05] 并发执行并等待全部完成
来源：http://hz.c1oappe.top/gtoeaqmqud.html

Py:   asyncio.gather(*tasks)
来源：http://hz.yanxiufei.cn/gtbdbhdffn.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.xziqi.cn/gtwbxidavy.html

JS:   await Promise.all(tasks)
来源：http://hz.yuanzhike.top/gtdwubxayd.html

TS:   await Promise.all(tasks)
来源：http://hz.52xcode.cn/gtdwckzjen.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.bjfxy.top/gtmbrwgmzs.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.9152youxi.cn/gtvaaoixmn.html

Ruby: threads.map(&:join)
来源：http://hz.sweek.top/gtxozrmpcr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.xinyue.icu/gtoeapuidk.html

[O06] 使用进程池
来源：http://hz.vqdsnc.cn/gtnfzspxsl.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.ydjk.org.cn/gtopjnnrqa.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.gaohongyu789.top/gtsjqkvurc.html

JS:   // child_process / cluster 模块
来源：http://hz.jinyuanbaomall.cn/gtdhduakdi.html

TS:   // child_process / cluster 模块
来源：http://hz.jqgfzy.top/gtnnxuaimi.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.ehwqpu.com/gtrjuewbwo.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.ydzc1.top/gtezitorcc.html

Ruby: // fork 块
来源：http://hz.ivvv.top/gtyyvouxwg.html

C#:   Parallel.For
来源：http://hz.yvedp.cn/gtwpeqbtbo.html

================================================================================
来源：http://hz.quarkkingdee.top/gtexxbhehx.html

P. 常用工具函数
来源：http://hz.svipenyu.cn/gtpjfadxkt.html

================================================================================
来源：http://hz.xylfe.cn/gtcbvkusld.html

[P01] 生成 UUID
来源：http://hz.sweek.top/gtixpsigct.html

Py:   str(uuid.uuid4())
来源：http://hz.shzxlz.cn/gtrzwkodny.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yuxming.cn/gtoyddisos.html

JS:   crypto.randomUUID()
来源：http://hz.shuidangran.top/gtvjtjuiom.html

TS:   crypto.randomUUID()
来源：http://hz.shangyingyoupin.top/gtygvcfxzx.html

Java: UUID.randomUUID().toString()
来源：http://hz.nanxuanxn.top/gtwrfsqldu.html

Go:   // 用 github.com/google/uuid
来源：http://hz.gogol.net.cn/gtpajepvqt.html

Ruby: SecureRandom.uuid
来源：http://hz.shanyushiyangkeji.top/gtjscpzfat.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.hnqzz.top/gthkkliijz.html

[P02] MD5 / SHA256 摘要
来源：http://hz.chenjidiqi.icu/gtblflhhxm.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.xziqi.cn/gtsenndteq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.xziqi.cn/gtmptzqsul.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.aibaodan.cn/gtaaktojrp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.yangfankeji.com/gtzkzcljlw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.fzhhl.top/gtbhyznngs.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.yueranfly.top/gtjdhgakvh.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.shanyushiyangtech.top/gtpognqwvr.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.zhaomingkeji.xyz/gtkpwwbsxs.html

[P03] 生成短随机字符串
来源：http://hz.hywenlv.cn/gtizdgwiba.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.zycfv.cn/gtdbjiyfsu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.sxryk.cn/gtfzxcxvxy.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.iojbl.cn/gthxvgoili.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xingfuxueyuan.xyz/gtizwtzyzh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jqgfzy.top/gtypaexsmr.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.gotoacloud.top/gtcsbcdgno.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.nanxinkj.top/gtypsztofw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jiagoushi.top/gtpkxpmbul.html

[P04] 求长度
来源：http://hz.gaohongyu789.top/gtkssaqcbn.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.9152youxi.cn/gtieoknjsp.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.bjfxy.top/gtfuyklbmw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.gaohongyu789.top/gtssnoazhx.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.wangdashe.top/gttxvdahyb.html

Java: list.size();  map.size();  s.length()
来源：http://hz.sxryk.cn/gtneusahge.html

Go:   len(arr);  len(m)
来源：http://hz.hnqzz.top/gtqxdcoypp.html

Ruby: x.length;  x.size
来源：http://hz.birdmap.top/gtixvsyley.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.ywan-chungtsiang.top/gtakjglyav.html

[P05] 判断两个对象内容是否相等
来源：http://hz.yueranfly.top/gtvpbgierv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.hfpthk.cn/gtebeplgkh.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.jlsjyb.cn/gtodswhbbt.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.zhiwuduotai.top/gtvndvkzgx.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jyoumei.cn/gtnzbpwltx.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.cdnleiting.top/gthauodygn.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.fengsongda.top/gtprfxcruo.html

Ruby: a == b
来源：http://hz.gotoacloud.top/gtaquhwwax.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.sweek.top/gtqscwdotp.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.smart0.xyz/gtnsrummpz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.yongpay.top/gtyjsemepv.html

PHP:  if (empty($x)) {}
来源：http://hz.ivvv.top/gtcrrdmfjn.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jinqigfzy.top/gtfwqbzlqb.html

TS:   if (x == null) {}
来源：http://hz.chenlongwang.top/gtolxqzggl.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.yj20258888.top/gtqwcxeebw.html

Go:   if x == nil {}
来源：http://hz.guannengcc.top/gttxfbjhpn.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.wangdashe.top/gtwizdzrpw.html

C#:   if (x is null) {}
来源：http://hz.xingfuxueyuan.xyz/gtxoatncvs.html

[P07] 防抖与节流
来源：http://hz.hammf.cn/gtrpusautr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jinyuanbaomall.cn/gtvjuwfjug.html

PHP:  // 手写时间戳比较
来源：http://hz.yuxming.cn/gtdbutjpoj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jinqigufen.top/gtbgvemfku.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.kuanghao11.cn/gtmcrjqmbs.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.havefunace.top/gtxvostpzj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.zhongyouzk.top/gtcpmwipxz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yj20258888.top/gttljvumfy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.snrcjt.cn/gtsrfgshky.html

[P08] 处理浮点精度问题
来源：http://hz.gzhubu.top/gtywyzbxvh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.cqqwz.cn/gtxodlqaqq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.wangshuangyany.cn/gtpcrqsiuv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.zhaomingkeji.xyz/gtvdasruwp.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.hfpthk.cn/gtydobgwyn.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.jiagoushi.top/gtnmfmczjz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.chenjidiqi.icu/gtqfpsqstq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.sweek.top/gtnlkhvpal.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.jlsjyb.cn/gtmrjkystu.html

================================================================================
来源：http://hz.wangdashe.top/gtztgdgfiz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.0kj1m.cn/gtxdmbjqcs.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtlpmnxdqc.html

[Q01] 创建表
来源：http://hz.chenzaomai.com/gtcexszqkt.html

CREATE TABLE users (
来源：http://hz.andypj.xyz/gtudqwhmzx.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jinghuilouyu.cn/gttqkynfcw.html

name VARCHAR(50) NOT NULL,
来源：http://hz.yj20258888.top/gtvwlzdhai.html

email VARCHAR(100) UNIQUE,
来源：http://hz.xylfe.cn/gtkawcvycv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.sxryk.cn/gtnirpxyfw.html

);
来源：http://hz.hywenlv.cn/gtqipjtdpa.html

[Q02] 创建带外键的表
来源：http://hz.yj20258.top/gtkozvamya.html

CREATE TABLE orders (
来源：http://hz.hnqzz.top/gtsaisrjny.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.kuanghao11.cn/gthgpyiefe.html

user_id INT NOT NULL,
来源：http://hz.quarkkingdee.top/gtwcndzomn.html

amount DECIMAL(10, 2),
来源：http://hz.chenjidiqi.icu/gtwlofozhs.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.jyoumei.cn/gtukozlbun.html

);
来源：http://hz.meibo888.top/gtlstjgqtu.html

[Q03] 增加列
来源：http://hz.dashuyun.cn/gtehjylckc.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.haohaochexian.top/gtkygtuhmq.html

[Q04] 修改列类型
来源：http://hz.sweek.top/gtqbizrerj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.zhiwuduotai.top/gtujirkggl.html

[Q05] 重命名列
来源：http://hz.havefunace.top/gtqhltoqgz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.sufxvd.cn/gtcdngiqfj.html

[Q06] 删除列
来源：http://hz.shangyingyoupin.top/gtbsabwvts.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.zhixingplan.top/gthltarwbn.html

[Q07] 删除表
来源：http://hz.zdqjudy.top/gtqbawryew.html

DROP TABLE IF EXISTS orders;
来源：http://hz.shzxlz.cn/gtlgylzcry.html

[Q08] 创建普通索引
来源：http://hz.xingfuxueyuan.xyz/gtyqllrefx.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.aibaodan.cn/gtlnblwyrq.html

[Q09] 创建唯一索引
来源：http://hz.52xcode.cn/gttddmqiuc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.yueranfly.top/gtkbdgdauy.html

[Q10] 插入单行
来源：http://hz.yj20258.top/gtiwnshbum.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.316326.xyz/gthmzbrdjf.html

[Q11] 一次插入多行
来源：http://hz.hammf.cn/gtvayksuzz.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.quarkkingdee.top/gtcfuqfvqz.html

[Q12] 插入后取自增 ID
来源：http://hz.cucudq.cn/gtjcywutgp.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.cqqwz.cn/gtihmfscih.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.jyoumei.cn/gtoypigsyq.html

[Q13] 忽略重复插入
来源：http://hz.hysaishi.cn/gtiytoimvu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jiagoushi.top/gtenusxfku.html

[Q14] 存在则更新（upsert）
来源：http://hz.9152youxi.cn/gtbkfanywn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.zhoulong.xyz/gtpucvawpp.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.aibaodan.cn/gtrhvnkted.html

[Q15] 查询全部
来源：http://hz.9152youxi.cn/gtwgslsjat.html

SELECT * FROM users;
来源：http://hz.hysaishi.cn/gtmfijipmz.html

[Q16] 查询指定列
来源：http://hz.cucudq.cn/gttplaluuf.html

SELECT id, name FROM users;
来源：http://hz.svipenyu.cn/gtohaoixyt.html

[Q17] 条件查询
来源：http://hz.jinqigfzy.top/gtvtykppgm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.jyoumei.cn/gttnhgjktb.html

[Q18] 模糊匹配
来源：http://hz.meibo888.top/gtjegbrsuv.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.c1oappe.top/gtkjdlmwid.html

[Q19] 范围查询
来源：http://hz.jiagoushi.top/gtkadrcpaz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.birdmap.top/gtqshvjley.html

[Q20] IN 列表
来源：http://hz.sysykeji.top/gtfgzqlugn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.tanke756.top/gteonjetua.html

[Q21] 空值判断
来源：http://hz.wangshuangyany.cn/gtxhtpcpns.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.sxryk.cn/gtmwtglnev.html

[Q22] 排序
来源：http://hz.nanxuanxn.top/gtolyadspd.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.tian-w.cn/gtpjtvunta.html

[Q23] 分页
来源：http://hz.9152youxi.cn/gtvfgqzkth.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.sysykeji.top/gtdqgzibdh.html

[Q24] 去重
来源：http://hz.shzxlz.cn/gtyutcrqbh.html

SELECT DISTINCT city FROM users;
来源：http://hz.gotoacloud.top/gtipatfsje.html

[Q25] 只取前 N 条
来源：http://hz.chenzaomai.com/gtsgwmwkcs.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.ydjk.org.cn/gtbjvdczfa.html

[Q26] 计数
来源：http://hz.aibaodan.cn/gtmruqbtpf.html

SELECT COUNT(*) FROM users;
来源：http://hz.feifeiyinyue.top/gtckalnruw.html

[Q27] 条件计数
来源：http://hz.daxiang520.top/gtljkakeat.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.gaohongyu789.top/gtzccbdzar.html

[Q28] 求和与平均
来源：http://hz.dianchejie.cn/gthmumleci.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.shanyushiyangkeji.top/gtldkinkul.html

[Q29] 最大最小值
来源：http://hz.jqgfzy.top/gtlpmizpcz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.hysaishi.cn/gtkkcdatsr.html

[Q30] 分组统计
来源：http://hz.cucudq.cn/gtwarspnli.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.zhiwuduotai.top/gtbabvnruu.html

[Q31] 分组后过滤
来源：http://hz.ehwqpu.com/gtrkznssxf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yj20258.top/gtxevlmyuo.html

[Q32] 分组拼接字符串
来源：http://hz.hnqzz.top/gtittcfyyh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.jiagoushi.top/gtlvyfmqvu.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.xziqi.cn/gtzehtnlxa.html

[Q33] 多列分组
来源：http://hz.vqdsnc.cn/gtopgncabq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.cqqwz.cn/gtukipqkhm.html

[Q34] 每组取第一条
来源：http://hz.zdqjudy.top/gtbfwfamca.html

SELECT * FROM (
来源：http://hz.hammf.cn/gtjtkgnevz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.fengsongda.top/gtgxwxjwjp.html

) t WHERE rn = 1;
来源：http://hz.chenlongwang.top/gtbdaxzrdp.html

[Q35] 内连接
来源：http://hz.fzhhl.top/gtlfabuomx.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.cheryme.top/gtkwbvalmy.html

[Q36] 左连接
来源：http://hz.zdqjudy.top/gtuugfjxav.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.sxryk.cn/gtmsbnkxrn.html

[Q37] 右连接
来源：http://hz.xylfe.cn/gtpqgfskcd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.bjfxy.top/gteqcsjdiy.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.ywan-chungtsiang.top/gtcsiactsk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.ppjwa.cn/gtauxcimfz.html

[Q39] 自连接（查上下级）
来源：http://hz.quarkkingdee.top/gtmasxoigz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.dashuyun.cn/gthdmzoolt.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.52xcode.cn/gtnphpvswd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.tianlin.xyz/gthsvyeioj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.sysykeji.top/gtknzldjjd.html

[Q41] 多表连接
来源：http://hz.mhx1999.top/gtiqyirlfn.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.nanxinkj.top/gtgtftvfqm.html

JOIN users u ON u.id = o.user_id
来源：http://hz.zhengqikj.top/gtpaltehtq.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.yueranfly.top/gtfaohybyn.html

[Q42] 连接条件附加过滤
来源：http://hz.shuidangran.top/gthmqvgpof.html

SELECT u.name, o.amount FROM users u
来源：http://hz.316326.xyz/gtaupirokq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yj20258.top/gthltugxqp.html

[Q43] 标量子查询
来源：http://hz.316326.xyz/gtusgxrngg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.zhiwuduotai.top/gtcmqrveag.html

[Q44] IN 子查询
来源：http://hz.vqdsnc.cn/gtqldnrsnb.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.tian-w.cn/gtwyduvqoh.html

[Q45] EXISTS 判断存在
来源：http://hz.chenlongwang.top/gtluqcljvi.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.cashguo.top/gtxbmtfejp.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.fzhhl.top/gtrbtusels.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.aibaodan.cn/gtfxcdrlrt.html

[Q47] 与平均值比较
来源：http://hz.gaohongyu789.top/gtqraaonfu.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.shangyingyoupin.top/gtowqymbkv.html

[Q48] CTE 公用表表达式
来源：http://hz.xingfuxueyuan.xyz/gtmuiuzkew.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.havefunace.top/gtgiymjukz.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.shanyushiyangkeji.top/gtgylecllk.html

[Q49] 更新单行
来源：http://hz.yuanzhike.top/gtymzazoes.html


<!-- 参考信息 -->