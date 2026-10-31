代发 wailian999

[N05] 最大公约数
来源：http://zx.newstarts.cn

Py:   math.gcd(a, b)
来源：http://mb.shxzskj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ut.gzmigu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mi.huixinmuqiang.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fu.hnjuh.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vn.yuntaijiaju.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ye.bookmarksfly.cn

Ruby: a.gcd(b)
来源：http://ow.hnjuh.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fw.jianghongdianzi.cn

[N06] 判断回文字符串
来源：http://gx.asd995.cn

Py:   s == s[::-1]
来源：http://qc.hahajie.cn

PHP:  $s === strrev($s);
来源：http://uh.newstarts.cn

JS:   s === [...s].reverse().join("")
来源：http://rg.yuntaijiaju.cn

TS:   s === [...s].reverse().join("")
来源：http://zw.hnjuh.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gu.colortex.cn

Go:   // 双指针从两端比较
来源：http://nu.bjjhwx.cn

Ruby: s == s.reverse
来源：http://yt.bookmarksfly.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://fj.lnxyls.cn

[N07] 两数之和（返回下标）
来源：http://rw.huanxung.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gv.huanxung.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://go.521024.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://uy.asd995.cn

TS:   // 手写 Map<string, number>
来源：http://gb.lnxyls.cn

Java: // 手写 HashMap
来源：http://ev.huixinmuqiang.cn

Go:   // 手写 map[int]int
来源：http://dz.wgjwhj.cn

Ruby: // 手写 Hash
来源：http://xv.9csxet.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ja.hahajie.cn

[N08] 生成全排列
来源：http://gk.nszjky.cn

Py:   itertools.permutations(arr)
来源：http://nl.muxihuayi.cn

PHP:  // 手写递归交换
来源：http://jn.nicolike.cn

JS:   // 手写回溯递归
来源：http://zt.hnjuh.cn

TS:   // 手写回溯递归
来源：http://px.yuntaijiaju.cn

Java: // 手写回溯递归
来源：http://qc.huanxung.cn

Go:   // 手写回溯递归
来源：http://gx.szsharing.cn

Ruby: arr.permutation.to_a
来源：http://se.jctech888.com.cn

C#:   // 手写回溯递归
来源：http://nr.colortex.cn

[N09] 栈与队列
来源：http://yw.muxihuayi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://me.wgjwhj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cm.yuntaijiaju.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dq.szsharing.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ta.hnjuh.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hu.muxihuayi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://oc.panjiajie.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://is.szsharing.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hn.muxihuayi.cn

[N10] 链表节点定义
来源：http://ot.bookmarksfly.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qi.yuntaijiaju.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ij.panjiajie.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ip.szsharing.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ep.gzmigu.cn

Java: class Node { int v; Node next; }
来源：http://pk.hnjuh.cn

Go:   type Node struct { V int; Next *Node }
来源：http://pe.haigaiapp.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://vq.lnxyls.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://es.yuntaijiaju.cn

[N11] 二叉树中序遍历
来源：http://rt.jianghongdianzi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://nu.chemitech.net.cn

PHP:  // 手写递归函数
来源：http://dn.colortex.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yv.wgjwhj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vs.huanxung.cn

Java: // 手写递归
来源：http://sl.bookmarksfly.cn

Go:   // 手写递归
来源：http://tb.muxihuayi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://md.yuntaijiaju.cn

C#:   // 手写递归
来源：http://tg.newstarts.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://yt.nszjky.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qr.szxytkj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qr.lnxyls.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dc.9csxet.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hl.huanxung.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qg.muxihuayi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pd.yuexingan06.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bj.wgjwhj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://eq.muxihuayi.cn

================================================================================
来源：http://xn.nszjky.cn

O. 并发与异步
来源：http://qt.shxzukj.cn

================================================================================
来源：http://xu.shtwfgs.cn

