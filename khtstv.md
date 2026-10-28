代发 wailian999

Py:   itertools.permutations(arr)
来源：http://hz.ywan-chungtsiang.top/gtwixdbzaz.html

PHP:  // 手写递归交换
来源：http://hz.cashguo.top/gtszsqopcl.html

JS:   // 手写回溯递归
来源：http://hz.yuxming.cn/gtancxtpyp.html

TS:   // 手写回溯递归
来源：http://hz.xylfe.cn/gtorzcruws.html

Java: // 手写回溯递归
来源：http://hz.tianlin.xyz/gtpkktynly.html

Go:   // 手写回溯递归
来源：http://hz.xylfe.cn/gtskqumuzx.html

Ruby: arr.permutation.to_a
来源：http://hz.nanxinkj.top/gtppcuqqsk.html

C#:   // 手写回溯递归
来源：http://hz.havefunace.top/gthglayxvd.html

[N09] 栈与队列
来源：http://hz.yj20258.top/gtpcqevhvi.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.zhaomingkeji.xyz/gtunitjklm.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.ydjk.org.cn/gtwduiadni.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.fengsongda.top/gtulvfdiiz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.pycfn.com/gtvhauuqcd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.zycfv.cn/gtpkjyqedb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.daxiang520.top/gtrnsompkk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.wangdashe.top/gtuokgkxvn.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.meibo888.top/gtzcyocdex.html

[N10] 链表节点定义
来源：http://hz.zhaomingkeji.xyz/gtoellkzdv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yj20258.top/gttxxjgtdb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.iojbl.cn/gtbvundska.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.ydjk.org.cn/gtatspgbhb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.shangyingyoupin.top/gtsjblqkjw.html

Java: class Node { int v; Node next; }
来源：http://hz.smart0.xyz/gthudyzdla.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.gzhubu.top/gtzqbzzdpd.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.hfpthk.cn/gtcvqhmbjj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.meibo888.top/gtgswiiefg.html

[N11] 二叉树中序遍历
来源：http://hz.zhongyouzk.top/gthcvbabbf.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.9152youxi.cn/gtxljvdxfv.html

PHP:  // 手写递归函数
来源：http://hz.shangyingyoupin.top/gtwxjqlxdb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.xylfe.cn/gtrebuanax.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.vqdsnc.cn/gtayiwyrty.html

Java: // 手写递归
来源：http://hz.zhixingplan.top/gtmclnoeqx.html

Go:   // 手写递归
来源：http://hz.yj202588.top/gtyrvgkfza.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.yj20258.top/gtctvrlcxe.html

C#:   // 手写递归
来源：http://hz.daxiang520.top/gtdgtssqdc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.nanxinkj.top/gtobezhjuh.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.xingfuxueyuan.xyz/gtfhjlgssp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jinqigufen.top/gtclnsudoc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.gaohongyu789.top/gtisasdeec.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.tanke756.top/gtzakgegmh.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.nwbrower.top/gtvrfsqgpg.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.zycfv.cn/gtcalnvqnf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.jqgfzy.top/gtycdxckeh.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.shzxlz.cn/gttenpnzic.html

================================================================================
来源：http://hz.birdmap.top/gtxceukcnm.html

O. 并发与异步
来源：http://hz.nanxinkj.top/gtalmifsne.html

================================================================================
来源：http://hz.nwbrower.top/gtorfrbmyj.html

[O01] 启动一个线程
来源：http://hz.svipenyu.cn/gtcikitvwd.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.nanxinkj.top/gtenqdvikk.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.gzhubu.top/gthbuvkzks.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.xuanzx.com/gtdnjujjee.html

TS:   // 同 JS
来源：http://hz.0kj1m.cn/gtlmnppoak.html

Java: new Thread(() -> f()).start()
来源：http://hz.wangdashe.top/gtmdmkeiug.html

Go:   go f()
来源：http://hz.iojbl.cn/gtepgqwhuk.html

Ruby: Thread.new { f }
来源：http://hz.hnxiangtu.top/gtqtytybcc.html

C#:   Task.Run(() => F());
来源：http://hz.kuanghao11.cn/gtpqkqmkea.html

[O02] 使用线程池
来源：http://hz.hongshengwenyu.top/gtdtjzfjnw.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.jinyuanbaomall.cn/gtcvergmja.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.yonumen.top/gtnysjandb.html

JS:   // worker_threads 线程池
来源：http://hz.52xcode.cn/gtpbzhihmr.html

