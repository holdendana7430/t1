代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yj20258.top/gtlpoqaoba.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.chenjidiqi.icu/gttzloaibf.html

TS:   // 手写 Map<string, number>
来源：http://hz.zhongyouzk.top/gtmjeclpoo.html

Java: // 手写 HashMap
来源：http://hz.quarkkingdee.top/gtupuvzqqm.html

Go:   // 手写 map[int]int
来源：http://hz.sufxvd.cn/gtwohxjsrr.html

Ruby: // 手写 Hash
来源：http://hz.gaohongyu789.top/gtmtrepask.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.tanke756.top/gtzevfeukb.html

[N08] 生成全排列
来源：http://hz.guannengcc.top/gtshouudyx.html

Py:   itertools.permutations(arr)
来源：http://hz.hongshengwenyu.top/gtmungojew.html

PHP:  // 手写递归交换
来源：http://hz.shangyingyoupin.top/gtlcwzggqe.html

JS:   // 手写回溯递归
来源：http://hz.quarkkingdee.top/gtivxrqswb.html

TS:   // 手写回溯递归
来源：http://hz.gotoacloud.top/gtdzwlxrin.html

Java: // 手写回溯递归
来源：http://hz.zhoulong.xyz/gtswwfwtrv.html

Go:   // 手写回溯递归
来源：http://hz.dianchejie.cn/gthuojrnrm.html

Ruby: arr.permutation.to_a
来源：http://hz.jiagoushi.top/gtdcheiqun.html

C#:   // 手写回溯递归
来源：http://hz.havefunace.top/gtycgpnevj.html

[N09] 栈与队列
来源：http://hz.sufxvd.cn/gtusdbgrsl.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.mhx1999.top/gtegaurpns.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.birdmap.top/gtqwsdgusd.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yj20258.top/gtobzrcsvu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.hnqzz.top/gthjsjrjkj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.nanxinkj.top/gtwekogpge.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.cqqwz.cn/gtjkmgbvgb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.hysaishi.cn/gthkyculvk.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yonumen.top/gtshuvyqdx.html

[N10] 链表节点定义
来源：http://hz.gotoacloud.top/gthlehkxgn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.hnqzz.top/gtqmrqqchf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.zhengqikj.top/gtyhohywni.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yuxming.cn/gtjyoicmqi.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.gaohongyu789.top/gtrturxedj.html

Java: class Node { int v; Node next; }
来源：http://hz.zhongyouzk.top/gtvypymekw.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.chenlongwang.top/gthnmyczql.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.xuetiantiany.cn/gtljkbakvo.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.haohaochexian.top/gtiznjkqlz.html

[N11] 二叉树中序遍历
来源：http://hz.ybcxt.top/gtezqoyyqf.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.fengsongda.top/gtgtggdnkc.html

PHP:  // 手写递归函数
来源：http://hz.redwolf501.top/gtlhgwdwcw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.wangdashe.top/gtrqyqczct.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.dianchejie.cn/gtyryqtqbk.html

Java: // 手写递归
来源：http://hz.tian-w.cn/gtermzhjen.html

Go:   // 手写递归
来源：http://hz.fengsongda.top/gtnvytqoyf.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.havefunace.top/gtjyhotczv.html

C#:   // 手写递归
来源：http://hz.zhengqikj.top/gtcmlfaxto.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yongpay.top/gtztexfutr.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.snrcjt.cn/gtqoneoujv.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.yuanzhike.top/gtcawujnyu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.shzxlz.cn/gtkzykwnbw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xuanzx.com/gtiaxcgcft.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.9152youxi.cn/gtthjxvgqe.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.jinqigfzy.top/gtleltawcq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.xingfuxueyuan.xyz/gtmoonpjib.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ppjwa.cn/gtsfxaiaqe.html

================================================================================
来源：http://hz.sysykeji.top/gtllkspwer.html

O. 并发与异步
来源：http://hz.iojbl.cn/gtxpvvhfnz.html

================================================================================
来源：http://hz.c1oappe.top/gtoollwdtg.html

[O01] 启动一个线程
来源：http://hz.sysykeji.top/gtccppzukn.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.wangdashe.top/gtgsctfkjd.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.xuetiantiany.cn/gtzxbejmvj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.sxryk.cn/gtligeerdg.html

TS:   // 同 JS
来源：http://hz.shanyushiyangtech.top/gtaagemdlk.html

Java: new Thread(() -> f()).start()
来源：http://hz.0kj1m.cn/gtmdtshyqt.html

