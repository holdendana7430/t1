代发 wailian999

Py:   itertools.permutations(arr)
来源：http://hz.jinqigfzy.top/gtjqycfrgx.html

PHP:  // 手写递归交换
来源：http://hz.iojbl.cn/gtleesbiju.html

JS:   // 手写回溯递归
来源：http://hz.xuanzx.com/gtmmydoyuc.html

TS:   // 手写回溯递归
来源：http://hz.c1oappe.top/gtcxpkneah.html

Java: // 手写回溯递归
来源：http://hz.nanxuanxn.top/gtbkggcoqm.html

Go:   // 手写回溯递归
来源：http://hz.yongpay.top/gtlkjoggsw.html

Ruby: arr.permutation.to_a
来源：http://hz.zhiwuduotai.top/gtwglrzujs.html

C#:   // 手写回溯递归
来源：http://hz.shanyushiyangtech.top/gtkesnsxtq.html

[N09] 栈与队列
来源：http://hz.haohaochexian.top/gtwtcgoiwj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.jinghuilouyu.cn/gtxdydocxb.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.jqgfzy.top/gtovcudfmk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yvedp.cn/gtttjidsge.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.gogol.net.cn/gtqocinech.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yj202588.top/gtwvdcqmfh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.cqqwz.cn/gtockcaucg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.cqqwz.cn/gtdbdlfubh.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.aizwys.cn/gtfegaefar.html

[N10] 链表节点定义
来源：http://hz.cucudq.cn/gtutpclxhr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.dashuyun.cn/gtflmueovm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.gaohongyu789.top/gtxexbvsqx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.birdmap.top/gtejwlstbg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.nwbrower.top/gtlujgvsnn.html

Java: class Node { int v; Node next; }
来源：http://hz.jinqigufen.top/gtvzezbxoc.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.jyoumei.cn/gtlipnklnp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.bjfxy.top/gtwzuwbeny.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.nwbrower.top/gtdgzewvao.html

[N11] 二叉树中序遍历
来源：http://hz.ivvv.top/gtsjhtqdkz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.cheryme.top/gttjypnbmo.html

PHP:  // 手写递归函数
来源：http://hz.zhengqikj.top/gtukbnebbd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jqgufenzy.top/gtxslbnfev.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.haohaochexian.top/gtnmhgfzur.html

Java: // 手写递归
来源：http://hz.havefunace.top/gtawnwhcgc.html

Go:   // 手写递归
来源：http://hz.hfpthk.cn/gtstyncphm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.mhx1999.top/gtzrffkjjo.html

C#:   // 手写递归
来源：http://hz.316326.xyz/gtitqsnxng.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.jinqigufen.top/gtikfmfexb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.hnxiangtu.top/gtcgjgpczd.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.vqdsnc.cn/gtxjltughl.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hywenlv.cn/gtiuavzita.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cheryme.top/gtpkyerncc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.havefunace.top/gtrhjngqis.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.meibo888.top/gtqdhjrofr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.jqgfzy.top/gtoyqiwhbv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zycfv.cn/gtzzuhwaaa.html

================================================================================
来源：http://hz.xylfe.cn/gtxvachfiw.html

O. 并发与异步
来源：http://hz.hnxiangtu.top/gthxkjnnqy.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtsttsndur.html

[O01] 启动一个线程
来源：http://hz.wangdashe.top/gthrslsvvx.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.bjfxy.top/gtjeisguhx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.wangshuangyany.cn/gtmmxsjhgm.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.52xcode.cn/gtppbfmjsp.html

TS:   // 同 JS
来源：http://hz.gzhubu.top/gtrnbnlskl.html

Java: new Thread(() -> f()).start()
来源：http://hz.feifeiyinyue.top/gtvjjgoycs.html

Go:   go f()
来源：http://hz.shanyushiyangtech.top/gtqucitfiw.html

Ruby: Thread.new { f }
来源：http://hz.wangdashe.top/gtpivkbopx.html

C#:   Task.Run(() => F());
来源：http://hz.zdqjudy.top/gtgsmbrhyt.html

[O02] 使用线程池
来源：http://hz.jinyuanbaomall.cn/gtdqzvnyzw.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.xingfuxueyuan.xyz/gtyxlhcesi.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.sysykeji.top/gtthatoqco.html

JS:   // worker_threads 线程池
来源：http://hz.daxiang520.top/gtvxhlvevv.html

