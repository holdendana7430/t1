代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.havefunace.top/gtipyvmpfz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.pengpengdd.cyou/gtgvyjhoft.html

TS:   // 手写 Map<string, number>
来源：http://hz.xziqi.cn/gthrroijmx.html

Java: // 手写 HashMap
来源：http://hz.xziqi.cn/gtpnasfzny.html

Go:   // 手写 map[int]int
来源：http://hz.hnqzz.top/gtryyvwixi.html

Ruby: // 手写 Hash
来源：http://hz.xuetiantiany.cn/gtolnyechd.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.cucudq.cn/gtdflvoueh.html

[N08] 生成全排列
来源：http://hz.yangfankeji.com/gtsrgnluue.html

Py:   itertools.permutations(arr)
来源：http://hz.dianchejie.cn/gtlkpjzyjo.html

PHP:  // 手写递归交换
来源：http://hz.xuetiantiany.cn/gtggusspzk.html

JS:   // 手写回溯递归
来源：http://hz.cashguo.top/gthkyupczp.html

TS:   // 手写回溯递归
来源：http://hz.jinghuilouyu.cn/gtrodgdqte.html

Java: // 手写回溯递归
来源：http://hz.pycfn.com/gtpdhxwfdj.html

Go:   // 手写回溯递归
来源：http://hz.xziqi.cn/gtkjruhzpr.html

Ruby: arr.permutation.to_a
来源：http://hz.cdnleiting.top/gtokmqqpnp.html

C#:   // 手写回溯递归
来源：http://hz.daria6918.cn/gtujzqkpln.html

[N09] 栈与队列
来源：http://hz.yvedp.cn/gtyoupligw.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.fzhhl.top/gtdjtxpfws.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.chenzaomai.com/gtxdwhoans.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.birdmap.top/gtmwpghavw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.zdqjudy.top/gtfgxgvbhy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.mhx1999.top/gttajsbisa.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.yj20258.top/gtdsdujugf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.gotoacloud.top/gtzecbzlby.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.ywan-chungtsiang.top/gtswerldla.html

[N10] 链表节点定义
来源：http://hz.jqgufenzy.top/gttbyoiodn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.52xcode.cn/gtvkjiyzmb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.yonumen.top/gtmpzliufx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.wangdashe.top/gtudjrkpxr.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.yonumen.top/gtzslzwgim.html

Java: class Node { int v; Node next; }
来源：http://hz.quarkkingdee.top/gtwkvwmxvs.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.zhaomingkeji.xyz/gtnfmpkqjk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.tanke756.top/gtcvxnupif.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.aizwys.cn/gtbakoydni.html

[N11] 二叉树中序遍历
来源：http://hz.shangyingyoupin.top/gtdslbznlz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.yonumen.top/gtsihiswks.html

PHP:  // 手写递归函数
来源：http://hz.nanxuanxn.top/gtjaxnpswm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jianghu66.top/gtuglwlsiz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yonumen.top/gtpkgizrli.html

Java: // 手写递归
来源：http://hz.zhaomingkeji.xyz/gthluvrpgy.html

Go:   // 手写递归
来源：http://hz.gotoacloud.top/gtrycfedcm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.hammf.cn/gtsgwvbzwz.html

C#:   // 手写递归
来源：http://hz.daxiang520.top/gtudskdmuy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.xuetiantiany.cn/gtaswdbaab.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.haohaochexian.top/gtxsdxmdos.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.aizwys.cn/gtvtsgbjvk.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cqqwz.cn/gttvxfhmoz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ivvv.top/gtssesdnbe.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yongpay.top/gtbwbyqtvx.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.yuxming.cn/gtuqcqbgpo.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.haohaochexian.top/gtsjhbtdjw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jqgfzy.top/gtykkovdne.html

================================================================================
来源：http://hz.yangfankeji.com/gtntnevygc.html

O. 并发与异步
来源：http://hz.jinqigufen.top/gtkhvucycg.html

================================================================================
来源：http://hz.sysykeji.top/gtjlxpxtnc.html

[O01] 启动一个线程
来源：http://hz.jianghu66.top/gtshubbifj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.zhaomingkeji.xyz/gtqmnknswr.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.mhx1999.top/gtwagokjvp.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.yj20258888.top/gtdpbwbsny.html

TS:   // 同 JS
来源：http://hz.iojbl.cn/gtpyqebbvw.html

Java: new Thread(() -> f()).start()
来源：http://hz.jqgufenzy.top/gtdfxaopsd.html

