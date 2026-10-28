代发 wailian999

[N09] 栈与队列
来源：http://hz.yj20258888.top/gtcjogtdgi.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.smart0.xyz/gtzljugoxf.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.fengsongda.top/gtxhbgohfs.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yj202588.top/gtnmxsroem.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.ehwqpu.com/gtsjlnvefu.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.gzhubu.top/gtxefimrxo.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.cucudq.cn/gtujqbewfl.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.fzhhl.top/gtvgltiazh.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.jinqigfzy.top/gtzrbmrgul.html

[N10] 链表节点定义
来源：http://hz.jianghu66.top/gtclrsophk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.xylfe.cn/gtxophoorl.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.daxiang520.top/gtkvdwdrez.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.cucudq.cn/gtxoxbxyll.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.dianchejie.cn/gtrucoirjl.html

Java: class Node { int v; Node next; }
来源：http://hz.yj20258888.top/gtklgmgepn.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.ydjk.org.cn/gtjsscbsdd.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.aibaodan.cn/gtcdmgblys.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.wangdashe.top/gtajhklnaj.html

[N11] 二叉树中序遍历
来源：http://hz.sufxvd.cn/gtbjebywxz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.ivvv.top/gtoyqhetim.html

PHP:  // 手写递归函数
来源：http://hz.zhijiandao.cn/gtludhwxdv.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.52xcode.cn/gtjubkikhx.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.c1oappe.top/gtstblghpj.html

Java: // 手写递归
来源：http://hz.iojbl.cn/gttsnziegv.html

Go:   // 手写递归
来源：http://hz.xingfuxueyuan.xyz/gtseyeavyw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.cqqwz.cn/gtcqcjgene.html

C#:   // 手写递归
来源：http://hz.cashguo.top/gtubpxjiwe.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.xuetiantiany.cn/gtwkzydbsr.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.xuetiantiany.cn/gtvgzrgoxq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.wangshuangyany.cn/gtpiedggxu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.gaohongyu789.top/gtclbwpwpz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.shzxlz.cn/gtggddpegu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.cdnleiting.top/gtglimltyd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.sweek.top/gtnjyxyxqv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.jqgfzy.top/gtxcuxexpj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.dashuyun.cn/gtblaftskz.html

================================================================================
来源：http://hz.chenlongwang.top/gtknhekbel.html

O. 并发与异步
来源：http://hz.ywan-chungtsiang.top/gttcoaapqm.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtmdhsbttp.html

[O01] 启动一个线程
来源：http://hz.yj20258.top/gtvpemesig.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.guannengcc.top/gtvcwgmqgh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.nanxuanxn.top/gtobiopsdf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.shanyushiyangkeji.top/gtjnqteihh.html

TS:   // 同 JS
来源：http://hz.tanke756.top/gtfppcepup.html

Java: new Thread(() -> f()).start()
来源：http://hz.wangshuangyany.cn/gturkvhzpm.html

Go:   go f()
来源：http://hz.hammf.cn/gtvmhtbldi.html

Ruby: Thread.new { f }
来源：http://hz.tanke756.top/gtoqqfoyyj.html

C#:   Task.Run(() => F());
来源：http://hz.shzxlz.cn/gtaruwtwlt.html

[O02] 使用线程池
来源：http://hz.yuxming.cn/gttpghrzqh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.bjfxy.top/gtepqntxxb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.chenlongwang.top/gtmnelxtev.html

JS:   // worker_threads 线程池
来源：http://hz.xuanzx.com/gtxhlqfhce.html

TS:   // worker_threads 线程池
来源：http://hz.pengpengdd.cyou/gtpgmrtnlm.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.jqgufenzy.top/gtumhnzegb.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.zhaomingkeji.xyz/gtvtuvrubg.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.ydjk.org.cn/gtuesqbepd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.9152youxi.cn/gtezpvwjkx.html

[O03] 加锁保护共享数据
来源：http://hz.gogol.net.cn/gtknjlrhcb.html

Py:   with lock: shared += 1
来源：http://hz.vqdsnc.cn/gtcenwmlnv.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.daxiang520.top/gtlrhcnlcv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.jqgfzy.top/gtgbdigduz.html

TS:   // 同 JS
来源：http://hz.cqqwz.cn/gtfwttocfo.html

Java: synchronized (this) { shared++; }
来源：http://hz.jinqigufen.top/gtbabkomba.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.zhijiandao.cn/gtdnggjukd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.xuetiantiany.cn/gtgdbhddwn.html