TS:   // worker_threads 线程池
来源：http://hz.shzxlz.cn/gtmitdtfpu.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.aizwys.cn/gtzfayqqky.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.chenzaomai.com/gtyusqwpje.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.gzhubu.top/gtwyocmojv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.shzxlz.cn/gtorhcszny.html

[O03] 加锁保护共享数据
来源：http://hz.dianchejie.cn/gtgoirekrm.html

Py:   with lock: shared += 1
来源：http://hz.jianghu66.top/gtvftdforc.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.kuanghao11.cn/gtlnwkvjqo.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.cdnleiting.top/gtwyceippu.html

TS:   // 同 JS
来源：http://hz.xingfuxueyuan.xyz/gtmiuanphb.html

Java: synchronized (this) { shared++; }
来源：http://hz.zhongyouzk.top/gtgttkcddd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yanxiufei.cn/gtmcdkitjy.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.hywenlv.cn/gtduhpmjws.html

C#:   lock (gate) { shared++; }
来源：http://hz.c1oappe.top/gtlitczjwq.html

[O04] 定义异步函数并等待
来源：http://hz.chenzaomai.com/gtqolglzey.html

Py:   async def f():⏎    await g()
来源：http://hz.52xcode.cn/gtbapujwjh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.nanxuanxn.top/gtfvzpjxtl.html

JS:   async function f() { await g(); }
来源：http://hz.xuetiantiany.cn/gtuwishdvd.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.tianlin.xyz/gtlrtluhit.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.tianlin.xyz/gtrcfqqrof.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.jinqigufen.top/gtbnlbnmfe.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.cdnleiting.top/gtmstckeix.html

C#:   async Task F() { await G(); }
来源：http://hz.tianlin.xyz/gtdxxpduum.html

[O05] 并发执行并等待全部完成
来源：http://hz.tianlin.xyz/gtmafaixhk.html

Py:   asyncio.gather(*tasks)
来源：http://hz.yonumen.top/gtyxekxtjk.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.hnxiangtu.top/gtmmcclfvl.html

JS:   await Promise.all(tasks)
来源：http://hz.fengsongda.top/gterajzeqf.html

TS:   await Promise.all(tasks)
来源：http://hz.gotoacloud.top/gtguolcoph.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.haohaochexian.top/gtmvvpkubp.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.gaohongyu789.top/gtjihiyojs.html

Ruby: threads.map(&:join)
来源：http://hz.zhongyouzk.top/gtuevlmhno.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.jqgufenzy.top/gtqjippgfj.html

[O06] 使用进程池
来源：http://hz.guowangkeji.top/gtzdouenpk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.xinyue.icu/gtrfiymzgg.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.birdmap.top/gtpordwsfc.html

JS:   // child_process / cluster 模块
来源：http://hz.dashuyun.cn/gtqcerexsd.html

TS:   // child_process / cluster 模块
来源：http://hz.kuanghao11.cn/gtssenjoij.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.zhiwuduotai.top/gtzhsjewih.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.9152youxi.cn/gtsqhbocxc.html

Ruby: // fork 块
来源：http://hz.sysykeji.top/gtppuyskiu.html

C#:   Parallel.For
来源：http://hz.jinyuanbaomall.cn/gthiksmicl.html

================================================================================
来源：http://hz.hysaishi.cn/gtlyjvxowc.html

P. 常用工具函数
来源：http://hz.hywenlv.cn/gtkzpppbdi.html

================================================================================
来源：http://hz.tanke756.top/gtnunbiwvg.html

[P01] 生成 UUID
来源：http://hz.guannengcc.top/gthqipdqwd.html

Py:   str(uuid.uuid4())
来源：http://hz.fzhhl.top/gtkzvbfudb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.9152youxi.cn/gtdcgzbzip.html

JS:   crypto.randomUUID()
来源：http://hz.zhoulong.xyz/gtmwzaqkxi.html

TS:   crypto.randomUUID()
来源：http://hz.yj20258.top/gtkcrcbklp.html

Java: UUID.randomUUID().toString()
来源：http://hz.nanxinkj.top/gtkqpoammf.html

Go:   // 用 github.com/google/uuid
来源：http://hz.cashguo.top/gtqhricmfc.html

Ruby: SecureRandom.uuid
来源：http://hz.xinyue.icu/gthneekrib.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.zhoulong.xyz/gtyqnjskrn.html

