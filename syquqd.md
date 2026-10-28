代发 wailian999

[N09] 栈与队列
来源：http://hz.dianchejie.cn/gtatdkttzt.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.jinqigfzy.top/gthvmhurip.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.zhixingplan.top/gtfrtvlefi.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.gzhubu.top/gtxtklayqd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.cashguo.top/gtciykipfr.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.xingfuxueyuan.xyz/gtrtgjuptt.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.fzhhl.top/gtlvdjctdh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.mhx1999.top/gtgrkmoexr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.fengsongda.top/gtvgxxkwfu.html

[N10] 链表节点定义
来源：http://hz.kuanghao11.cn/gttuencfag.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.gaohongyu789.top/gtutxaasqb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.52xcode.cn/gtinckdxrw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.cdnleiting.top/gthquhwpcn.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.shuidangran.top/gtbocdcmmz.html

Java: class Node { int v; Node next; }
来源：http://hz.nwbrower.top/gtsehqgfat.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.daria6918.cn/gtnnunskqv.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.pycfn.com/gtgjrjdtfs.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.hammf.cn/gtndmcdonz.html

[N11] 二叉树中序遍历
来源：http://hz.shanyushiyangtech.top/gtjcuetxrr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.dianchejie.cn/gtwfmuhdwp.html

PHP:  // 手写递归函数
来源：http://hz.pycfn.com/gtuiaavtqf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.cucudq.cn/gtuejcnifq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ivvv.top/gtzggndjzh.html

Java: // 手写递归
来源：http://hz.chenzaomai.com/gtnprhqirk.html

Go:   // 手写递归
来源：http://hz.zhijiandao.cn/gtdkcmydhn.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.tian-w.cn/gtdxrkurgz.html

C#:   // 手写递归
来源：http://hz.pengpengdd.cyou/gteapbqion.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.zdqjudy.top/gtorpuiecg.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.tianlin.xyz/gtrmfamlkg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.svipenyu.cn/gtztrnnser.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.gotoacloud.top/gtuyzwkexs.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.haohaochexian.top/gttqlxdadv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.gzhubu.top/gthfiyqnzc.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.cqqwz.cn/gtitjvhwft.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.xziqi.cn/gtmpyrgxjm.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ivvv.top/gtiorfvgvw.html

================================================================================
来源：http://hz.jinqigufen.top/gtpajqtkid.html

O. 并发与异步
来源：http://hz.xingfuxueyuan.xyz/gtqxmnkcah.html

================================================================================
来源：http://hz.redwolf501.top/gtvhshmoed.html

[O01] 启动一个线程
来源：http://hz.svipenyu.cn/gttetaugaq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.xinyue.icu/gtmpexlxlx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.hfpthk.cn/gtsekfmqtq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.smart0.xyz/gttgsbhgjx.html

TS:   // 同 JS
来源：http://hz.guannengcc.top/gthgonvnrv.html

Java: new Thread(() -> f()).start()
来源：http://hz.shanyushiyangkeji.top/gtmszxtkgq.html

Go:   go f()
来源：http://hz.316326.xyz/gtvzbmxcgc.html

Ruby: Thread.new { f }
来源：http://hz.jqgufenzy.top/gtpfanmkln.html

C#:   Task.Run(() => F());
来源：http://hz.hammf.cn/gthxjsngiy.html

[O02] 使用线程池
来源：http://hz.haohaochexian.top/gtuqreipjk.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.hywenlv.cn/gtjvbpecft.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.nanxinkj.top/gtickmciux.html

JS:   // worker_threads 线程池
来源：http://hz.tanke756.top/gtspdkoowj.html

TS:   // worker_threads 线程池
来源：http://hz.yj20258.top/gtyivcdbcy.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.xylfe.cn/gtxzwkcwwo.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.jinghuilouyu.cn/gtmsmqvnvy.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.jinghuilouyu.cn/gtclruneuh.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.fengsongda.top/gtlsahbkyr.html

[O03] 加锁保护共享数据
来源：http://hz.zhiwuduotai.top/gtglczzuis.html

Py:   with lock: shared += 1
来源：http://hz.vqdsnc.cn/gtjiqojhtu.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.sxryk.cn/gttoafjrnx.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.gotoacloud.top/gtgheezxsn.html

TS:   // 同 JS
来源：http://hz.bjfxy.top/gtpnagmdne.html

Java: synchronized (this) { shared++; }
来源：http://hz.ybcxt.top/gtatdpcrcy.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.hongshengwenyu.top/gthfakfkzk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.daxiang520.top/gtbdbokqfs.html