[O01] 启动一个线程
来源：http://xf.shxzukj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ts.muxihuayi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://cg.muxihuayi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wl.panjiajie.cn

TS:   // 同 JS
来源：http://qr.wgjwhj.cn

Java: new Thread(() -> f()).start()
来源：http://sm.jctech888.com.cn

Go:   go f()
来源：http://sa.hnjuh.cn

Ruby: Thread.new { f }
来源：http://mz.hnjuh.cn

C#:   Task.Run(() => F());
来源：http://qj.jctech888.com.cn

[O02] 使用线程池
来源：http://pc.yuntaijiaju.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://nd.colortex.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zz.gzmigu.cn

JS:   // worker_threads 线程池
来源：http://bp.lnxyls.cn

TS:   // worker_threads 线程池
来源：http://br.yuexingan06.cn

Java: Executors.newFixedThreadPool(4)
来源：http://gr.nszjky.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://te.hnjuh.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vn.haigaiapp.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gv.shtwfgs.cn

[O03] 加锁保护共享数据
来源：http://ds.haigaiapp.cn

Py:   with lock: shared += 1
来源：http://cd.shtwfgs.cn

PHP:  // 用 flock() 做文件锁
来源：http://ta.colortex.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ve.lnxyls.cn

TS:   // 同 JS
来源：http://cu.nszjky.cn

Java: synchronized (this) { shared++; }
来源：http://zf.colortex.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://se.muxihuayi.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://cw.nszjky.cn

C#:   lock (gate) { shared++; }
来源：http://sj.colortex.cn

[O04] 定义异步函数并等待
来源：http://lp.521024.cn

Py:   async def f():⏎    await g()
来源：http://xu.hahajie.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kx.521024.cn

JS:   async function f() { await g(); }
来源：http://kk.lnxyls.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://uk.huixinmuqiang.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xe.szsharing.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pd.newstarts.cn

Ruby: # 用 Fiber 或 async gem
来源：http://py.9csxet.cn

C#:   async Task F() { await G(); }
来源：http://xm.lnxyls.cn

[O05] 并发执行并等待全部完成
来源：http://ah.wgjwhj.cn

Py:   asyncio.gather(*tasks)
来源：http://oq.jianghongdianzi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zl.yuexingan06.cn

JS:   await Promise.all(tasks)
来源：http://px.szxytkj.cn

TS:   await Promise.all(tasks)
来源：http://lk.huixiangedu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jz.huixinmuqiang.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://jy.panjiajie.cn

Ruby: threads.map(&:join)
来源：http://nn.szsharing.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://lv.hnjuh.cn

[O06] 使用进程池
来源：http://mf.521024.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gd.colortex.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://nk.hahajie.cn

JS:   // child_process / cluster 模块
来源：http://qa.haigaiapp.cn

TS:   // child_process / cluster 模块
来源：http://lg.muxihuayi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tu.shxzukj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://uv.yuntaijiaju.cn

Ruby: // fork 块
来源：http://jx.panjiajie.cn

C#:   Parallel.For
来源：http://qg.lnxyls.cn

================================================================================
来源：http://fi.szxytkj.cn

P. 常用工具函数
来源：http://ia.jianghongdianzi.cn

================================================================================
来源：http://xx.haigaiapp.cn

[P01] 生成 UUID
来源：http://zp.shxzukj.cn

Py:   str(uuid.uuid4())
来源：http://pu.muxihuayi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xh.hnjuh.cn

JS:   crypto.randomUUID()
来源：http://oe.huixiangedu.cn

TS:   crypto.randomUUID()
来源：http://af.shxzukj.cn

Java: UUID.randomUUID().toString()
来源：http://kj.jctech888.com.cn

Go:   // 用 github.com/google/uuid
来源：http://jk.newstarts.cn

Ruby: SecureRandom.uuid
来源：http://zy.nicolike.cn

C#:   Guid.NewGuid().ToString()
来源：http://bp.9csxet.cn