[P02] MD5 / SHA256 摘要
来源：http://hz.shzxlz.cn/gtkyeplvug.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.316326.xyz/gtxhwpjlic.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.aizwys.cn/gtzcakoyva.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.kuanghao11.cn/gtteqqdsdl.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.hfpthk.cn/gtsmutvfiz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.feifeiyinyue.top/gtepkuglff.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.sweek.top/gtpbwbzuel.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.zhengqikj.top/gtcxmyvgmx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.xinyue.icu/gtajzusznk.html

[P03] 生成短随机字符串
来源：http://hz.jinqigufen.top/gthmhtuyov.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.cheryme.top/gtjrilwhvd.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.wangdashe.top/gtaohwhdlb.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ybcxt.top/gtgdzrjeut.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hammf.cn/gtnfongind.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jianghu66.top/gtdwbldftc.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.cashguo.top/gteyimpkfy.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.hammf.cn/gtnhlualyd.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jyoumei.cn/gtaafpkodm.html

[P04] 求长度
来源：http://hz.gaohongyu789.top/gtsyxiiwhl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.jyoumei.cn/gtdeqnefog.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jinqigfzy.top/gtnzmctgad.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.cheryme.top/gtqwnmvslt.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.daxiang520.top/gtibpduidb.html

Java: list.size();  map.size();  s.length()
来源：http://hz.ehwqpu.com/gttasemnqs.html

Go:   len(arr);  len(m)
来源：http://hz.guowangkeji.top/gtvycwzrte.html

Ruby: x.length;  x.size
来源：http://hz.jinghuilouyu.cn/gtblmuwgpe.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.pycfn.com/gtjjjsdisd.html

[P05] 判断两个对象内容是否相等
来源：http://hz.c1oappe.top/gtgfbhkxxe.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.yuxming.cn/gtsabwxjxq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.shanyushiyangkeji.top/gtxohfrsxv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.sufxvd.cn/gtnbdwncmx.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.fengsongda.top/gtwyanukql.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.sxryk.cn/gtjsbrsjrx.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.dashuyun.cn/gtoyrzhldv.html

Ruby: a == b
来源：http://hz.chenjidiqi.icu/gtaztkqkop.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.gaohongyu789.top/gteunzhyil.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.chenjidiqi.icu/gthonphasw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.jyoumei.cn/gthsisnmdc.html

PHP:  if (empty($x)) {}
来源：http://hz.gzhubu.top/gtymvjnirs.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.andypj.xyz/gtrmzubsuv.html

TS:   if (x == null) {}
来源：http://hz.dianchejie.cn/gtxxfeuvvy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.c1oappe.top/gtvwtulohh.html

Go:   if x == nil {}
来源：http://hz.jinghuilouyu.cn/gtcatlhjso.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.cqqwz.cn/gtxpemgbjy.html

C#:   if (x is null) {}
来源：http://hz.0kj1m.cn/gtmshjyrjj.html

[P07] 防抖与节流
来源：http://hz.zycfv.cn/gtbkwluret.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.fzhhl.top/gtdpvxidnz.html

PHP:  // 手写时间戳比较
来源：http://hz.zycfv.cn/gteeoprpbp.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jqgufenzy.top/gtkbrjebxe.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.chenzaomai.com/gtlvhvrnwd.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.guannengcc.top/gtihxvxfth.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.gaohongyu789.top/gtjjnrwean.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.tanke756.top/gtdpfdejar.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.chenlongwang.top/gtiictekgj.html

[P08] 处理浮点精度问题
来源：http://hz.dianchejie.cn/gtmdtdonig.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.xziqi.cn/gtletwafuk.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.xylfe.cn/gtqjmzxqmh.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.tianlin.xyz/gtxijnfiwl.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.vqdsnc.cn/gttkvmrejr.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.zhengqikj.top/gtexacesec.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.gaohongyu789.top/gthuuapnrv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.sysykeji.top/gtljhegwwb.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.dianchejie.cn/gtjchrdghr.html

================================================================================
来源：http://hz.guowangkeji.top/gthlvahpwi.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.haohaochexian.top/gtihygejew.html

================================================================================
来源：http://hz.sweek.top/gtyycfjyeh.html

[Q01] 创建表
来源：http://hz.wangshuangyany.cn/gtptkvqshp.html

CREATE TABLE users (
来源：http://hz.cucudq.cn/gtwkqmbark.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhengqikj.top/gtgarpkvze.html

name VARCHAR(50) NOT NULL,
来源：http://hz.ppjwa.cn/gtyefornwj.html

email VARCHAR(100) UNIQUE,
来源：http://hz.cdnleiting.top/gtohupsehm.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.hfpthk.cn/gtxrckppks.html

);
来源：http://hz.ydzc1.top/gtffveogiq.html