C#:   lock (gate) { shared++; }
来源：http://hz.yangfankeji.com/gtnmxuwjfl.html

[O04] 定义异步函数并等待
来源：http://hz.bjfxy.top/gtxuwxatyu.html

Py:   async def f():⏎    await g()
来源：http://hz.svipenyu.cn/gtncihimhi.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.nanxinkj.top/gtgsraewli.html

JS:   async function f() { await g(); }
来源：http://hz.sysykeji.top/gtdbuhnbyr.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.316326.xyz/gtjmkntryt.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.jinqigufen.top/gttoumzriz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.yongpay.top/gtwqyhgduu.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.ydzc1.top/gtgtksvtfa.html

C#:   async Task F() { await G(); }
来源：http://hz.zhixingplan.top/gtgbcypams.html

[O05] 并发执行并等待全部完成
来源：http://hz.guowangkeji.top/gthrtwoglm.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jqgfzy.top/gtxsgftkvc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.ydzc1.top/gtszacwoag.html

JS:   await Promise.all(tasks)
来源：http://hz.jinqigufen.top/gtqujaiocp.html

TS:   await Promise.all(tasks)
来源：http://hz.chenjidiqi.icu/gtuhbxdkky.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.havefunace.top/gtzrpcakrq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.chenlongwang.top/gtqcrjwpcl.html

Ruby: threads.map(&:join)
来源：http://hz.yangfankeji.com/gtmriluhwi.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.zdqjudy.top/gtyjqtnegv.html

[O06] 使用进程池
来源：http://hz.yanxiufei.cn/gtyhovijwg.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.jqgufenzy.top/gtpwavoruu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.jlsjyb.cn/gtsszwlzta.html

JS:   // child_process / cluster 模块
来源：http://hz.hnxiangtu.top/gtdhhpqyxj.html

TS:   // child_process / cluster 模块
来源：http://hz.yvedp.cn/gtvayzojuq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.hnxiangtu.top/gtkzdsgtuq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.yuxming.cn/gtjoytkuhd.html

Ruby: // fork 块
来源：http://hz.yj20258.top/gtlmswyfji.html

C#:   Parallel.For
来源：http://hz.shanyushiyangtech.top/gtxftwwbha.html

================================================================================
来源：http://hz.yvedp.cn/gthejmukdo.html

P. 常用工具函数
来源：http://hz.hammf.cn/gtyygwtadj.html

================================================================================
来源：http://hz.guannengcc.top/gtgoegwpif.html

[P01] 生成 UUID
来源：http://hz.gaohongyu789.top/gtpkmwluuv.html

Py:   str(uuid.uuid4())
来源：http://hz.nanxuanxn.top/gtwtfggeke.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jinyuanbaomall.cn/gtnawyewyp.html

JS:   crypto.randomUUID()
来源：http://hz.xinyue.icu/gtluufkilt.html

TS:   crypto.randomUUID()
来源：http://hz.pycfn.com/gtfdfnimeg.html

Java: UUID.randomUUID().toString()
来源：http://hz.jinqigufen.top/gtdgbjfysj.html

Go:   // 用 github.com/google/uuid
来源：http://hz.zhoulong.xyz/gtdkweaoav.html

Ruby: SecureRandom.uuid
来源：http://hz.chenlongwang.top/gtgqgaqldb.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.guowangkeji.top/gthrepewso.html

[P02] MD5 / SHA256 摘要
来源：http://hz.chenlongwang.top/gtykncadvr.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.yongpay.top/gtdvxueccq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.yj20258.top/gtzqtxasre.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.jinqigfzy.top/gtkshdhzto.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.zhixingplan.top/gtkkrtyckq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.aibaodan.cn/gtfkuddkug.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.316326.xyz/gtaoverzxr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.hfpthk.cn/gtbcofjmkd.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.ydjk.org.cn/gtbcibetuc.html

[P03] 生成短随机字符串
来源：http://hz.gzhubu.top/gtiqjepjju.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.yuanzhike.top/gtvppibcxr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.nanxuanxn.top/gttpntjjfs.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.kuanghao11.cn/gtsroszakb.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zycfv.cn/gtuvewbvvq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.gotoacloud.top/gtrgvxznjs.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yuanzhike.top/gtgxaleysh.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jiagoushi.top/gtqevvwnus.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.daria6918.cn/gtdbollwzg.html

