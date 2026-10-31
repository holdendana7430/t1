代发 wailian999

[N05] 最大公约数
来源：http://bf.lnxyls.cn

Py:   math.gcd(a, b)
来源：http://hv.lnxyls.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://au.bookmarksfly.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oh.yuntaijiaju.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mp.jctech888.com.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://pz.haigaiapp.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ml.asd995.cn

Ruby: a.gcd(b)
来源：http://ed.9csxet.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ln.jctech888.com.cn

[N06] 判断回文字符串
来源：http://eh.hahajie.cn

Py:   s == s[::-1]
来源：http://vi.chemitech.net.cn

PHP:  $s === strrev($s);
来源：http://mk.nicolike.cn

JS:   s === [...s].reverse().join("")
来源：http://hk.9csxet.cn

TS:   s === [...s].reverse().join("")
来源：http://ng.lnxyls.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://cy.haigaiapp.cn

Go:   // 双指针从两端比较
来源：http://ft.bjjhwx.cn

Ruby: s == s.reverse
来源：http://kr.wgjwhj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ry.newstarts.cn

[N07] 两数之和（返回下标）
来源：http://mf.bookmarksfly.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ol.bookmarksfly.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fk.yuexingan06.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ha.hahajie.cn

TS:   // 手写 Map<string, number>
来源：http://ri.lnxyls.cn

Java: // 手写 HashMap
来源：http://ci.bookmarksfly.cn

Go:   // 手写 map[int]int
来源：http://sn.jianghongdianzi.cn

Ruby: // 手写 Hash
来源：http://ek.colortex.cn

C#:   // 手写 Dictionary<int, int>
来源：http://cw.szsharing.cn

[N08] 生成全排列
来源：http://od.szxytkj.cn

Py:   itertools.permutations(arr)
来源：http://qt.jctech888.com.cn

PHP:  // 手写递归交换
来源：http://ak.colortex.cn

JS:   // 手写回溯递归
来源：http://xp.yuexingan06.cn

TS:   // 手写回溯递归
来源：http://ux.muxihuayi.cn

Java: // 手写回溯递归
来源：http://ul.nszjky.cn

Go:   // 手写回溯递归
来源：http://gg.wgjwhj.cn

Ruby: arr.permutation.to_a
来源：http://um.panjiajie.cn

C#:   // 手写回溯递归
来源：http://hb.shxzskj.cn

[N09] 栈与队列
来源：http://ka.jianghongdianzi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rz.huixiangedu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mp.panjiajie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://tt.jctech888.com.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://yr.shxzukj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://tz.huixiangedu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kn.gzmigu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ki.haigaiapp.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cg.9csxet.cn

[N10] 链表节点定义
来源：http://qh.newstarts.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lm.newstarts.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://nr.haigaiapp.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://if.shxzskj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ka.shxzukj.cn

Java: class Node { int v; Node next; }
来源：http://kn.newstarts.cn

Go:   type Node struct { V int; Next *Node }
来源：http://rc.jctech888.com.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://uz.huixiangedu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://va.chemitech.net.cn

[N11] 二叉树中序遍历
来源：http://kn.nszjky.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ga.gzmigu.cn

PHP:  // 手写递归函数
来源：http://zy.shxzukj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qj.gzmigu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kl.bookmarksfly.cn

Java: // 手写递归
来源：http://ul.haigaiapp.cn

Go:   // 手写递归
来源：http://yl.hahajie.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xf.muxihuayi.cn

C#:   // 手写递归
来源：http://hh.521024.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pr.huanxung.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://lk.szsharing.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zn.bookmarksfly.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lj.colortex.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sv.bookmarksfly.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://py.huanxung.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zb.hahajie.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qg.shxzskj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hf.bookmarksfly.cn

================================================================================
来源：http://pu.nicolike.cn

O. 并发与异步
来源：http://ok.jctech888.com.cn

================================================================================
来源：http://fy.nszjky.cn