Go:   go f()
来源：http://hz.xylfe.cn/gtbwnumefo.html

Ruby: Thread.new { f }
来源：http://hz.nanxuanxn.top/gtgkzyhihq.html

C#:   Task.Run(() => F());
来源：http://hz.hfpthk.cn/gtwebdnlyb.html

[O02] 使用线程池
来源：http://hz.wangdashe.top/gtoiqoxkmt.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.sxryk.cn/gtdfjqkeps.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.tianlin.xyz/gtdtkxgdom.html

JS:   // worker_threads 线程池
来源：http://hz.jqgufenzy.top/gtvvxlviyz.html

TS:   // worker_threads 线程池
来源：http://hz.kuanghao11.cn/gttxaonmbr.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.jyoumei.cn/gtkgtynycg.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.pengpengdd.cyou/gtnrvplyeu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.smart0.xyz/gtxcoezgel.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.sufxvd.cn/gtcatcvoyr.html

[O03] 加锁保护共享数据
来源：http://hz.wangdashe.top/gtvmowurto.html

Py:   with lock: shared += 1
来源：http://hz.aizwys.cn/gtyvtwvjaj.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zhaomingkeji.xyz/gttgzuprii.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.guannengcc.top/gtklvbvrii.html

TS:   // 同 JS
来源：http://hz.cqqwz.cn/gteklwcinr.html

Java: synchronized (this) { shared++; }
来源：http://hz.hywenlv.cn/gteheiynrt.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.jinyuanbaomall.cn/gtbnsglvgd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.ydjk.org.cn/gtjfpnpygt.html

C#:   lock (gate) { shared++; }
来源：http://hz.chenlongwang.top/gtutjetfju.html

[O04] 定义异步函数并等待
来源：http://hz.haohaochexian.top/gtcalcqtds.html

Py:   async def f():⏎    await g()
来源：http://hz.sysykeji.top/gtrwrjbmez.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.cdnleiting.top/gtefzaataq.html

JS:   async function f() { await g(); }
来源：http://hz.xziqi.cn/gtsumvfxhg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.ehwqpu.com/gtngyamwfj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.wangshuangyany.cn/gtzmfrfgpw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.nanxuanxn.top/gtzypfgkfz.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.xuanzx.com/gtpfimksoh.html

C#:   async Task F() { await G(); }
来源：http://hz.guowangkeji.top/gtobamdvkl.html

[O05] 并发执行并等待全部完成
来源：http://hz.havefunace.top/gtctwxvwli.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jianghu66.top/gtoenyhtua.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.hywenlv.cn/gtgbthbvlp.html

JS:   await Promise.all(tasks)
来源：http://hz.316326.xyz/gtpjzkreec.html

TS:   await Promise.all(tasks)
来源：http://hz.yueranfly.top/gtqysmhchj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.yj20258888.top/gtrmcmuyzz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.tian-w.cn/gtywzbbhek.html

Ruby: threads.map(&:join)
来源：http://hz.cdnleiting.top/gttuisgysb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.xuetiantiany.cn/gtfeegkoio.html

[O06] 使用进程池
来源：http://hz.jinyuanbaomall.cn/gtumcrcwmg.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.xziqi.cn/gtpvksrgje.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.jiagoushi.top/gtewsmfazr.html

JS:   // child_process / cluster 模块
来源：http://hz.jyoumei.cn/gtapeqhytp.html

TS:   // child_process / cluster 模块
来源：http://hz.0kj1m.cn/gtzodupjdl.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.0kj1m.cn/gtsmvgrpuk.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.hfpthk.cn/gthbphgztn.html

Ruby: // fork 块
来源：http://hz.cheryme.top/gtzpfpjoka.html

C#:   Parallel.For
来源：http://hz.dashuyun.cn/gthchyyguc.html

================================================================================
来源：http://hz.chenlongwang.top/gtfwwkemlz.html

P. 常用工具函数
来源：http://hz.jinqigfzy.top/gtkyzcustv.html

================================================================================
来源：http://hz.wangdashe.top/gterlhreqp.html

[P01] 生成 UUID
来源：http://hz.316326.xyz/gtombhedmr.html

Py:   str(uuid.uuid4())
来源：http://hz.gzhubu.top/gtvzxcbhcw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.chenlongwang.top/gtcvizhbis.html

JS:   crypto.randomUUID()
来源：http://hz.cqqwz.cn/gtzttfffgs.html

TS:   crypto.randomUUID()
来源：http://hz.pengpengdd.cyou/gtgxnrfwsd.html