[P04] 求长度
来源：http://hz.tianlin.xyz/gtpkrzejpq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.sweek.top/gtlgjfxvli.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.daxiang520.top/gtriwahtiv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.redwolf501.top/gthcxvdexq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.gaohongyu789.top/gtrokhzjlj.html

Java: list.size();  map.size();  s.length()
来源：http://hz.hammf.cn/gtmpbntgez.html

Go:   len(arr);  len(m)
来源：http://hz.gogol.net.cn/gtbarfelsv.html

Ruby: x.length;  x.size
来源：http://hz.yueranfly.top/gtwoizurmw.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.zycfv.cn/gtuvltuobn.html

[P05] 判断两个对象内容是否相等
来源：http://hz.zhiwuduotai.top/gtjnzavqrb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.dashuyun.cn/gtnimhxuqp.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.cdnleiting.top/gtisrxcmfo.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.xziqi.cn/gtgkgbqecs.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.c1oappe.top/gtezgxrujx.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.ydjk.org.cn/gtqqwrdynr.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.ybcxt.top/gtrcjgbocl.html

Ruby: a == b
来源：http://hz.chenzaomai.com/gtcfhbehxb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.cucudq.cn/gtkycrzrlr.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.sxryk.cn/gtjsupgxll.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.0kj1m.cn/gtgupzpklf.html

PHP:  if (empty($x)) {}
来源：http://hz.hysaishi.cn/gtowuppbqg.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.redwolf501.top/gtiycryeod.html

TS:   if (x == null) {}
来源：http://hz.meibo888.top/gtkphyrzzh.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.jiagoushi.top/gtfbbrmanj.html

Go:   if x == nil {}
来源：http://hz.jiagoushi.top/gtmfmviqey.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jqgfzy.top/gtzvsobxvg.html

C#:   if (x is null) {}
来源：http://hz.hongshengwenyu.top/gtalhlzxjr.html

[P07] 防抖与节流
来源：http://hz.yj20258.top/gthrgqgpuo.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.iojbl.cn/gtrxdaaqgo.html

PHP:  // 手写时间戳比较
来源：http://hz.guowangkeji.top/gtomvrcfep.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shzxlz.cn/gtzcwdybtx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ehwqpu.com/gtwoomxwme.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.ehwqpu.com/gtzadsomtk.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.birdmap.top/gtsgbiwkld.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.guowangkeji.top/gthgdpsrqd.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.cheryme.top/gtllrqynjr.html

[P08] 处理浮点精度问题
来源：http://hz.zhiwuduotai.top/gtjvqiuurp.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.haohaochexian.top/gtbmtvppeu.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.gzhubu.top/gtbehilinp.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.sysykeji.top/gtapzmdgqq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.yuxming.cn/gtvozhyklf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.cqqwz.cn/gturuddgvn.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.redwolf501.top/gtmeidvvdb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.feifeiyinyue.top/gtgeuuygzq.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.jqgufenzy.top/gtvfszrhvf.html

================================================================================
来源：http://hz.shuidangran.top/gtrcxxpfrp.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.ydzc1.top/gtwfjquqaf.html

================================================================================
来源：http://hz.jqgufenzy.top/gtyqaqhbxi.html

[Q01] 创建表
来源：http://hz.ivvv.top/gtormhpqpj.html

CREATE TABLE users (
来源：http://hz.jinqigufen.top/gtfhsldqxa.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jinqigufen.top/gtmuafebdh.html

name VARCHAR(50) NOT NULL,
来源：http://hz.cdnleiting.top/gtuxcvvljs.html

email VARCHAR(100) UNIQUE,
来源：http://hz.xuanzx.com/gtccbwcffv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.jqgufenzy.top/gtyybinagq.html

);
来源：http://hz.316326.xyz/gtniknsksj.html

[Q02] 创建带外键的表
来源：http://hz.dashuyun.cn/gtbfeerynf.html

CREATE TABLE orders (
来源：http://hz.mhx1999.top/gtexyeynhb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.chenzaomai.com/gtpzkygmfj.html

user_id INT NOT NULL,
来源：http://hz.chenzaomai.com/gtcpmpfjpc.html

amount DECIMAL(10, 2),
来源：http://hz.wangshuangyany.cn/gtbiuhhetl.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.c1oappe.top/gtsfluijjf.html

);
来源：http://hz.guannengcc.top/gtddtctkbn.html

[Q03] 增加列
来源：http://hz.hammf.cn/gtdqqnyaub.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.jinqigufen.top/gtuiltgycg.html