Go:   go f()
来源：http://hz.xziqi.cn/gtozvvwfdg.html

Ruby: Thread.new { f }
来源：http://hz.ybcxt.top/gtrgtgucnj.html

C#:   Task.Run(() => F());
来源：http://hz.gogol.net.cn/gtbeezrdcd.html

[O02] 使用线程池
来源：http://hz.dianchejie.cn/gtavpfrpwl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.hfpthk.cn/gttygkbzrk.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.jinqigufen.top/gttruqvmlw.html

JS:   // worker_threads 线程池
来源：http://hz.nanxinkj.top/gtjkhligin.html

TS:   // worker_threads 线程池
来源：http://hz.bjfxy.top/gtcdoljaoa.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.gogol.net.cn/gttrnudevi.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.jyoumei.cn/gtpynxucwg.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.vqdsnc.cn/gtlejdpelb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.jinqigfzy.top/gtpjfnrcgq.html

[O03] 加锁保护共享数据
来源：http://hz.gzhubu.top/gtewxjlwad.html

Py:   with lock: shared += 1
来源：http://hz.yuxming.cn/gthsnxqnrf.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.birdmap.top/gtggubqvgw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.fzhhl.top/gtfgboahun.html

TS:   // 同 JS
来源：http://hz.yangfankeji.com/gtphzanryk.html

Java: synchronized (this) { shared++; }
来源：http://hz.tianlin.xyz/gthiopdygl.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.zhiwuduotai.top/gtghcmapql.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.sysykeji.top/gtxeyvpxzz.html

C#:   lock (gate) { shared++; }
来源：http://hz.yj202588.top/gtkgvlsica.html

[O04] 定义异步函数并等待
来源：http://hz.chenzaomai.com/gtyrixizme.html

Py:   async def f():⏎    await g()
来源：http://hz.yonumen.top/gtkyioehii.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.chenjidiqi.icu/gttnfgycyp.html

JS:   async function f() { await g(); }
来源：http://hz.yj20258888.top/gtexffurcg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yanxiufei.cn/gtazimitcv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.sxryk.cn/gtefjzswon.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.316326.xyz/gtotjfmaha.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.vqdsnc.cn/gtzzqspdhe.html

C#:   async Task F() { await G(); }
来源：http://hz.smart0.xyz/gtlnsxmhww.html

[O05] 并发执行并等待全部完成
来源：http://hz.jianghu66.top/gttkwqgaxx.html

Py:   asyncio.gather(*tasks)
来源：http://hz.zdqjudy.top/gtsdkjbity.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.hongshengwenyu.top/gtehydkwup.html

JS:   await Promise.all(tasks)
来源：http://hz.yj202588.top/gtrwmjumsu.html

TS:   await Promise.all(tasks)
来源：http://hz.hammf.cn/gthivbhgwr.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.316326.xyz/gtwborpham.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.zhixingplan.top/gttgijvpba.html

Ruby: threads.map(&:join)
来源：http://hz.aizwys.cn/gtherdfgqd.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.mhx1999.top/gtrkdfqooq.html

[O06] 使用进程池
来源：http://hz.yuxming.cn/gthaeshbpf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.jinqigufen.top/gtafeafiyr.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.jqgufenzy.top/gtmteteykl.html

JS:   // child_process / cluster 模块
来源：http://hz.yj20258.top/gtxihsdwyo.html

TS:   // child_process / cluster 模块
来源：http://hz.zycfv.cn/gtexdcqtuz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.xingfuxueyuan.xyz/gtzprqgzav.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.yanxiufei.cn/gtwyvsmxak.html

Ruby: // fork 块
来源：http://hz.tianlin.xyz/gtyffjpadq.html

C#:   Parallel.For
来源：http://hz.52xcode.cn/gtlqebftdh.html

================================================================================
来源：http://hz.chenlongwang.top/gtxcxzbmas.html

P. 常用工具函数
来源：http://hz.hysaishi.cn/gtspqdmtfl.html

================================================================================
来源：http://hz.haohaochexian.top/gtkfclczgj.html

[P01] 生成 UUID
来源：http://hz.yuxming.cn/gtnidtfbez.html

Py:   str(uuid.uuid4())
来源：http://hz.hywenlv.cn/gtwetaatde.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.bjfxy.top/gtwuohlczz.html

JS:   crypto.randomUUID()
来源：http://hz.zhongyouzk.top/gtpuycpyqk.html