C#:   lock (gate) { shared++; }
来源：http://hz.aibaodan.cn/gtjlqfzqqv.html

[O04] 定义异步函数并等待
来源：http://hz.yonumen.top/gthytfaljl.html

Py:   async def f():⏎    await g()
来源：http://hz.gzhubu.top/gttsfpokbd.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.hnxiangtu.top/gtpthbsfzd.html

JS:   async function f() { await g(); }
来源：http://hz.pengpengdd.cyou/gtnsydrhju.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.daria6918.cn/gtxlvwhyxk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.ydzc1.top/gtqmfrufmg.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.nwbrower.top/gtpsxiiunu.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.birdmap.top/gtijjpskmz.html

C#:   async Task F() { await G(); }
来源：http://hz.hfpthk.cn/gtmpwuvcwa.html

[O05] 并发执行并等待全部完成
来源：http://hz.guowangkeji.top/gtyvvzscia.html

Py:   asyncio.gather(*tasks)
来源：http://hz.fengsongda.top/gtgevrnqjq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.iojbl.cn/gtpamcggsr.html

JS:   await Promise.all(tasks)
来源：http://hz.yuanzhike.top/gtrytilobr.html

TS:   await Promise.all(tasks)
来源：http://hz.guowangkeji.top/gtyeeaejyg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.hfpthk.cn/gtxvktalyn.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.zhaomingkeji.xyz/gtvydmufnu.html

Ruby: threads.map(&:join)
来源：http://hz.yangfankeji.com/gtoagpqyxh.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.hfpthk.cn/gtpmnsosod.html

[O06] 使用进程池
来源：http://hz.yj20258.top/gtfxfwgycg.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.ydzc1.top/gtgcfjbrrw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.hongshengwenyu.top/gtfhrkqmez.html

JS:   // child_process / cluster 模块
来源：http://hz.chenlongwang.top/gtzkhmhzwu.html

TS:   // child_process / cluster 模块
来源：http://hz.snrcjt.cn/gtzlzdnrix.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yangfankeji.com/gtritsbktd.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.smart0.xyz/gtuwhbpaen.html

Ruby: // fork 块
来源：http://hz.hywenlv.cn/gtazorsjiq.html

C#:   Parallel.For
来源：http://hz.hongshengwenyu.top/gtkxdwqwzs.html

================================================================================
来源：http://hz.svipenyu.cn/gtejmzqnvt.html

P. 常用工具函数
来源：http://hz.xylfe.cn/gtcbbllmwv.html

================================================================================
来源：http://hz.shzxlz.cn/gtkcjionyi.html

[P01] 生成 UUID
来源：http://hz.nanxuanxn.top/gtgyinxpls.html

Py:   str(uuid.uuid4())
来源：http://hz.zhoulong.xyz/gtjjgtgpeb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.cucudq.cn/gtxifptpkc.html

JS:   crypto.randomUUID()
来源：http://hz.snrcjt.cn/gtxdsgnyhj.html

TS:   crypto.randomUUID()
来源：http://hz.aibaodan.cn/gtdlobrncu.html

Java: UUID.randomUUID().toString()
来源：http://hz.jlsjyb.cn/gtoqczjfbl.html

Go:   // 用 github.com/google/uuid
来源：http://hz.52xcode.cn/gtszomkfdn.html

Ruby: SecureRandom.uuid
来源：http://hz.zhaomingkeji.xyz/gtqgtoogsf.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.9152youxi.cn/gtgkgwgqfq.html

[P02] MD5 / SHA256 摘要
来源：http://hz.c1oappe.top/gtwkstnjxt.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.daxiang520.top/gtspcmexis.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.sxryk.cn/gtsvkfefaa.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.tianlin.xyz/gtjlmmquyt.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.xuetiantiany.cn/gtixsoxdia.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.nanxuanxn.top/gtwevrtkmt.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.xuanzx.com/gtosxysljt.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.havefunace.top/gterueqhla.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.hnqzz.top/gttyuflfky.html

[P03] 生成短随机字符串
来源：http://hz.shanyushiyangtech.top/gtankjnloz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.yongpay.top/gtidmmwpyn.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.hywenlv.cn/gtzrmwwqai.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.cqqwz.cn/gtkixvjlbm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.0kj1m.cn/gtkdehmtvf.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.chenlongwang.top/gtzkzbltug.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yj202588.top/gtadckdnxs.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.cdnleiting.top/gtjbdfgfyx.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jinqigufen.top/gtohbdeuik.html