[P02] MD5 / SHA256 摘要
来源：http://qj.lnxyls.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mo.szsharing.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ja.hahajie.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ww.hnjuh.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zp.wgjwhj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ti.nicolike.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nn.hahajie.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ow.shtwfgs.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tu.newstarts.cn

[P03] 生成短随机字符串
来源：http://mx.szsharing.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://it.muxihuayi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://fe.colortex.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wq.jctech888.com.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hm.szxytkj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ik.hahajie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ae.nicolike.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://pt.lnxyls.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://nv.newstarts.cn

[P04] 求长度
来源：http://ou.nszjky.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xd.yuexingan06.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://aj.hnjuh.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rg.9csxet.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zq.bookmarksfly.cn

Java: list.size();  map.size();  s.length()
来源：http://ip.lnxyls.cn

Go:   len(arr);  len(m)
来源：http://sh.9csxet.cn

Ruby: x.length;  x.size
来源：http://gl.wgjwhj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://se.jianghongdianzi.cn

[P05] 判断两个对象内容是否相等
来源：http://ty.shtwfgs.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ho.hahajie.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dt.chemitech.net.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://an.huixiangedu.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://un.haigaiapp.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://os.newstarts.cn

Go:   reflect.DeepEqual(a, b)
来源：http://nl.hnjuh.cn

Ruby: a == b
来源：http://oa.hahajie.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://nf.521024.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://fe.shtwfgs.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mh.muxihuayi.cn

PHP:  if (empty($x)) {}
来源：http://ys.huixinmuqiang.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://iz.huixiangedu.cn

TS:   if (x == null) {}
来源：http://ub.jianghongdianzi.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://js.nszjky.cn

Go:   if x == nil {}
来源：http://wx.huanxung.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://nv.haigaiapp.cn

C#:   if (x is null) {}
来源：http://gz.yuexingan06.cn

[P07] 防抖与节流
来源：http://ga.9csxet.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rt.521024.cn

PHP:  // 手写时间戳比较
来源：http://lq.newstarts.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ey.nszjky.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://le.wgjwhj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pk.shxzukj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://et.chemitech.net.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://wv.muxihuayi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://we.shtwfgs.cn

[P08] 处理浮点精度问题
来源：http://xc.yuntaijiaju.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mk.huixiangedu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://sy.newstarts.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zr.newstarts.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://oc.szxytkj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ux.521024.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://rg.chemitech.net.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zx.colortex.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://nn.newstarts.cn

================================================================================
来源：http://cf.shxzukj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vi.lnxyls.cn

================================================================================
来源：http://xb.huixinmuqiang.cn

[Q01] 创建表
来源：http://pp.bookmarksfly.cn

CREATE TABLE users (
来源：http://wq.wgjwhj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xn.jianghongdianzi.cn

name VARCHAR(50) NOT NULL,
来源：http://nk.shxzskj.cn

email VARCHAR(100) UNIQUE,
来源：http://yt.szsharing.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bq.bjjhwx.cn

);
来源：http://he.huixinmuqiang.cn

[Q02] 创建带外键的表
来源：http://ug.asd995.cn

CREATE TABLE orders (
来源：http://ot.panjiajie.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ma.yuexingan06.cn

user_id INT NOT NULL,
来源：http://uf.panjiajie.cn

amount DECIMAL(10, 2),
来源：http://pl.hahajie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://il.huixiangedu.cn

);
来源：http://nm.huanxung.cn

[Q03] 增加列
来源：http://ew.jianghongdianzi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fe.yuntaijiaju.cn

[Q04] 修改列类型
来源：http://wk.hnjuh.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yb.huixinmuqiang.cn

[Q05] 重命名列
来源：http://ng.521024.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://nw.huixinmuqiang.cn

[Q06] 删除列
来源：http://vd.jctech888.com.cn