[O01] 启动一个线程
来源：http://iw.hnjuh.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wc.colortex.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xc.colortex.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hj.bookmarksfly.cn

TS:   // 同 JS
来源：http://hr.huanxung.cn

Java: new Thread(() -> f()).start()
来源：http://ze.yuntaijiaju.cn

Go:   go f()
来源：http://vi.szsharing.cn

Ruby: Thread.new { f }
来源：http://jw.colortex.cn

C#:   Task.Run(() => F());
来源：http://eu.newstarts.cn

[O02] 使用线程池
来源：http://st.huixiangedu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://yp.huanxung.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zi.szsharing.cn

JS:   // worker_threads 线程池
来源：http://yn.shtwfgs.cn

TS:   // worker_threads 线程池
来源：http://fp.huixinmuqiang.cn

Java: Executors.newFixedThreadPool(4)
来源：http://jm.muxihuayi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://gm.chemitech.net.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zj.huixinmuqiang.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nh.chemitech.net.cn

[O03] 加锁保护共享数据
来源：http://xq.521024.cn

Py:   with lock: shared += 1
来源：http://uw.gzmigu.cn

PHP:  // 用 flock() 做文件锁
来源：http://ur.colortex.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wi.huixinmuqiang.cn

TS:   // 同 JS
来源：http://if.yuntaijiaju.cn

Java: synchronized (this) { shared++; }
来源：http://bl.shxzukj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://th.huixiangedu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ne.yuexingan06.cn

C#:   lock (gate) { shared++; }
来源：http://uj.521024.cn

[O04] 定义异步函数并等待
来源：http://fv.huanxung.cn

Py:   async def f():⏎    await g()
来源：http://zp.muxihuayi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ff.haigaiapp.cn

JS:   async function f() { await g(); }
来源：http://df.muxihuayi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ip.shtwfgs.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ex.yuexingan06.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qq.bjjhwx.cn

Ruby: # 用 Fiber 或 async gem
来源：http://xw.yuntaijiaju.cn

C#:   async Task F() { await G(); }
来源：http://lz.colortex.cn

[O05] 并发执行并等待全部完成
来源：http://lx.szsharing.cn

Py:   asyncio.gather(*tasks)
来源：http://sh.nszjky.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://th.hnjuh.cn

JS:   await Promise.all(tasks)
来源：http://xp.newstarts.cn

TS:   await Promise.all(tasks)
来源：http://hf.shxzukj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pb.nicolike.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nh.nicolike.cn

Ruby: threads.map(&:join)
来源：http://rf.9csxet.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://xg.chemitech.net.cn

[O06] 使用进程池
来源：http://th.huanxung.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jm.shxzukj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://pk.wgjwhj.cn

JS:   // child_process / cluster 模块
来源：http://am.nicolike.cn

TS:   // child_process / cluster 模块
来源：http://sl.hahajie.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lp.9csxet.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://yp.jianghongdianzi.cn

Ruby: // fork 块
来源：http://vt.shxzskj.cn

C#:   Parallel.For
来源：http://hs.hnjuh.cn

================================================================================
来源：http://di.asd995.cn

P. 常用工具函数
来源：http://tg.jianghongdianzi.cn

================================================================================
来源：http://az.chemitech.net.cn

[P01] 生成 UUID
来源：http://id.huixiangedu.cn

Py:   str(uuid.uuid4())
来源：http://ld.shtwfgs.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ry.newstarts.cn

JS:   crypto.randomUUID()
来源：http://yh.szsharing.cn

TS:   crypto.randomUUID()
来源：http://nm.yuexingan06.cn

Java: UUID.randomUUID().toString()
来源：http://ky.wgjwhj.cn

Go:   // 用 github.com/google/uuid
来源：http://lx.hnjuh.cn

Ruby: SecureRandom.uuid
来源：http://wl.colortex.cn

C#:   Guid.NewGuid().ToString()
来源：http://xl.szsharing.cn