TS:   // worker_threads 线程池
来源：http://hz.ehwqpu.com/gtgrtgxgoq.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.wangshuangyany.cn/gtjunuamiq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.wangdashe.top/gtufmwmrov.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.jqgufenzy.top/gtgnappgbq.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.jiagoushi.top/gtwnsmrkjy.html

[O03] 加锁保护共享数据
来源：http://hz.tanke756.top/gtzweqjsmf.html

Py:   with lock: shared += 1
来源：http://hz.tian-w.cn/gtznacdhbc.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.birdmap.top/gtazidfasv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.chenzaomai.com/gtsdcfephz.html

TS:   // 同 JS
来源：http://hz.jyoumei.cn/gtjyhteuqp.html

Java: synchronized (this) { shared++; }
来源：http://hz.zhengqikj.top/gtmjbssluz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yuxming.cn/gtsasgxpxy.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.hywenlv.cn/gtqyzusnrr.html

C#:   lock (gate) { shared++; }
来源：http://hz.gotoacloud.top/gtvirnilfb.html

[O04] 定义异步函数并等待
来源：http://hz.zhijiandao.cn/gtprowptjv.html

Py:   async def f():⏎    await g()
来源：http://hz.sxryk.cn/gtsqpdtano.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.chenzaomai.com/gtcvvszhde.html

JS:   async function f() { await g(); }
来源：http://hz.wangshuangyany.cn/gtvmnussne.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.snrcjt.cn/gtxoymjazr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.hnxiangtu.top/gtuayaefpc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.sysykeji.top/gtaxwsstsj.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.chenjidiqi.icu/gtfavbfjbg.html

C#:   async Task F() { await G(); }
来源：http://hz.xziqi.cn/gttcovqlla.html

[O05] 并发执行并等待全部完成
来源：http://hz.andypj.xyz/gtvdmwdafp.html

Py:   asyncio.gather(*tasks)
来源：http://hz.xziqi.cn/gtojiprwbc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.pengpengdd.cyou/gtivyzcpyb.html

JS:   await Promise.all(tasks)
来源：http://hz.iojbl.cn/gtdpgpeuue.html

TS:   await Promise.all(tasks)
来源：http://hz.gogol.net.cn/gtwqbmqtcj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.zhijiandao.cn/gtnsiiaxvb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.cheryme.top/gttvpqfqri.html

Ruby: threads.map(&:join)
来源：http://hz.xinyue.icu/gtmusmtwvn.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.tian-w.cn/gtpioashge.html

[O06] 使用进程池
来源：http://hz.ehwqpu.com/gtvagbwcfa.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.ybcxt.top/gticxezgln.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.cdnleiting.top/gtenvaoxoc.html

JS:   // child_process / cluster 模块
来源：http://hz.svipenyu.cn/gtelfyefon.html

TS:   // child_process / cluster 模块
来源：http://hz.ywan-chungtsiang.top/gtxhpakzrl.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.pengpengdd.cyou/gtdbxqjxen.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.ydzc1.top/gtkjihnpst.html

Ruby: // fork 块
来源：http://hz.sufxvd.cn/gtpxivhsmg.html

C#:   Parallel.For
来源：http://hz.nanxuanxn.top/gtkhlqziue.html

================================================================================
来源：http://hz.zhijiandao.cn/gtjvyhrrxf.html

P. 常用工具函数
来源：http://hz.vqdsnc.cn/gthlbrxslz.html

================================================================================
来源：http://hz.gaohongyu789.top/gtuovrgsrq.html

[P01] 生成 UUID
来源：http://hz.meibo888.top/gtquqvuyvq.html

Py:   str(uuid.uuid4())
来源：http://hz.jqgufenzy.top/gtrfgsbujc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.zhixingplan.top/gtuwgvcdem.html

JS:   crypto.randomUUID()
来源：http://hz.sysykeji.top/gtwvugaxko.html

TS:   crypto.randomUUID()
来源：http://hz.cqqwz.cn/gtyfeuaist.html

Java: UUID.randomUUID().toString()
来源：http://hz.pengpengdd.cyou/gtyzvtoakk.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yvedp.cn/gtirfjrkxd.html

Ruby: SecureRandom.uuid
来源：http://hz.svipenyu.cn/gtpdptpddq.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.dashuyun.cn/gthsjfpdhw.html