[Q02] 创建带外键的表
来源：http://hz.redwolf501.top/gtdntjgejl.html

CREATE TABLE orders (
来源：http://hz.hammf.cn/gtugilqdfl.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xziqi.cn/gtkpdltoea.html

user_id INT NOT NULL,
来源：http://hz.zhiwuduotai.top/gtbhonlugk.html

amount DECIMAL(10, 2),
来源：http://hz.zhoulong.xyz/gttxmcunlw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.gotoacloud.top/gtdykmbaqa.html

);
来源：http://hz.tian-w.cn/gtsckkhiqq.html

[Q03] 增加列
来源：http://hz.yuanzhike.top/gtogiurbir.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.yonumen.top/gtgqnzzsbm.html

[Q04] 修改列类型
来源：http://hz.quarkkingdee.top/gtdyekxnmr.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.xuetiantiany.cn/gthxsujush.html

[Q05] 重命名列
来源：http://hz.pycfn.com/gtlbnvmdxe.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.yongpay.top/gtrlzuonlz.html

[Q06] 删除列
来源：http://hz.svipenyu.cn/gtqifuysdn.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.zhiwuduotai.top/gtgzeidrsc.html

[Q07] 删除表
来源：http://hz.feifeiyinyue.top/gtafqsgtlu.html

DROP TABLE IF EXISTS orders;
来源：http://hz.yangfankeji.com/gthpvsgtmc.html

[Q08] 创建普通索引
来源：http://hz.chenlongwang.top/gtpfwnqato.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.wangshuangyany.cn/gtfvkodpnb.html

[Q09] 创建唯一索引
来源：http://hz.fzhhl.top/gtpdobcdrc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.zycfv.cn/gtnxnmejsz.html

[Q10] 插入单行
来源：http://hz.guowangkeji.top/gtaaiaufko.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jinghuilouyu.cn/gtqrswfarg.html

[Q11] 一次插入多行
来源：http://hz.hysaishi.cn/gtpzymgtdw.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.birdmap.top/gtgtekzclf.html

[Q12] 插入后取自增 ID
来源：http://hz.jlsjyb.cn/gtxlfwytbe.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.dashuyun.cn/gtchnsabop.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.zycfv.cn/gtbxchbcat.html

[Q13] 忽略重复插入
来源：http://hz.ywan-chungtsiang.top/gtuxyanffw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.gaohongyu789.top/gtjzjxxbgt.html

[Q14] 存在则更新（upsert）
来源：http://hz.birdmap.top/gtpbiwudyx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.tanke756.top/gtebtegjjq.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.hammf.cn/gtdrftcscm.html

[Q15] 查询全部
来源：http://hz.chenzaomai.com/gtxdkblhwr.html

SELECT * FROM users;
来源：http://hz.sxryk.cn/gtkwnvmjtf.html

[Q16] 查询指定列
来源：http://hz.zycfv.cn/gtnmodktwj.html

SELECT id, name FROM users;
来源：http://hz.zhongyouzk.top/gtfvwbqxku.html

[Q17] 条件查询
来源：http://hz.tian-w.cn/gtnjreielq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.svipenyu.cn/gthdzfqafx.html

[Q18] 模糊匹配
来源：http://hz.shanyushiyangkeji.top/gtlrfextql.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yangfankeji.com/gtupuithkg.html

[Q19] 范围查询
来源：http://hz.guannengcc.top/gtvveyfsut.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.cdnleiting.top/gtynisvdsn.html

[Q20] IN 列表
来源：http://hz.zhongyouzk.top/gtsosngwnm.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.nanxinkj.top/gtmepoogyj.html

[Q21] 空值判断
来源：http://hz.pengpengdd.cyou/gtogvoqybm.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.yj20258888.top/gtqjfdvkxn.html

[Q22] 排序
来源：http://hz.tian-w.cn/gteakhgdsx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.vqdsnc.cn/gtpzmkvlxt.html

[Q23] 分页
来源：http://hz.zdqjudy.top/gthmvoirnu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yuxming.cn/gtphlksymx.html

[Q24] 去重
来源：http://hz.hammf.cn/gtzhsteggs.html

SELECT DISTINCT city FROM users;
来源：http://hz.9152youxi.cn/gtffppqlsu.html

[Q25] 只取前 N 条
来源：http://hz.jyoumei.cn/gtbdvbouto.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.jinqigfzy.top/gtmhjjakod.html