[P04] 求长度
来源：http://hz.sufxvd.cn/gtupdkoqbx.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.zhijiandao.cn/gtwhqwxuki.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.bjfxy.top/gtfypaahpv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.meibo888.top/gtlsvsfvar.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xuetiantiany.cn/gtoxwziviy.html

Java: list.size();  map.size();  s.length()
来源：http://hz.gogol.net.cn/gtgibvpcko.html

Go:   len(arr);  len(m)
来源：http://hz.jqgufenzy.top/gtqfsacbar.html

Ruby: x.length;  x.size
来源：http://hz.yangfankeji.com/gtfpmmcvnn.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.xingfuxueyuan.xyz/gtzqrjdjdn.html

[P05] 判断两个对象内容是否相等
来源：http://hz.zdqjudy.top/gtmkdiufgd.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.yj202588.top/gtbwmgujjl.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.0kj1m.cn/gthfljkxre.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.hfpthk.cn/gtukppifta.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jinyuanbaomall.cn/gtbexrycap.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.ydzc1.top/gtgpyvlgto.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yanxiufei.cn/gtrsrgdqad.html

Ruby: a == b
来源：http://hz.hnqzz.top/gtwbwuhtxf.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.yuanzhike.top/gtvorokwmk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.ehwqpu.com/gttrhahmwl.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.cheryme.top/gtdsjvjimi.html

PHP:  if (empty($x)) {}
来源：http://hz.nwbrower.top/gthwsulhbv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.quarkkingdee.top/gtwbabkuvd.html

TS:   if (x == null) {}
来源：http://hz.chenjidiqi.icu/gtgkkcpgnb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.zhongyouzk.top/gtisuevrzv.html

Go:   if x == nil {}
来源：http://hz.guannengcc.top/gtybkkmmpa.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jianghu66.top/gtsexkqwof.html

C#:   if (x is null) {}
来源：http://hz.snrcjt.cn/gtdipwgzny.html

[P07] 防抖与节流
来源：http://hz.hongshengwenyu.top/gtsrguotgh.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.52xcode.cn/gthtypqlgm.html

PHP:  // 手写时间戳比较
来源：http://hz.yanxiufei.cn/gteplmbcdn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhijiandao.cn/gtzwaberqt.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.meibo888.top/gtiejccprs.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.hammf.cn/gtjuvfpupv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.zhiwuduotai.top/gttuufsxck.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.jinqigufen.top/gtoadxvlet.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.shanyushiyangkeji.top/gtnkffctrn.html

[P08] 处理浮点精度问题
来源：http://hz.xuetiantiany.cn/gtdgppsuai.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jinghuilouyu.cn/gthzydqxkv.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.zdqjudy.top/gtbqdwwzeb.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.nanxinkj.top/gtxfouzori.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.sxryk.cn/gtajwuwbvx.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.tian-w.cn/gttouiixwq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.tanke756.top/gtwrxbkbjw.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.yanxiufei.cn/gtshowsqtg.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.ehwqpu.com/gtujvmilpx.html

================================================================================
来源：http://hz.zhijiandao.cn/gtlijpyoyn.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yj202588.top/gtlpzbeftj.html

================================================================================
来源：http://hz.jiagoushi.top/gtmlcsjglb.html

[Q01] 创建表
来源：http://hz.dashuyun.cn/gtwxlkvjus.html

CREATE TABLE users (
来源：http://hz.snrcjt.cn/gthaqlfngp.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.vqdsnc.cn/gtarhdterf.html

name VARCHAR(50) NOT NULL,
来源：http://hz.xuanzx.com/gtupkqsinr.html

email VARCHAR(100) UNIQUE,
来源：http://hz.c1oappe.top/gtzavimofu.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.aibaodan.cn/gtbcasvtzw.html

);
来源：http://hz.vqdsnc.cn/gtayppnohe.html

[Q02] 创建带外键的表
来源：http://hz.ppjwa.cn/gtglgrrrev.html

CREATE TABLE orders (
来源：http://hz.aizwys.cn/gtgfpoxpkf.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.guowangkeji.top/gtllxcmzfb.html

user_id INT NOT NULL,
来源：http://hz.gaohongyu789.top/gtxkovyniq.html

amount DECIMAL(10, 2),
来源：http://hz.jqgufenzy.top/gthqokihqb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.feifeiyinyue.top/gtsqkqnamz.html

);
来源：http://hz.52xcode.cn/gtjgowbfue.html