ALTER TABLE users DROP COLUMN age;
来源：http://dq.newstarts.cn

[Q07] 删除表
来源：http://go.gzmigu.cn

DROP TABLE IF EXISTS orders;
来源：http://nx.bookmarksfly.cn

[Q08] 创建普通索引
来源：http://il.hnjuh.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://cq.hnjuh.cn

[Q09] 创建唯一索引
来源：http://ir.newstarts.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ki.shxzskj.cn

[Q10] 插入单行
来源：http://ny.panjiajie.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ro.panjiajie.cn

[Q11] 一次插入多行
来源：http://iy.chemitech.net.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gi.asd995.cn

[Q12] 插入后取自增 ID
来源：http://pe.shxzskj.cn

INSERT INTO users (name) VALUES ('C');
来源：http://li.hahajie.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wx.panjiajie.cn

[Q13] 忽略重复插入
来源：http://lz.shxzskj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fb.bjjhwx.cn

[Q14] 存在则更新（upsert）
来源：http://we.colortex.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vf.521024.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://rl.shxzukj.cn

[Q15] 查询全部
来源：http://tp.nszjky.cn

SELECT * FROM users;
来源：http://pf.szsharing.cn

[Q16] 查询指定列
来源：http://gh.szsharing.cn

SELECT id, name FROM users;
来源：http://go.hnjuh.cn

[Q17] 条件查询
来源：http://ni.lnxyls.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mi.szxytkj.cn

[Q18] 模糊匹配
来源：http://sz.hahajie.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jv.asd995.cn

[Q19] 范围查询
来源：http://af.shtwfgs.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://am.hnjuh.cn

[Q20] IN 列表
来源：http://sc.newstarts.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://aq.lnxyls.cn

[Q21] 空值判断
来源：http://uk.chemitech.net.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://jx.9csxet.cn

[Q22] 排序
来源：http://qy.hahajie.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://pa.huanxung.cn

[Q23] 分页
来源：http://rh.colortex.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xf.newstarts.cn

[Q24] 去重
来源：http://gc.lnxyls.cn

SELECT DISTINCT city FROM users;
来源：http://mz.9csxet.cn

[Q25] 只取前 N 条
来源：http://ke.haigaiapp.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zu.jianghongdianzi.cn

[Q26] 计数
来源：http://ib.nicolike.cn

SELECT COUNT(*) FROM users;
来源：http://wx.shxzukj.cn

[Q27] 条件计数
来源：http://bf.521024.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fs.hahajie.cn

[Q28] 求和与平均
来源：http://cz.nicolike.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://fx.chemitech.net.cn

[Q29] 最大最小值
来源：http://yg.shxzukj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://yr.nszjky.cn

[Q30] 分组统计
来源：http://ep.panjiajie.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vv.yuntaijiaju.cn

[Q31] 分组后过滤
来源：http://sx.huanxung.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yb.chemitech.net.cn

[Q32] 分组拼接字符串
来源：http://wt.hahajie.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mm.shxzukj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jr.nicolike.cn

[Q33] 多列分组
来源：http://pc.jianghongdianzi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ds.hnjuh.cn

[Q34] 每组取第一条
来源：http://nl.bjjhwx.cn

SELECT * FROM (
来源：http://rv.shxzskj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lh.muxihuayi.cn

) t WHERE rn = 1;
来源：http://jl.szxytkj.cn

[Q35] 内连接
来源：http://ee.colortex.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lu.hnjuh.cn

[Q36] 左连接
来源：http://ab.yuexingan06.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://lg.yuntaijiaju.cn

[Q37] 右连接
来源：http://kc.panjiajie.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ep.panjiajie.cn

[Q38] 全外连接（PostgreSQL）
来源：http://yy.shxzskj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://oy.shxzukj.cn

[Q39] 自连接（查上下级）
来源：http://kn.huixiangedu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://gu.newstarts.cn


<!-- 参考信息 -->