[P02] MD5 / SHA256 摘要
来源：http://hz.kuanghao11.cn/gtpkmacesn.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.hywenlv.cn/gtwgtswcll.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.quarkkingdee.top/gtrcfoqqfo.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.ehwqpu.com/gtrqbftgol.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.shuidangran.top/gtntokisju.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.zhiwuduotai.top/gtrcnovejf.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.yangfankeji.com/gtfirfgmbx.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.tianlin.xyz/gtmtowqxfz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yuxming.cn/gtbongciec.html

[P03] 生成短随机字符串
来源：http://hz.daxiang520.top/gtjlvsymer.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.xuetiantiany.cn/gtivldfulj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.nwbrower.top/gtxrcjxxvg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.guowangkeji.top/gtfxxambzr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hnxiangtu.top/gthbcdoqks.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.nanxinkj.top/gthknprrhm.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.ybcxt.top/gtbheukmka.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.yvedp.cn/gtfxnbddyy.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.zhoulong.xyz/gtynrufpru.html

[P04] 求长度
来源：http://hz.zycfv.cn/gtpuyplbib.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.yj20258.top/gtubsjtcwk.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.gogol.net.cn/gtvjvjaxed.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.gzhubu.top/gttpumxejh.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xuanzx.com/gtjiogrojb.html

Java: list.size();  map.size();  s.length()
来源：http://hz.gotoacloud.top/gtbkupviub.html

Go:   len(arr);  len(m)
来源：http://hz.cucudq.cn/gtjbpmbsrr.html

Ruby: x.length;  x.size
来源：http://hz.aizwys.cn/gtzmxqamlv.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.bjfxy.top/gtzethndhn.html

[P05] 判断两个对象内容是否相等
来源：http://hz.pycfn.com/gtmnfmunsi.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.redwolf501.top/gtwedurcwa.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.nanxuanxn.top/gtkgcedrkh.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.guannengcc.top/gtukgckmeq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zhongyouzk.top/gtfgpnvzev.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.chenzaomai.com/gthvipdizf.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yuanzhike.top/gtlfabbjnx.html

Ruby: a == b
来源：http://hz.shanyushiyangtech.top/gtebpatboc.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.iojbl.cn/gtayodjjmm.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.hywenlv.cn/gtxnxziulx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.sufxvd.cn/gtlvwyenlm.html

PHP:  if (empty($x)) {}
来源：http://hz.fengsongda.top/gtimowhpos.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.shzxlz.cn/gtzvurczhd.html

TS:   if (x == null) {}
来源：http://hz.fengsongda.top/gtifptoxbh.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.316326.xyz/gtqagkrbfo.html

Go:   if x == nil {}
来源：http://hz.jyoumei.cn/gtgotbsrap.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.nanxuanxn.top/gttgyqygkx.html

C#:   if (x is null) {}
来源：http://hz.cheryme.top/gtpsqvqyfv.html

[P07] 防抖与节流
来源：http://hz.bjfxy.top/gtlxnatyjp.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.hammf.cn/gtubtxnxns.html

PHP:  // 手写时间戳比较
来源：http://hz.chenjidiqi.icu/gtqbmmneqn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yongpay.top/gtqnlewdrr.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhijiandao.cn/gttoohxcei.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.zhoulong.xyz/gtysrpqhiv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.chenzaomai.com/gtormklcid.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.wangshuangyany.cn/gtetxmpkel.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.9152youxi.cn/gtblvafusy.html

[P08] 处理浮点精度问题
来源：http://hz.cdnleiting.top/gtzhaearbw.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.yj202588.top/gtgbtqffej.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.xuanzx.com/gtqmtenbfw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.tanke756.top/gtpdhntnmr.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.jinqigufen.top/gtoexbtkxz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.cheryme.top/gtclxrqczy.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.aibaodan.cn/gtqitkslbf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.tianlin.xyz/gtsblzhlgx.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.daxiang520.top/gtvslxytwy.html

================================================================================
来源：http://hz.birdmap.top/gtrqnmyioq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.daria6918.cn/gteiohsomi.html

================================================================================
来源：http://hz.tian-w.cn/gtfcfyejdl.html

[Q01] 创建表
来源：http://hz.hammf.cn/gttpmnekyv.html

CREATE TABLE users (
来源：http://hz.cashguo.top/gtkvyvesmq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jqgufenzy.top/gtwtkvslrk.html

name VARCHAR(50) NOT NULL,
来源：http://hz.gogol.net.cn/gtkbnzeqpd.html

email VARCHAR(100) UNIQUE,
来源：http://hz.yonumen.top/gthasdsqqr.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.0kj1m.cn/gtpoetcnth.html

);
来源：http://hz.birdmap.top/gtvpotrpwu.html