[Q04] 修改列类型
来源：http://hz.zhoulong.xyz/gtrgvumvey.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.cdnleiting.top/gtcunrembw.html

[Q05] 重命名列
来源：http://hz.nwbrower.top/gtylpjjwho.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.yangfankeji.com/gtuavkuqai.html

[Q06] 删除列
来源：http://hz.meibo888.top/gtplttwtmf.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.zycfv.cn/gthzvuadgi.html

[Q07] 删除表
来源：http://hz.quarkkingdee.top/gtleuteeiu.html

DROP TABLE IF EXISTS orders;
来源：http://hz.ywan-chungtsiang.top/gtcwlehheg.html

[Q08] 创建普通索引
来源：http://hz.aizwys.cn/gtxuubdsyv.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.yanxiufei.cn/gtkcfsurzl.html

[Q09] 创建唯一索引
来源：http://hz.hywenlv.cn/gtbuchrnpm.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.yj20258888.top/gtiachkxmk.html

[Q10] 插入单行
来源：http://hz.cdnleiting.top/gtdiabnwwl.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.tianlin.xyz/gtepwttmkb.html

[Q11] 一次插入多行
来源：http://hz.yonumen.top/gtsiplsuet.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yueranfly.top/gtmxksdwbd.html

[Q12] 插入后取自增 ID
来源：http://hz.yuxming.cn/gtbdvblesu.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.aibaodan.cn/gttzwljbyt.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.316326.xyz/gtxuzvwxrq.html

[Q13] 忽略重复插入
来源：http://hz.fzhhl.top/gtkgjixwsz.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.ppjwa.cn/gtzoywgjjn.html

[Q14] 存在则更新（upsert）
来源：http://hz.zdqjudy.top/gtvxedkdtf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.cdnleiting.top/gtobhmdcxw.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.yj202588.top/gtbbqsnead.html

[Q15] 查询全部
来源：http://hz.c1oappe.top/gtadjdpblc.html

SELECT * FROM users;
来源：http://hz.hywenlv.cn/gtwlpbzcno.html

[Q16] 查询指定列
来源：http://hz.jinyuanbaomall.cn/gtjjegbekn.html

SELECT id, name FROM users;
来源：http://hz.shzxlz.cn/gtndkzakfn.html

[Q17] 条件查询
来源：http://hz.sxryk.cn/gthpdckmbs.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.zhongyouzk.top/gtwbqldvfx.html

[Q18] 模糊匹配
来源：http://hz.gaohongyu789.top/gtlirbedds.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.svipenyu.cn/gtpnkqkfju.html

[Q19] 范围查询
来源：http://hz.guannengcc.top/gtwhbqbzmz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.snrcjt.cn/gtmowjogdj.html

[Q20] IN 列表
来源：http://hz.tianlin.xyz/gttfcvfrqk.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.ywan-chungtsiang.top/gtjdzhucuk.html

[Q21] 空值判断
来源：http://hz.mhx1999.top/gtsrfsobkm.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.havefunace.top/gtxujupbid.html

[Q22] 排序
来源：http://hz.zhixingplan.top/gtjlrncdgb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.shuidangran.top/gtvikfcthe.html

[Q23] 分页
来源：http://hz.pengpengdd.cyou/gtnzfqdktw.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.ywan-chungtsiang.top/gtksjkjtof.html

[Q24] 去重
来源：http://hz.havefunace.top/gtnaeoodis.html

SELECT DISTINCT city FROM users;
来源：http://hz.aibaodan.cn/gtooadnjpm.html

[Q25] 只取前 N 条
来源：http://hz.zhijiandao.cn/gtgmwufzpb.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.xuanzx.com/gtmqhovnqc.html

[Q26] 计数
来源：http://hz.ivvv.top/gtsjkdukkp.html

SELECT COUNT(*) FROM users;
来源：http://hz.hywenlv.cn/gtztcoksqh.html

[Q27] 条件计数
来源：http://hz.wangdashe.top/gtdvyfdbol.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.tanke756.top/gttnoyiysw.html

[Q28] 求和与平均
来源：http://hz.gaohongyu789.top/gthurjdqak.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.yuanzhike.top/gtpbhksshr.html

[Q29] 最大最小值
来源：http://hz.yanxiufei.cn/gtzsssvyur.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.tian-w.cn/gtkhysjsyf.html

[Q30] 分组统计
来源：http://hz.smart0.xyz/gtglqfyueu.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.shangyingyoupin.top/gtpblwlwrv.html