[P02] MD5 / SHA256 摘要
来源：http://lu.szxytkj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mf.bjjhwx.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://oq.yuntaijiaju.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gq.wgjwhj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bc.bookmarksfly.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://oo.panjiajie.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://su.shxzukj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ov.huixinmuqiang.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ei.huixiangedu.cn

[P03] 生成短随机字符串
来源：http://bh.shtwfgs.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mp.newstarts.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ri.huixinmuqiang.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qx.newstarts.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mx.newstarts.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://sk.jianghongdianzi.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ln.yuexingan06.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://nx.huixinmuqiang.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rn.szsharing.cn

[P04] 求长度
来源：http://wp.wgjwhj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mi.muxihuayi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kr.hahajie.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ty.szsharing.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://oo.bookmarksfly.cn

Java: list.size();  map.size();  s.length()
来源：http://us.chemitech.net.cn

Go:   len(arr);  len(m)
来源：http://nu.wgjwhj.cn

Ruby: x.length;  x.size
来源：http://mh.yuexingan06.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://xj.newstarts.cn

[P05] 判断两个对象内容是否相等
来源：http://vc.bjjhwx.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://dz.nszjky.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bl.jianghongdianzi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jq.jctech888.com.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://km.panjiajie.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hj.hahajie.cn

Go:   reflect.DeepEqual(a, b)
来源：http://jx.shtwfgs.cn

Ruby: a == b
来源：http://rz.jctech888.com.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vi.muxihuayi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ta.hahajie.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wt.jctech888.com.cn

PHP:  if (empty($x)) {}
来源：http://vu.9csxet.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ro.jianghongdianzi.cn

TS:   if (x == null) {}
来源：http://al.szsharing.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://gu.jctech888.com.cn

Go:   if x == nil {}
来源：http://bz.huanxung.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ej.asd995.cn

C#:   if (x is null) {}
来源：http://ig.521024.cn

[P07] 防抖与节流
来源：http://od.huixinmuqiang.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://px.shtwfgs.cn

PHP:  // 手写时间戳比较
来源：http://yj.nszjky.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wx.yuexingan06.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kf.nicolike.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://lw.asd995.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hk.huixiangedu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://fu.shxzskj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://es.bjjhwx.cn

[P08] 处理浮点精度问题
来源：http://gd.colortex.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://lx.colortex.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://rw.lnxyls.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://yw.haigaiapp.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mu.szsharing.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vr.bookmarksfly.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qh.shtwfgs.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lg.yuntaijiaju.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bj.muxihuayi.cn

================================================================================
来源：http://pl.shtwfgs.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wr.huanxung.cn

================================================================================
来源：http://zl.shxzukj.cn

[Q01] 创建表
来源：http://al.bookmarksfly.cn

CREATE TABLE users (
来源：http://zc.colortex.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jt.asd995.cn

name VARCHAR(50) NOT NULL,
来源：http://sk.wgjwhj.cn

email VARCHAR(100) UNIQUE,
来源：http://fd.521024.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://or.jianghongdianzi.cn

);
来源：http://fx.muxihuayi.cn

[Q02] 创建带外键的表
来源：http://yg.nicolike.cn

CREATE TABLE orders (
来源：http://av.yuexingan06.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://oi.szxytkj.cn

user_id INT NOT NULL,
来源：http://nd.asd995.cn

amount DECIMAL(10, 2),
来源：http://ga.jctech888.com.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://dy.shtwfgs.cn

);
来源：http://bf.jctech888.com.cn

[Q03] 增加列
来源：http://cs.huixiangedu.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://de.muxihuayi.cn

[Q04] 修改列类型
来源：http://wj.wgjwhj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://pe.muxihuayi.cn

[Q05] 重命名列
来源：http://el.chemitech.net.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://sz.muxihuayi.cn

[Q06] 删除列
来源：http://rn.shxzukj.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ni.nszjky.cn