Java: UUID.randomUUID().toString()
来源：http://hz.aibaodan.cn/gtyuderrgc.html

Go:   // 用 github.com/google/uuid
来源：http://hz.daxiang520.top/gtqlayilbh.html

Ruby: SecureRandom.uuid
来源：http://hz.feifeiyinyue.top/gticzcmzhr.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.dashuyun.cn/gtdrruvhqb.html

[P02] MD5 / SHA256 摘要
来源：http://hz.sweek.top/gtriqivzsk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.yj20258888.top/gtzojmpfyq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.cdnleiting.top/gtgyvcbmyi.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.sxryk.cn/gtkorxcokk.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jqgufenzy.top/gtknaogpor.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.ywan-chungtsiang.top/gtsdphvdwi.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.cheryme.top/gtplyyflvq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.tian-w.cn/gtmbrcwgft.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.shangyingyoupin.top/gtijllkidd.html

[P03] 生成短随机字符串
来源：http://hz.dianchejie.cn/gtnogqwvkc.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.hnxiangtu.top/gtpgnzwzwa.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.shzxlz.cn/gttihdmctx.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jinqigfzy.top/gtfhsispat.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.bjfxy.top/gtjcfwscnr.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.redwolf501.top/gtpvgztxpc.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.zhoulong.xyz/gtezskzlpd.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.nanxinkj.top/gtlnrrlhqs.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.xylfe.cn/gtnihlcdse.html

[P04] 求长度
来源：http://hz.shanyushiyangtech.top/gthohcblig.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.gzhubu.top/gteboxloct.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.fengsongda.top/gtqedmcrhm.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jinqigufen.top/gtkivzknzt.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ydjk.org.cn/gtxipdqrcl.html

Java: list.size();  map.size();  s.length()
来源：http://hz.dashuyun.cn/gtpcfxuktt.html

Go:   len(arr);  len(m)
来源：http://hz.xuanzx.com/gtvpfwrtiv.html

Ruby: x.length;  x.size
来源：http://hz.gogol.net.cn/gtrykzfmqz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.hfpthk.cn/gttfsmvzei.html

[P05] 判断两个对象内容是否相等
来源：http://hz.hywenlv.cn/gtzowydhel.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.xinyue.icu/gtybxejtpc.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.0kj1m.cn/gtadknijof.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.pycfn.com/gtsodatqlw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jinyuanbaomall.cn/gtcelkpiwa.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.bjfxy.top/gtajktdgdz.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.fzhhl.top/gtwttlloog.html

Ruby: a == b
来源：http://hz.pycfn.com/gtblpsalfl.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.0kj1m.cn/gtnzxestrx.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.tian-w.cn/gtvfnzceys.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.xziqi.cn/gtngfnyhpe.html

PHP:  if (empty($x)) {}
来源：http://hz.jqgufenzy.top/gtcupzifdr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.chenzaomai.com/gtwdbuwsjo.html

TS:   if (x == null) {}
来源：http://hz.svipenyu.cn/gteacipzxm.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.aibaodan.cn/gtmrezrfmd.html

Go:   if x == nil {}
来源：http://hz.shzxlz.cn/gtoyxrbiol.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.hywenlv.cn/gtvgkahset.html

C#:   if (x is null) {}
来源：http://hz.316326.xyz/gtklwyahld.html

[P07] 防抖与节流
来源：http://hz.yuanzhike.top/gtmyxsyzen.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.zhongyouzk.top/gtwigvoaav.html

PHP:  // 手写时间戳比较
来源：http://hz.hywenlv.cn/gtmdmzawdp.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.svipenyu.cn/gthiwkuzpi.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yanxiufei.cn/gtyqmmuwhn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.jinyuanbaomall.cn/gtmgdfgamf.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.cashguo.top/gtfahzevmq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.vqdsnc.cn/gtgbwlgduq.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.zhengqikj.top/gtimjlqymz.html

[P08] 处理浮点精度问题
来源：http://hz.dianchejie.cn/gtzftkzchl.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.hnxiangtu.top/gtvbzjvrrw.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.tanke756.top/gtmtiowhsf.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.chenjidiqi.icu/gtklysbcan.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.shuidangran.top/gtpbbspbgq.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.guowangkeji.top/gtdmztklhy.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.zhengqikj.top/gtblrkztaj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.hammf.cn/gtsvyxokos.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.feifeiyinyue.top/gtgaxbyrab.html

================================================================================
来源：http://hz.tian-w.cn/gtfwvthijf.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.tian-w.cn/gtqoqfwlpq.html