[Q26] 计数
来源：http://hz.fengsongda.top/gtquannwzm.html

SELECT COUNT(*) FROM users;
来源：http://hz.ppjwa.cn/gtiugehlyl.html

[Q27] 条件计数
来源：http://hz.shangyingyoupin.top/gtjyajeneo.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.pycfn.com/gtlymqsbru.html

[Q28] 求和与平均
来源：http://hz.ivvv.top/gtihwvtafs.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.meibo888.top/gtkdyzjnfq.html

[Q29] 最大最小值
来源：http://hz.gaohongyu789.top/gtxptclnel.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.feifeiyinyue.top/gtftljnxmk.html

[Q30] 分组统计
来源：http://hz.chenjidiqi.icu/gtsalxdwqf.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.hywenlv.cn/gtfymeloty.html

[Q31] 分组后过滤
来源：http://hz.sysykeji.top/gtopcxxeab.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.birdmap.top/gthkgupzdi.html

[Q32] 分组拼接字符串
来源：http://hz.ydzc1.top/gtuckrbjnq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.yuxming.cn/gtlfqaigcd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.jinyuanbaomall.cn/gtzkxljwrh.html

[Q33] 多列分组
来源：http://hz.xuetiantiany.cn/gtejjxwmed.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.xuetiantiany.cn/gtiyhvqfep.html

[Q34] 每组取第一条
来源：http://hz.yj20258.top/gtijoqebdn.html

SELECT * FROM (
来源：http://hz.havefunace.top/gtqhqnwmcz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.xuetiantiany.cn/gtumbhefig.html

) t WHERE rn = 1;
来源：http://hz.chenzaomai.com/gtrxhiqrao.html

[Q35] 内连接
来源：http://hz.pengpengdd.cyou/gtaymbllll.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.sweek.top/gtmcpwpxcv.html

[Q36] 左连接
来源：http://hz.feifeiyinyue.top/gtkxljpchy.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.jinghuilouyu.cn/gttdwyuyst.html

[Q37] 右连接
来源：http://hz.9152youxi.cn/gtdspsshss.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.yj202588.top/gtcnpisgwx.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.sxryk.cn/gttzgrkoui.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.zhongyouzk.top/gtamxuyxcq.html

[Q39] 自连接（查上下级）
来源：http://hz.xziqi.cn/gtbeedqdwd.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.yj202588.top/gtwwresyqb.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.zhijiandao.cn/gttmjnhmzu.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.guannengcc.top/gtvzprkxog.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.haohaochexian.top/gttxzxjmni.html

[Q41] 多表连接
来源：http://hz.birdmap.top/gtgyhhpstz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.gaohongyu789.top/gthjkdjcms.html

JOIN users u ON u.id = o.user_id
来源：http://hz.fengsongda.top/gtsgjdlpon.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.zhongyouzk.top/gtlrofkrek.html

[Q42] 连接条件附加过滤
来源：http://hz.cheryme.top/gtdxtsbzvd.html

SELECT u.name, o.amount FROM users u
来源：http://hz.dashuyun.cn/gtiygpyqap.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.fengsongda.top/gtykybfohx.html

[Q43] 标量子查询
来源：http://hz.feifeiyinyue.top/gtyymlxicl.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.dianchejie.cn/gtwcvynphv.html

[Q44] IN 子查询
来源：http://hz.shanyushiyangkeji.top/gtoojdkpsa.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.redwolf501.top/gtndwxddzy.html

[Q45] EXISTS 判断存在
来源：http://hz.vqdsnc.cn/gtwwbwrkyp.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.sxryk.cn/gtamhpofnd.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yueranfly.top/gtfizuaocr.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.shanyushiyangtech.top/gtpoegpnfk.html

[Q47] 与平均值比较
来源：http://hz.cheryme.top/gtyweqxwoj.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.guowangkeji.top/gtrrjrtvdc.html

[Q48] CTE 公用表表达式
来源：http://hz.daxiang520.top/gthjncdkjx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.zhongyouzk.top/gtsvybvehj.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.ywan-chungtsiang.top/gtznsopzrd.html

[Q49] 更新单行
来源：http://hz.jinyuanbaomall.cn/gtwrfdorqx.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.gzhubu.top/gtjbtmgefq.html

[Q50] 批量更新
来源：http://hz.aizwys.cn/gtaqkrtqhn.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.sysykeji.top/gtduojyyet.html

[Q51] 用子查询更新
来源：http://hz.tian-w.cn/gtxmnpxxvh.html


<!-- 参考信息 -->