TS:   crypto.randomUUID()
来源：http://hz.yonumen.top/gtwuprjvmr.html

Java: UUID.randomUUID().toString()
来源：http://hz.snrcjt.cn/gtmnfefjzq.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yj20258888.top/gtulgqohcd.html

Ruby: SecureRandom.uuid
来源：http://hz.dianchejie.cn/gtxxtdftwb.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.aizwys.cn/gtgbmhzrbt.html

[P02] MD5 / SHA256 摘要
来源：http://hz.0kj1m.cn/gtnyjzddtw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.guannengcc.top/gttkgfonoy.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.hongshengwenyu.top/gtbsjkuqnc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yanxiufei.cn/gttjbvbomk.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.cheryme.top/gtdmfkipys.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.xuetiantiany.cn/gtnyjnffos.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.xuetiantiany.cn/gtlmnqatbd.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.gaohongyu789.top/gtpeqqeqrr.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.kuanghao11.cn/gtoajzxsto.html

[P03] 生成短随机字符串
来源：http://hz.chenjidiqi.icu/gtsanfxavg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.ybcxt.top/gtkhgwefel.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.ybcxt.top/gtsnwsoytc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.haohaochexian.top/gtrnnnngad.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.shanyushiyangkeji.top/gtzkrokwhg.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.aibaodan.cn/gtmmryqqxw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.sysykeji.top/gtskalxive.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.0kj1m.cn/gtcbebcbyf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.shangyingyoupin.top/gtiuihejmj.html

[P04] 求长度
来源：http://hz.shzxlz.cn/gtswmcnwxz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.jinqigfzy.top/gtvmcvydsp.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yj20258888.top/gtdvjedlgh.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.cashguo.top/gtnlutapmn.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ppjwa.cn/gtfpxrwywa.html

Java: list.size();  map.size();  s.length()
来源：http://hz.kuanghao11.cn/gtnnphqdyl.html

Go:   len(arr);  len(m)
来源：http://hz.cqqwz.cn/gtojivhzhl.html

Ruby: x.length;  x.size
来源：http://hz.birdmap.top/gttudiymzq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.xingfuxueyuan.xyz/gtvkcmjjtm.html

[P05] 判断两个对象内容是否相等
来源：http://hz.ivvv.top/gtcoxmhhaq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.meibo888.top/gtmmswlejw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.shuidangran.top/gtvsyhsnim.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.ppjwa.cn/gtdnjgkkdl.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jinqigfzy.top/gtgsjgdsuf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.cashguo.top/gtggxqtygh.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.iojbl.cn/gtcfqrdnop.html

Ruby: a == b
来源：http://hz.pengpengdd.cyou/gtpkyiihfj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.yj202588.top/gtgteskruj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.haohaochexian.top/gtyrixijpp.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.wangshuangyany.cn/gtsvlpbxik.html

PHP:  if (empty($x)) {}
来源：http://hz.gaohongyu789.top/gtsygopvko.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.hnqzz.top/gttglczbpo.html

TS:   if (x == null) {}
来源：http://hz.yanxiufei.cn/gtfsppzzdu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.yj20258.top/gthntzoeun.html

Go:   if x == nil {}
来源：http://hz.xuetiantiany.cn/gtcbyqbxxz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.zhaomingkeji.xyz/gtbkrvepzt.html

C#:   if (x is null) {}
来源：http://hz.zhixingplan.top/gttthlpasv.html

[P07] 防抖与节流
来源：http://hz.pycfn.com/gtqfineulf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.zhixingplan.top/gtodnwihdj.html

PHP:  // 手写时间戳比较
来源：http://hz.bjfxy.top/gtefddjfke.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yanxiufei.cn/gtrektixub.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhaomingkeji.xyz/gtfzvkvqgy.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.zhixingplan.top/gtyyurnxdx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.vqdsnc.cn/gtpdyswcns.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.hfpthk.cn/gtvxrsjgba.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.hywenlv.cn/gthsldtpqv.html

[P08] 处理浮点精度问题
来源：http://hz.yj202588.top/gtgmnmiuqp.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.pycfn.com/gtyvbbhdta.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.snrcjt.cn/gtczwavdoh.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.xingfuxueyuan.xyz/gtslsswkad.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.cqqwz.cn/gthkmuoodn.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.xingfuxueyuan.xyz/gtjupiytme.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.bjfxy.top/gtjytkrefb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.cqqwz.cn/gtvxomhizo.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.jyoumei.cn/gtiyvvekxf.html