[Q31] 分组后过滤
来源：http://hz.ehwqpu.com/gtxvgehbsm.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.jyoumei.cn/gtzfkajvma.html

[Q32] 分组拼接字符串
来源：http://hz.jinyuanbaomall.cn/gtwsdmxyci.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.52xcode.cn/gtqukudihb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.dianchejie.cn/gtijzbqrzx.html

[Q33] 多列分组
来源：http://hz.snrcjt.cn/gtebheprjg.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.redwolf501.top/gtsfqboadi.html

[Q34] 每组取第一条
来源：http://hz.0kj1m.cn/gtndrqajto.html

SELECT * FROM (
来源：http://hz.zhixingplan.top/gtetxriwby.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.tian-w.cn/gtwkhcbxjv.html

) t WHERE rn = 1;
来源：http://hz.hnxiangtu.top/gtkpsxxuni.html

[Q35] 内连接
来源：http://hz.ehwqpu.com/gtblvsyivf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.hnqzz.top/gtqdbpaypg.html

[Q36] 左连接
来源：http://hz.dianchejie.cn/gtilycdfze.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.wangshuangyany.cn/gtmzojyrxp.html

[Q37] 右连接
来源：http://hz.wangshuangyany.cn/gtlysqjirb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.yj202588.top/gtqvzcjdtr.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.fengsongda.top/gtqappshuh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.chenzaomai.com/gttfoqzecm.html

[Q39] 自连接（查上下级）
来源：http://hz.chenzaomai.com/gthewnirjj.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.dianchejie.cn/gtgotwkekr.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yueranfly.top/gtrgmdvvxq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.shanyushiyangkeji.top/gterbhtfhy.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.pengpengdd.cyou/gtvfcixysx.html

[Q41] 多表连接
来源：http://hz.guannengcc.top/gtojcusqwt.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.yanxiufei.cn/gtyzntkalk.html

JOIN users u ON u.id = o.user_id
来源：http://hz.feifeiyinyue.top/gtrgwbeixx.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.daria6918.cn/gtieuwplbw.html

[Q42] 连接条件附加过滤
来源：http://hz.nanxuanxn.top/gtghyivdzv.html

SELECT u.name, o.amount FROM users u
来源：http://hz.ppjwa.cn/gthremrwmz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.dianchejie.cn/gtaspoeulv.html

[Q43] 标量子查询
来源：http://hz.dashuyun.cn/gtydsjxybb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.hfpthk.cn/gtrdzusxxw.html

[Q44] IN 子查询
来源：http://hz.gaohongyu789.top/gtktpuujxs.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.c1oappe.top/gtgeuapdwp.html

[Q45] EXISTS 判断存在
来源：http://hz.jinghuilouyu.cn/gtwhrkpxak.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhongyouzk.top/gtgimzschj.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.shuidangran.top/gtnocybhmd.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jyoumei.cn/gtfeunosnr.html

[Q47] 与平均值比较
来源：http://hz.guowangkeji.top/gtbuhuxips.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.chenlongwang.top/gtdvbqkxrt.html

[Q48] CTE 公用表表达式
来源：http://hz.hysaishi.cn/gtkjpicxhq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.ppjwa.cn/gtomwdjlbj.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.ybcxt.top/gtmnjfaotx.html

[Q49] 更新单行
来源：http://hz.dashuyun.cn/gtrxayzyjl.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.cashguo.top/gtqhmycfoe.html

[Q50] 批量更新
来源：http://hz.svipenyu.cn/gtpqttqjst.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.c1oappe.top/gtxkwjqxki.html

[Q51] 用子查询更新
来源：http://hz.yuanzhike.top/gtcuiksyux.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.fengsongda.top/gtgmlnskux.html

[Q52] 删除指定行
来源：http://hz.haohaochexian.top/gtyxmzcyqr.html

DELETE FROM users WHERE id = 10;
来源：http://hz.jinghuilouyu.cn/gtnimxmknw.html

[Q53] 按条件删除
来源：http://hz.xylfe.cn/gtgyxqscav.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.xuanzx.com/gtbwjcriwf.html

[Q54] 清空表
来源：http://hz.ehwqpu.com/gtjsutpbhi.html

TRUNCATE TABLE logs;
来源：http://hz.wangshuangyany.cn/gtkdwentel.html

[Q55] 排名（并列占位）
来源：http://hz.yuanzhike.top/gtlvrfgrco.html


<!-- 参考信息 -->