[Q03] 增加列
来源：http://hz.guowangkeji.top/gtlqxvbjdp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.ppjwa.cn/gtdtxsownw.html

[Q04] 修改列类型
来源：http://hz.kuanghao11.cn/gtsolunilh.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.ywan-chungtsiang.top/gtovigxjay.html

[Q05] 重命名列
来源：http://hz.pengpengdd.cyou/gtwvkhxgqu.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.hongshengwenyu.top/gtyltmymgi.html

[Q06] 删除列
来源：http://hz.guannengcc.top/gtvcdotyqx.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.chenjidiqi.icu/gtseuvgamm.html

[Q07] 删除表
来源：http://hz.redwolf501.top/gtbzhaohaz.html

DROP TABLE IF EXISTS orders;
来源：http://hz.pengpengdd.cyou/gtrhwovmzj.html

[Q08] 创建普通索引
来源：http://hz.meibo888.top/gtbrqtndmh.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.gaohongyu789.top/gtxxasfbgf.html

[Q09] 创建唯一索引
来源：http://hz.zhoulong.xyz/gtmygieocx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.chenzaomai.com/gtohksnapz.html

[Q10] 插入单行
来源：http://hz.yanxiufei.cn/gtwxjfozpf.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.havefunace.top/gtxdrcmabw.html

[Q11] 一次插入多行
来源：http://hz.daria6918.cn/gtpiozfzkg.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.52xcode.cn/gtucywnmir.html

[Q12] 插入后取自增 ID
来源：http://hz.shangyingyoupin.top/gtapbumugd.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.aibaodan.cn/gtishpfsnk.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.jqgfzy.top/gtbpnqnxrs.html

[Q13] 忽略重复插入
来源：http://hz.kuanghao11.cn/gtwwiiztqk.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.hysaishi.cn/gtelmosmpe.html

[Q14] 存在则更新（upsert）
来源：http://hz.vqdsnc.cn/gtkermqhnk.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.bjfxy.top/gtwjvlmpqa.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.xinyue.icu/gtjysuayey.html

[Q15] 查询全部
来源：http://hz.shangyingyoupin.top/gtlvwdqetv.html

SELECT * FROM users;
来源：http://hz.cdnleiting.top/gtyzjdkjkj.html

[Q16] 查询指定列
来源：http://hz.xuanzx.com/gtzuugueoy.html

SELECT id, name FROM users;
来源：http://hz.ybcxt.top/gtytancixt.html

[Q17] 条件查询
来源：http://hz.ppjwa.cn/gtlboxcxzi.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.yonumen.top/gtcxcpagbf.html

[Q18] 模糊匹配
来源：http://hz.ivvv.top/gtcqforqli.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.svipenyu.cn/gtvluwasrd.html

[Q19] 范围查询
来源：http://hz.quarkkingdee.top/gtkhjsqedp.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.yj20258888.top/gtbjlgbgmt.html

[Q20] IN 列表
来源：http://hz.nwbrower.top/gtfsxlidzr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.xingfuxueyuan.xyz/gtkfryfozy.html

[Q21] 空值判断
来源：http://hz.hfpthk.cn/gtetwzpuaj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.yuxming.cn/gtazyxulgl.html

[Q22] 排序
来源：http://hz.zhengqikj.top/gttzanxtyr.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.tian-w.cn/gtmlbmnnla.html

[Q23] 分页
来源：http://hz.ywan-chungtsiang.top/gtobhmnokb.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.shangyingyoupin.top/gtipwhiycy.html

[Q24] 去重
来源：http://hz.guowangkeji.top/gtjhybiajs.html

SELECT DISTINCT city FROM users;
来源：http://hz.zhixingplan.top/gtvfulgyyr.html

[Q25] 只取前 N 条
来源：http://hz.yanxiufei.cn/gtcggopjud.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.sysykeji.top/gtyekacuta.html

[Q26] 计数
来源：http://hz.cashguo.top/gtjqkrjpnm.html

SELECT COUNT(*) FROM users;
来源：http://hz.sysykeji.top/gtillersaa.html

[Q27] 条件计数
来源：http://hz.jinqigufen.top/gtkelmrczg.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.guannengcc.top/gtxbfsjgzp.html

[Q28] 求和与平均
来源：http://hz.hammf.cn/gtpklzbtfj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.hammf.cn/gtbsxvwtcg.html

[Q29] 最大最小值
来源：http://hz.wangshuangyany.cn/gtwnmxittg.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.yonumen.top/gtqemdiwlj.html