[Q02] 创建带外键的表
来源：http://hz.chenzaomai.com/gtnnozuxgt.html

CREATE TABLE orders (
来源：http://hz.0kj1m.cn/gtghovgyov.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.c1oappe.top/gtodinrrwz.html

user_id INT NOT NULL,
来源：http://hz.xingfuxueyuan.xyz/gthukgcmrw.html

amount DECIMAL(10, 2),
来源：http://hz.jiagoushi.top/gtzkacjzhh.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.dianchejie.cn/gtbtsgdncx.html

);
来源：http://hz.xinyue.icu/gtnclcmnth.html

[Q03] 增加列
来源：http://hz.cashguo.top/gtbxjftlrg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.smart0.xyz/gtrgokyrgi.html

[Q04] 修改列类型
来源：http://hz.bjfxy.top/gtemohnsav.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.nanxinkj.top/gtuwtofdpk.html

[Q05] 重命名列
来源：http://hz.vqdsnc.cn/gtekpyizgc.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.jinghuilouyu.cn/gtfpvlfogc.html

[Q06] 删除列
来源：http://hz.redwolf501.top/gtlntgtowu.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.meibo888.top/gtpqebmhpa.html

[Q07] 删除表
来源：http://hz.dianchejie.cn/gtpwbvirmj.html

DROP TABLE IF EXISTS orders;
来源：http://hz.quarkkingdee.top/gtmczdspra.html

[Q08] 创建普通索引
来源：http://hz.dianchejie.cn/gtgimoqwun.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jlsjyb.cn/gtivmbsiet.html

[Q09] 创建唯一索引
来源：http://hz.ydzc1.top/gtluivcykt.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.sweek.top/gtgmczspru.html

[Q10] 插入单行
来源：http://hz.shangyingyoupin.top/gtvlzvqubf.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.tian-w.cn/gtfrdpgkrm.html

[Q11] 一次插入多行
来源：http://hz.gogol.net.cn/gtsuqdpzei.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.shzxlz.cn/gtqmmqsdte.html

[Q12] 插入后取自增 ID
来源：http://hz.9152youxi.cn/gteivponhl.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.pengpengdd.cyou/gthxxblgcg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.316326.xyz/gtujffdluv.html

[Q13] 忽略重复插入
来源：http://hz.bjfxy.top/gtjyorzsqa.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.zhongyouzk.top/gtlnjgcqnt.html

[Q14] 存在则更新（upsert）
来源：http://hz.zycfv.cn/gtcrzbkvav.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.yuxming.cn/gtaxcrnzvv.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.xuanzx.com/gthyqqbcmx.html

[Q15] 查询全部
来源：http://hz.quarkkingdee.top/gtaldoamto.html

SELECT * FROM users;
来源：http://hz.shanyushiyangkeji.top/gtdxktkdjd.html

[Q16] 查询指定列
来源：http://hz.tian-w.cn/gtuxhvggnv.html

SELECT id, name FROM users;
来源：http://hz.jinqigfzy.top/gteioulbdd.html

[Q17] 条件查询
来源：http://hz.xinyue.icu/gtmbhderyh.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.tian-w.cn/gtuclqenkq.html

[Q18] 模糊匹配
来源：http://hz.aibaodan.cn/gthwkrlfju.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.nanxuanxn.top/gtvonyiomb.html

[Q19] 范围查询
来源：http://hz.cdnleiting.top/gtieqwxjph.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.ppjwa.cn/gtybwnowcv.html

[Q20] IN 列表
来源：http://hz.tanke756.top/gtdcuxzunf.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.hongshengwenyu.top/gtjrlxxvyc.html

[Q21] 空值判断
来源：http://hz.yj20258.top/gtchzkakbg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.tian-w.cn/gtkajkkfzx.html

[Q22] 排序
来源：http://hz.sxryk.cn/gtvhlqmpuf.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.meibo888.top/gtavxgtosv.html

[Q23] 分页
来源：http://hz.zhixingplan.top/gtlvfuwysl.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yj202588.top/gtuvylhjnd.html

[Q24] 去重
来源：http://hz.shzxlz.cn/gtuvtcjffe.html

SELECT DISTINCT city FROM users;
来源：http://hz.yj202588.top/gtbjpqeysv.html

[Q25] 只取前 N 条
来源：http://hz.ydzc1.top/gtdpdxwqnr.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.ppjwa.cn/gtdxtljrsh.html