================================================================================
来源：http://hz.mhx1999.top/gtfsdhpqca.html

[Q01] 创建表
来源：http://hz.hammf.cn/gthvfvbtqx.html

CREATE TABLE users (
来源：http://hz.shzxlz.cn/gttmzjhepw.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xinyue.icu/gtalenthhx.html

name VARCHAR(50) NOT NULL,
来源：http://hz.smart0.xyz/gtiwhkbygv.html

email VARCHAR(100) UNIQUE,
来源：http://hz.yvedp.cn/gttvwevmkf.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.gzhubu.top/gtmruzrhql.html

);
来源：http://hz.zycfv.cn/gtkesfplkz.html

[Q02] 创建带外键的表
来源：http://hz.iojbl.cn/gtsaipcksk.html

CREATE TABLE orders (
来源：http://hz.hnqzz.top/gttbwjivpf.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.chenlongwang.top/gtsqfmejfp.html

user_id INT NOT NULL,
来源：http://hz.yuxming.cn/gtczorpvkl.html

amount DECIMAL(10, 2),
来源：http://hz.9152youxi.cn/gtjtbivqiw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.cheryme.top/gtxoqxfabc.html

);
来源：http://hz.xuetiantiany.cn/gtohbjabra.html

[Q03] 增加列
来源：http://hz.jinqigfzy.top/gtdzxzsdql.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.gaohongyu789.top/gttwnmzliu.html

[Q04] 修改列类型
来源：http://hz.haohaochexian.top/gtcaoipuox.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.zhijiandao.cn/gthtywhpen.html

[Q05] 重命名列
来源：http://hz.ywan-chungtsiang.top/gtwyamisgw.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.yuanzhike.top/gtlvpqnxcf.html

[Q06] 删除列
来源：http://hz.xziqi.cn/gtfdyzipov.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.kuanghao11.cn/gtznatpwla.html

[Q07] 删除表
来源：http://hz.tian-w.cn/gtiyjofjko.html

DROP TABLE IF EXISTS orders;
来源：http://hz.pengpengdd.cyou/gtcfuvschx.html

[Q08] 创建普通索引
来源：http://hz.jinghuilouyu.cn/gtbkzuvdvi.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.yuxming.cn/gtoedvtlew.html

[Q09] 创建唯一索引
来源：http://hz.cqqwz.cn/gtcensqaud.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.xingfuxueyuan.xyz/gtxeosssua.html

[Q10] 插入单行
来源：http://hz.hywenlv.cn/gtnbakldyq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.bjfxy.top/gtyqbxcphf.html

[Q11] 一次插入多行
来源：http://hz.pycfn.com/gtyiykwkql.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.tianlin.xyz/gtxhrhndpn.html

[Q12] 插入后取自增 ID
来源：http://hz.chenlongwang.top/gtlslemqzx.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.hfpthk.cn/gtramntkqv.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yonumen.top/gtwykjblsh.html

[Q13] 忽略重复插入
来源：http://hz.svipenyu.cn/gtaphdoifu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.snrcjt.cn/gtvvhbikaw.html

[Q14] 存在则更新（upsert）
来源：http://hz.jyoumei.cn/gtgtbxoinz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.zycfv.cn/gtusxzjkay.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.ppjwa.cn/gtmxdwcyqv.html

[Q15] 查询全部
来源：http://hz.gogol.net.cn/gtghdvdfll.html

SELECT * FROM users;
来源：http://hz.guannengcc.top/gtqrxgayvx.html

[Q16] 查询指定列
来源：http://hz.birdmap.top/gtgddzggfp.html

SELECT id, name FROM users;
来源：http://hz.zhengqikj.top/gtxumwuusk.html

[Q17] 条件查询
来源：http://hz.sweek.top/gtubfrkccp.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.zhongyouzk.top/gtvlbhjlvz.html

[Q18] 模糊匹配
来源：http://hz.c1oappe.top/gtrpwpnict.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.guannengcc.top/gteembuiya.html

[Q19] 范围查询
来源：http://hz.mhx1999.top/gtfxihejjr.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.zdqjudy.top/gtxvpwalyv.html

[Q20] IN 列表
来源：http://hz.dashuyun.cn/gtydwunnwn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.zhixingplan.top/gtjwthsbao.html

[Q21] 空值判断
来源：http://hz.yj20258.top/gtkholgavp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.jinyuanbaomall.cn/gtzxvfjdmx.html