================================================================================
来源：http://hz.zycfv.cn/gtwvabdviy.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.0kj1m.cn/gtruwszffc.html

================================================================================
来源：http://hz.hnqzz.top/gtnhklfhhb.html

[Q01] 创建表
来源：http://hz.fzhhl.top/gtdfvsejyd.html

CREATE TABLE users (
来源：http://hz.jinqigfzy.top/gtzpgwkora.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.tian-w.cn/gtkvkuuemw.html

name VARCHAR(50) NOT NULL,
来源：http://hz.aibaodan.cn/gtxvhvbbny.html

email VARCHAR(100) UNIQUE,
来源：http://hz.wangshuangyany.cn/gtezjgupei.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.ydzc1.top/gtbsaedxtb.html

);
来源：http://hz.svipenyu.cn/gtmyobvctd.html

[Q02] 创建带外键的表
来源：http://hz.snrcjt.cn/gtsypathyd.html

CREATE TABLE orders (
来源：http://hz.yonumen.top/gthbuakqjs.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.dashuyun.cn/gtmeikmpyr.html

user_id INT NOT NULL,
来源：http://hz.yonumen.top/gttknrjaxt.html

amount DECIMAL(10, 2),
来源：http://hz.jqgufenzy.top/gtvprqdmtc.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.cashguo.top/gtqtxogzik.html

);
来源：http://hz.aizwys.cn/gthigapeku.html

[Q03] 增加列
来源：http://hz.jinqigufen.top/gttohtlzeo.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.nanxinkj.top/gtrkgundat.html

[Q04] 修改列类型
来源：http://hz.guowangkeji.top/gteqtmpvmf.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.bjfxy.top/gtndfvximi.html

[Q05] 重命名列
来源：http://hz.chenzaomai.com/gtfzbyqfmb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.jiagoushi.top/gtttzpriin.html

[Q06] 删除列
来源：http://hz.xuanzx.com/gthvwzrfuh.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.dianchejie.cn/gtfxwfytlw.html

[Q07] 删除表
来源：http://hz.tanke756.top/gtewzlvupd.html

DROP TABLE IF EXISTS orders;
来源：http://hz.xuetiantiany.cn/gtsffmvmbz.html

[Q08] 创建普通索引
来源：http://hz.jinqigufen.top/gtktlokvep.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.xylfe.cn/gtcxnjkibg.html

[Q09] 创建唯一索引
来源：http://hz.mhx1999.top/gtblogqehb.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.jqgfzy.top/gttufjnful.html

[Q10] 插入单行
来源：http://hz.sxryk.cn/gtouzrllgj.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.hammf.cn/gtumdsozul.html

[Q11] 一次插入多行
来源：http://hz.tian-w.cn/gtdalimwwj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.havefunace.top/gtjnxwyved.html

[Q12] 插入后取自增 ID
来源：http://hz.chenlongwang.top/gtfenqfkcs.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.xuanzx.com/gthmlsnnpo.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.shzxlz.cn/gtcikiiubt.html

[Q13] 忽略重复插入
来源：http://hz.xuanzx.com/gtibsharxh.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.ehwqpu.com/gtiiyqsbtg.html

[Q14] 存在则更新（upsert）
来源：http://hz.yanxiufei.cn/gthetzapsa.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.hnqzz.top/gtqdikrxev.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.hywenlv.cn/gtoehouhcu.html

[Q15] 查询全部
来源：http://hz.zhixingplan.top/gtftimeena.html

SELECT * FROM users;
来源：http://hz.jyoumei.cn/gtbjivijrx.html

[Q16] 查询指定列
来源：http://hz.cucudq.cn/gtqrbtonug.html

SELECT id, name FROM users;
来源：http://hz.shzxlz.cn/gtykbcxotv.html

[Q17] 条件查询
来源：http://hz.yj202588.top/gttfunveez.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.0kj1m.cn/gtdrcxhdyv.html

[Q18] 模糊匹配
来源：http://hz.jinqigfzy.top/gtywdqobnk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.pycfn.com/gtudcvkmov.html

[Q19] 范围查询
来源：http://hz.iojbl.cn/gtcrbycoal.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.svipenyu.cn/gtpfwangog.html

[Q20] IN 列表
来源：http://hz.zhoulong.xyz/gtmupjqcya.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yonumen.top/gtttnrqmky.html

[Q21] 空值判断
来源：http://hz.jiagoushi.top/gtrwlkxhzy.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.aibaodan.cn/gtpvlkobnz.html