[Q26] 计数
来源：http://hz.haohaochexian.top/gtbgkjlxsh.html

SELECT COUNT(*) FROM users;
来源：http://hz.sufxvd.cn/gtzatgezrl.html

[Q27] 条件计数
来源：http://hz.jlsjyb.cn/gtdkzhdjna.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.ivvv.top/gttowriwip.html

[Q28] 求和与平均
来源：http://hz.gogol.net.cn/gtzkvkidzg.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.fengsongda.top/gtbrwqtujz.html

[Q29] 最大最小值
来源：http://hz.zhoulong.xyz/gtrnpyeqyi.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.zdqjudy.top/gtjdqhsvsn.html

[Q30] 分组统计
来源：http://hz.shanyushiyangkeji.top/gtsvsffbni.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.haohaochexian.top/gtjywcqhob.html

[Q31] 分组后过滤
来源：http://hz.jianghu66.top/gtuewgxbya.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yj20258.top/gthasiljst.html

[Q32] 分组拼接字符串
来源：http://hz.zhengqikj.top/gtpcyzclgy.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.ywan-chungtsiang.top/gteznkytmc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.nanxinkj.top/gtaivrzkrj.html

[Q33] 多列分组
来源：http://hz.tanke756.top/gtbqkjyyja.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.zhengqikj.top/gtkstigvwx.html

[Q34] 每组取第一条
来源：http://hz.yj20258.top/gtmipeknbe.html

SELECT * FROM (
来源：http://hz.yongpay.top/gtleumkryt.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.hywenlv.cn/gtmhwpypdh.html

) t WHERE rn = 1;
来源：http://hz.sysykeji.top/gtfsktsnnh.html

[Q35] 内连接
来源：http://hz.ivvv.top/gtdyfmwrci.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.yj20258.top/gtaqwithmf.html

[Q36] 左连接
来源：http://hz.chenjidiqi.icu/gtttiidhwh.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.birdmap.top/gtgllfqwrr.html

[Q37] 右连接
来源：http://hz.yj202588.top/gtuehoycmd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.birdmap.top/gtvvwyefsw.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.sxryk.cn/gtiskhznwt.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.yonumen.top/gtibjfyypt.html

[Q39] 自连接（查上下级）
来源：http://hz.yuanzhike.top/gtszolumni.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.zycfv.cn/gtjlojpsof.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.dianchejie.cn/gtipbynhkd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.smart0.xyz/gtwliayesb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.jinqigfzy.top/gtipexquqc.html

[Q41] 多表连接
来源：http://hz.zhongyouzk.top/gtnmjkkcci.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.jqgfzy.top/gtzmscrnhb.html

JOIN users u ON u.id = o.user_id
来源：http://hz.pengpengdd.cyou/gtbzbobusz.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.hongshengwenyu.top/gtzsoxzuev.html

[Q42] 连接条件附加过滤
来源：http://hz.hnxiangtu.top/gtdeergrvo.html

SELECT u.name, o.amount FROM users u
来源：http://hz.shanyushiyangtech.top/gtyswngnch.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.mhx1999.top/gtmmhfmlxh.html

[Q43] 标量子查询
来源：http://hz.nwbrower.top/gtqditjwco.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.jinyuanbaomall.cn/gthdcjnioa.html

[Q44] IN 子查询
来源：http://hz.gogol.net.cn/gtcvrkyscx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.nwbrower.top/gtanfjrhap.html

[Q45] EXISTS 判断存在
来源：http://hz.ydjk.org.cn/gtljtfdukr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.aizwys.cn/gtwgjbzpjq.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.zdqjudy.top/gtpntgondi.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.wangshuangyany.cn/gtfodsrnlo.html

[Q47] 与平均值比较
来源：http://hz.nanxinkj.top/gtjbauzfzn.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.zhoulong.xyz/gtqarygdhk.html

[Q48] CTE 公用表表达式
来源：http://hz.svipenyu.cn/gteeseoqsn.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.wangdashe.top/gtsctkhaew.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.guannengcc.top/gtiixaypau.html

[Q49] 更新单行
来源：http://hz.zdqjudy.top/gtxzaxjdbs.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.zhixingplan.top/gthlgyyphm.html

[Q50] 批量更新
来源：http://hz.cheryme.top/gtlrgjgcar.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.jyoumei.cn/gtkwcbjnlu.html

[Q51] 用子查询更新
来源：http://hz.havefunace.top/gtylrvrrli.html


<!-- 参考信息 -->