[Q30] 分组统计
来源：http://hz.zycfv.cn/gtzidsotmr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.zhengqikj.top/gtrhnjeiqj.html

[Q31] 分组后过滤
来源：http://hz.xinyue.icu/gtdukujhpi.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.tanke756.top/gtavltxpiv.html

[Q32] 分组拼接字符串
来源：http://hz.pycfn.com/gtegbepopz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.feifeiyinyue.top/gtguluceto.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.chenjidiqi.icu/gtxmanwvrq.html

[Q33] 多列分组
来源：http://hz.guannengcc.top/gtawkkgbvg.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.fengsongda.top/gtapyfsyfu.html

[Q34] 每组取第一条
来源：http://hz.hammf.cn/gtszrxpqff.html

SELECT * FROM (
来源：http://hz.yuxming.cn/gtodiwoggl.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.kuanghao11.cn/gtwkeifoiu.html

) t WHERE rn = 1;
来源：http://hz.shzxlz.cn/gtiaoabmnd.html

[Q35] 内连接
来源：http://hz.dashuyun.cn/gtucpiyrtw.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.wangshuangyany.cn/gtgtnuyfcd.html

[Q36] 左连接
来源：http://hz.xuetiantiany.cn/gtdcxlndli.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.bjfxy.top/gttqvmhgcm.html

[Q37] 右连接
来源：http://hz.sweek.top/gtmyftykng.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.zhijiandao.cn/gtbvnrkets.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.wangshuangyany.cn/gtpdszfmfm.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.yj202588.top/gtmpskkglh.html

[Q39] 自连接（查上下级）
来源：http://hz.havefunace.top/gtprjsrsre.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.zhongyouzk.top/gtfdufddte.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.kuanghao11.cn/gtfgijchwr.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.redwolf501.top/gtsnwxqkqa.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.zycfv.cn/gthbqprfyg.html

[Q41] 多表连接
来源：http://hz.xylfe.cn/gtpwvupslg.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.52xcode.cn/gtxdwxixwp.html

JOIN users u ON u.id = o.user_id
来源：http://hz.xingfuxueyuan.xyz/gtbzcbhlbi.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.ppjwa.cn/gthosfcyvb.html

[Q42] 连接条件附加过滤
来源：http://hz.tanke756.top/gtjkkppuqc.html

SELECT u.name, o.amount FROM users u
来源：http://hz.yuanzhike.top/gtetffbovd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.daria6918.cn/gtxgvydtul.html

[Q43] 标量子查询
来源：http://hz.cheryme.top/gtiwlrpgbk.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.jiagoushi.top/gttbwjhovq.html

[Q44] IN 子查询
来源：http://hz.zhaomingkeji.xyz/gtaosbrpmz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.jiagoushi.top/gtinjeqwhh.html

[Q45] EXISTS 判断存在
来源：http://hz.gzhubu.top/gtrahrbsoy.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.guannengcc.top/gtieepvbgr.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.daxiang520.top/gtuklkvrcv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.gotoacloud.top/gtgnaggzgc.html

[Q47] 与平均值比较
来源：http://hz.aizwys.cn/gtpgfpdprn.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.sufxvd.cn/gteerajxxe.html

[Q48] CTE 公用表表达式
来源：http://hz.smart0.xyz/gtwatmoufo.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jinqigufen.top/gtnxrmpudn.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.feifeiyinyue.top/gtllqexlyf.html

[Q49] 更新单行
来源：http://hz.yuanzhike.top/gtbuxnmzbe.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.jinqigufen.top/gtzptftkvy.html

[Q50] 批量更新
来源：http://hz.jinghuilouyu.cn/gtqxqhzyas.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.shanyushiyangkeji.top/gtupjcnccs.html

[Q51] 用子查询更新
来源：http://hz.xuanzx.com/gtfswitqwv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.ivvv.top/gtagylrtaz.html

[Q52] 删除指定行
来源：http://hz.zhengqikj.top/gtbbamihll.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yj20258.top/gthovrmoxp.html

[Q53] 按条件删除
来源：http://hz.tianlin.xyz/gtggpytwgz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yuxming.cn/gthzmhdobc.html

[Q54] 清空表
来源：http://hz.cheryme.top/gtdvroayov.html

TRUNCATE TABLE logs;
来源：http://hz.shanyushiyangkeji.top/gtlbpmmhcc.html

[Q55] 排名（并列占位）
来源：http://hz.jinghuilouyu.cn/gtalvwapey.html


<!-- 参考信息 -->