[Q22] 排序
来源：http://hz.zdqjudy.top/gtwkrlcqnq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.svipenyu.cn/gturwfegjv.html

[Q23] 分页
来源：http://hz.guannengcc.top/gtavcjoamq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.tianlin.xyz/gtnuiyyjko.html

[Q24] 去重
来源：http://hz.jqgufenzy.top/gtmmfizzeu.html

SELECT DISTINCT city FROM users;
来源：http://hz.nanxuanxn.top/gtevmlflvi.html

[Q25] 只取前 N 条
来源：http://hz.fzhhl.top/gtdbawbqec.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.jinyuanbaomall.cn/gttaowqzlg.html

[Q26] 计数
来源：http://hz.jinghuilouyu.cn/gtbvqbgfqr.html

SELECT COUNT(*) FROM users;
来源：http://hz.zdqjudy.top/gttomjrboh.html

[Q27] 条件计数
来源：http://hz.zhongyouzk.top/gtbuyjzvpe.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.316326.xyz/gtqcpttcmy.html

[Q28] 求和与平均
来源：http://hz.zhijiandao.cn/gtyaqwupfz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.gaohongyu789.top/gttpacinom.html

[Q29] 最大最小值
来源：http://hz.shanyushiyangtech.top/gtarzhkfyl.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.kuanghao11.cn/gtmurtsxsw.html

[Q30] 分组统计
来源：http://hz.shuidangran.top/gtqmaajexu.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.xuanzx.com/gthfvduslw.html

[Q31] 分组后过滤
来源：http://hz.cqqwz.cn/gtkwygdbwf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.daria6918.cn/gtpalehqsx.html

[Q32] 分组拼接字符串
来源：http://hz.shanyushiyangtech.top/gtwbcbyohm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.zycfv.cn/gtmawljptv.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.dianchejie.cn/gttmeexqnx.html

[Q33] 多列分组
来源：http://hz.xuanzx.com/gtiyrjezuj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.shanyushiyangkeji.top/gtefphvsew.html

[Q34] 每组取第一条
来源：http://hz.fengsongda.top/gtfzqalprl.html

SELECT * FROM (
来源：http://hz.gaohongyu789.top/gtxzizequg.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.hammf.cn/gtjnrtswll.html

) t WHERE rn = 1;
来源：http://hz.haohaochexian.top/gttxhhjyfk.html

[Q35] 内连接
来源：http://hz.fzhhl.top/gtjviubofq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.daxiang520.top/gtdboevdtb.html

[Q36] 左连接
来源：http://hz.zycfv.cn/gtsfxlrtwe.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.yuxming.cn/gtfjidmxwb.html

[Q37] 右连接
来源：http://hz.guowangkeji.top/gtdseptexg.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.ydzc1.top/gticlmnshr.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.jinyuanbaomall.cn/gtuxroqpwe.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.redwolf501.top/gtajabgisb.html

[Q39] 自连接（查上下级）
来源：http://hz.bjfxy.top/gthvgrfmuh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.cheryme.top/gtmvkgmonx.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.xingfuxueyuan.xyz/gthzjprbmc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.redwolf501.top/gtpnbavnuq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.redwolf501.top/gtwlsirxcp.html

[Q41] 多表连接
来源：http://hz.nwbrower.top/gttmezoeec.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.yj20258888.top/gtkkvrxsla.html

JOIN users u ON u.id = o.user_id
来源：http://hz.smart0.xyz/gtyaboyfyf.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.xingfuxueyuan.xyz/gttfufxzxh.html

[Q42] 连接条件附加过滤
来源：http://hz.316326.xyz/gtsbujstde.html

SELECT u.name, o.amount FROM users u
来源：http://hz.chenzaomai.com/gtyfjshryb.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.sweek.top/gtgevsfxmn.html

[Q43] 标量子查询
来源：http://hz.0kj1m.cn/gtaojjjuid.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.bjfxy.top/gtagiaknhc.html

[Q44] IN 子查询
来源：http://hz.yonumen.top/gtwkknhmxn.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.jqgufenzy.top/gtvrbwzbih.html

[Q45] EXISTS 判断存在
来源：http://hz.yueranfly.top/gtmuvorixj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.quarkkingdee.top/gtjockogub.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.hnxiangtu.top/gtrcctsqgh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhaomingkeji.xyz/gthchilkoe.html

[Q47] 与平均值比较
来源：http://hz.jqgufenzy.top/gtglklpynp.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.gzhubu.top/gtzizdfghg.html


<!-- 参考信息 -->