[Q07] 删除表
来源：http://nj.huixiangedu.cn

DROP TABLE IF EXISTS orders;
来源：http://qj.bookmarksfly.cn

[Q08] 创建普通索引
来源：http://ir.huixiangedu.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://fv.hnjuh.cn

[Q09] 创建唯一索引
来源：http://qt.nszjky.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ea.huanxung.cn

[Q10] 插入单行
来源：http://np.nicolike.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wa.haigaiapp.cn

[Q11] 一次插入多行
来源：http://qo.chemitech.net.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ip.chemitech.net.cn

[Q12] 插入后取自增 ID
来源：http://fr.chemitech.net.cn

INSERT INTO users (name) VALUES ('C');
来源：http://zt.hnjuh.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wn.muxihuayi.cn

[Q13] 忽略重复插入
来源：http://xd.chemitech.net.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://uq.jianghongdianzi.cn

[Q14] 存在则更新（upsert）
来源：http://aj.shxzukj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wt.gzmigu.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lv.szxytkj.cn

[Q15] 查询全部
来源：http://hg.bjjhwx.cn

SELECT * FROM users;
来源：http://oy.huixinmuqiang.cn

[Q16] 查询指定列
来源：http://zb.jctech888.com.cn

SELECT id, name FROM users;
来源：http://mw.haigaiapp.cn

[Q17] 条件查询
来源：http://wg.shxzskj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://on.hahajie.cn

[Q18] 模糊匹配
来源：http://ti.hahajie.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://we.9csxet.cn

[Q19] 范围查询
来源：http://st.hnjuh.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nx.hnjuh.cn

[Q20] IN 列表
来源：http://mm.shxzskj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kc.muxihuayi.cn

[Q21] 空值判断
来源：http://fz.colortex.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://mb.bookmarksfly.cn

[Q22] 排序
来源：http://jh.hahajie.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://la.haigaiapp.cn

[Q23] 分页
来源：http://wd.newstarts.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ma.asd995.cn

[Q24] 去重
来源：http://zf.shxzskj.cn

SELECT DISTINCT city FROM users;
来源：http://me.bjjhwx.cn

[Q25] 只取前 N 条
来源：http://hf.9csxet.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ke.bjjhwx.cn

[Q26] 计数
来源：http://sg.jianghongdianzi.cn

SELECT COUNT(*) FROM users;
来源：http://po.9csxet.cn

[Q27] 条件计数
来源：http://ja.gzmigu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://bi.shtwfgs.cn

[Q28] 求和与平均
来源：http://lz.muxihuayi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ws.hahajie.cn

[Q29] 最大最小值
来源：http://xv.shxzskj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://lu.shtwfgs.cn

[Q30] 分组统计
来源：http://nm.wgjwhj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vk.hnjuh.cn

[Q31] 分组后过滤
来源：http://rk.colortex.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://sm.szxytkj.cn

[Q32] 分组拼接字符串
来源：http://za.shxzukj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wq.yuexingan06.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ex.muxihuayi.cn

[Q33] 多列分组
来源：http://eu.gzmigu.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://yl.wgjwhj.cn

[Q34] 每组取第一条
来源：http://qb.nszjky.cn

SELECT * FROM (
来源：http://us.haigaiapp.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xu.nszjky.cn

) t WHERE rn = 1;
来源：http://tl.huixiangedu.cn

[Q35] 内连接
来源：http://ke.nszjky.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wg.jianghongdianzi.cn

[Q36] 左连接
来源：http://gi.szsharing.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://be.bjjhwx.cn

[Q37] 右连接
来源：http://cu.newstarts.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://no.colortex.cn

[Q38] 全外连接（PostgreSQL）
来源：http://bx.jctech888.com.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ai.asd995.cn

[Q39] 自连接（查上下级）
来源：http://ap.nszjky.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://yp.haigaiapp.cn


<!-- 参考信息 -->