[Q22] 排序
来源：http://hz.guowangkeji.top/gtgwmkxrgt.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.jyoumei.cn/gttvuxiaca.html

[Q23] 分页
来源：http://hz.ywan-chungtsiang.top/gtcmxybeje.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.hfpthk.cn/gtuwqctovv.html

[Q24] 去重
来源：http://hz.hnxiangtu.top/gtkdxafxza.html

SELECT DISTINCT city FROM users;
来源：http://hz.jyoumei.cn/gtrgnotgkm.html

[Q25] 只取前 N 条
来源：http://hz.meibo888.top/gtszjvgosk.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.yonumen.top/gtrquobomq.html

[Q26] 计数
来源：http://hz.nanxuanxn.top/gtbcqwlvwk.html

SELECT COUNT(*) FROM users;
来源：http://hz.yj20258888.top/gtkbmkfojb.html

[Q27] 条件计数
来源：http://hz.xingfuxueyuan.xyz/gtoacbdcqe.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.fzhhl.top/gtwtrrwtjw.html

[Q28] 求和与平均
来源：http://hz.gotoacloud.top/gtostrnqya.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.xuanzx.com/gtofwnpkbn.html

[Q29] 最大最小值
来源：http://hz.cheryme.top/gtilalmkls.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.zhongyouzk.top/gtvkzbgarg.html

[Q30] 分组统计
来源：http://hz.yongpay.top/gtmbwlcvok.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.yj202588.top/gtjdxonocq.html

[Q31] 分组后过滤
来源：http://hz.dashuyun.cn/gtvmadpcvd.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.jinghuilouyu.cn/gthxjxhgzc.html

[Q32] 分组拼接字符串
来源：http://hz.guannengcc.top/gtzvwomfds.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.fzhhl.top/gtgsgpnhzr.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.ywan-chungtsiang.top/gtiogofesm.html

[Q33] 多列分组
来源：http://hz.hongshengwenyu.top/gtfeznskln.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.feifeiyinyue.top/gtdkmdlfya.html

[Q34] 每组取第一条
来源：http://hz.xinyue.icu/gtlrknrcsl.html

SELECT * FROM (
来源：http://hz.hammf.cn/gttnatowgh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.52xcode.cn/gtgagbfker.html

) t WHERE rn = 1;
来源：http://hz.zhaomingkeji.xyz/gtdcufhuny.html

[Q35] 内连接
来源：http://hz.haohaochexian.top/gtxxsajupn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.nwbrower.top/gtiaycyjkf.html

[Q36] 左连接
来源：http://hz.yanxiufei.cn/gtnmxnxztu.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.shzxlz.cn/gtrligmnrp.html

[Q37] 右连接
来源：http://hz.iojbl.cn/gtymvnnufy.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.aizwys.cn/gtzecubxbf.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.52xcode.cn/gtdlkfrngg.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.redwolf501.top/gtpnyciiuu.html

[Q39] 自连接（查上下级）
来源：http://hz.cdnleiting.top/gtzwcpjjcc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.0kj1m.cn/gthnywxtso.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.feifeiyinyue.top/gtaeafkgeo.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.hfpthk.cn/gthlmgpqqj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.cucudq.cn/gtlxpzupei.html

[Q41] 多表连接
来源：http://hz.gaohongyu789.top/gterqvmisn.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.tianlin.xyz/gtzmbpjejz.html

JOIN users u ON u.id = o.user_id
来源：http://hz.pycfn.com/gtffutenvf.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.gotoacloud.top/gtwepvonfp.html

[Q42] 连接条件附加过滤
来源：http://hz.iojbl.cn/gtnqgovtwj.html

SELECT u.name, o.amount FROM users u
来源：http://hz.0kj1m.cn/gtulnmjmle.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.sufxvd.cn/gtkzznuvqm.html

[Q43] 标量子查询
来源：http://hz.ydjk.org.cn/gtwoenhaof.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.iojbl.cn/gtnnyziffn.html

[Q44] IN 子查询
来源：http://hz.nanxuanxn.top/gtkwkyirtt.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.havefunace.top/gtnlxornkc.html

[Q45] EXISTS 判断存在
来源：http://hz.jqgufenzy.top/gtcdwccytj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.gaohongyu789.top/gtexgchqll.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.cdnleiting.top/gtiupmwplj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zycfv.cn/gtmopcvoil.html

[Q47] 与平均值比较
来源：http://hz.zhixingplan.top/gtxmuqtpyp.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.xuetiantiany.cn/gtxozkjxqs.html


<!-- 参考信息 -->