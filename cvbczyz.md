代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://uy.newstarts.cn

[N06] 判断回文字符串
来源：http://cy.colortex.cn

Py:   s == s[::-1]
来源：http://gb.wgjwhj.cn

PHP:  $s === strrev($s);
来源：http://vw.muxihuayi.cn

JS:   s === [...s].reverse().join("")
来源：http://ap.huixiangedu.cn

TS:   s === [...s].reverse().join("")
来源：http://xy.szxytkj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ij.9csxet.cn

Go:   // 双指针从两端比较
来源：http://wi.hnjuh.cn

Ruby: s == s.reverse
来源：http://pj.asd995.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://wq.lnxyls.cn

[N07] 两数之和（返回下标）
来源：http://js.521024.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gq.szxytkj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qc.szxytkj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://mx.haigaiapp.cn

TS:   // 手写 Map<string, number>
来源：http://eh.szsharing.cn

Java: // 手写 HashMap
来源：http://jw.newstarts.cn

Go:   // 手写 map[int]int
来源：http://tm.hahajie.cn

Ruby: // 手写 Hash
来源：http://dw.chemitech.net.cn

C#:   // 手写 Dictionary<int, int>
来源：http://oe.muxihuayi.cn

[N08] 生成全排列
来源：http://fj.yuexingan06.cn

Py:   itertools.permutations(arr)
来源：http://xs.bookmarksfly.cn

PHP:  // 手写递归交换
来源：http://mf.nicolike.cn

JS:   // 手写回溯递归
来源：http://wm.shxzukj.cn

TS:   // 手写回溯递归
来源：http://yi.shxzukj.cn

Java: // 手写回溯递归
来源：http://wk.bjjhwx.cn

Go:   // 手写回溯递归
来源：http://wu.521024.cn

Ruby: arr.permutation.to_a
来源：http://rz.shxzukj.cn

C#:   // 手写回溯递归
来源：http://gg.huixinmuqiang.cn

[N09] 栈与队列
来源：http://pe.haigaiapp.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://km.bookmarksfly.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tn.chemitech.net.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mw.nszjky.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pj.shtwfgs.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://sy.bookmarksfly.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wx.yuexingan06.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yl.szsharing.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gj.wgjwhj.cn

[N10] 链表节点定义
来源：http://ax.yuexingan06.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vr.lnxyls.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://qy.huanxung.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wi.colortex.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ud.hahajie.cn

Java: class Node { int v; Node next; }
来源：http://rx.hahajie.cn

Go:   type Node struct { V int; Next *Node }
来源：http://pu.szsharing.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ut.yuexingan06.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://rp.huixiangedu.cn

[N11] 二叉树中序遍历
来源：http://tg.shxzukj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cv.shxzukj.cn

PHP:  // 手写递归函数
来源：http://wf.nszjky.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ru.newstarts.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ew.521024.cn

Java: // 手写递归
来源：http://cb.muxihuayi.cn

Go:   // 手写递归
来源：http://fh.wgjwhj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fy.nicolike.cn

C#:   // 手写递归
来源：http://ww.szsharing.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zf.asd995.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xb.haigaiapp.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jg.shxzskj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vq.szxytkj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ea.wgjwhj.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://uy.szsharing.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://gb.asd995.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://nx.jctech888.com.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ib.wgjwhj.cn

================================================================================
来源：http://az.bjjhwx.cn

O. 并发与异步
来源：http://xk.yuntaijiaju.cn

================================================================================
来源：http://hx.nszjky.cn

[O01] 启动一个线程
来源：http://kj.huixiangedu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://oc.nszjky.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zk.asd995.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ri.hahajie.cn

TS:   // 同 JS
来源：http://qt.haigaiapp.cn

Java: new Thread(() -> f()).start()
来源：http://pw.shtwfgs.cn

Go:   go f()
来源：http://bq.hahajie.cn

Ruby: Thread.new { f }
来源：http://rt.huanxung.cn

C#:   Task.Run(() => F());
来源：http://et.bjjhwx.cn

[O02] 使用线程池
来源：http://fa.gzmigu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lb.9csxet.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://an.jctech888.com.cn

JS:   // worker_threads 线程池
来源：http://ob.yuexingan06.cn

TS:   // worker_threads 线程池
来源：http://ke.szxytkj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://oh.yuexingan06.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ir.gzmigu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://pb.haigaiapp.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zl.hahajie.cn

[O03] 加锁保护共享数据
来源：http://kt.chemitech.net.cn

Py:   with lock: shared += 1
来源：http://vn.shxzukj.cn

PHP:  // 用 flock() 做文件锁
来源：http://bz.newstarts.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://kk.nszjky.cn

TS:   // 同 JS
来源：http://xf.nszjky.cn

Java: synchronized (this) { shared++; }
来源：http://zp.huanxung.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hu.shxzukj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://yz.521024.cn

C#:   lock (gate) { shared++; }
来源：http://my.szsharing.cn

[O04] 定义异步函数并等待
来源：http://od.chemitech.net.cn

Py:   async def f():⏎    await g()
来源：http://xs.chemitech.net.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gp.nicolike.cn

JS:   async function f() { await g(); }
来源：http://fb.huixinmuqiang.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://pi.hnjuh.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://bz.shtwfgs.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kn.bookmarksfly.cn

Ruby: # 用 Fiber 或 async gem
来源：http://hd.szsharing.cn

C#:   async Task F() { await G(); }
来源：http://eb.nszjky.cn

[O05] 并发执行并等待全部完成
来源：http://ha.yuntaijiaju.cn

Py:   asyncio.gather(*tasks)
来源：http://uq.newstarts.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fc.asd995.cn

JS:   await Promise.all(tasks)
来源：http://pu.newstarts.cn

TS:   await Promise.all(tasks)
来源：http://tv.jianghongdianzi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://as.jctech888.com.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hh.huixinmuqiang.cn

Ruby: threads.map(&:join)
来源：http://gh.muxihuayi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://zl.lnxyls.cn

[O06] 使用进程池
来源：http://gg.huixinmuqiang.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ab.9csxet.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://js.haigaiapp.cn

JS:   // child_process / cluster 模块
来源：http://oo.huixiangedu.cn

TS:   // child_process / cluster 模块
来源：http://zz.huanxung.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://iu.muxihuayi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vp.huixiangedu.cn

Ruby: // fork 块
来源：http://qx.shxzskj.cn

C#:   Parallel.For
来源：http://eh.shtwfgs.cn

================================================================================
来源：http://ab.521024.cn

P. 常用工具函数
来源：http://qh.szxytkj.cn

================================================================================
来源：http://lb.haigaiapp.cn

[P01] 生成 UUID
来源：http://yb.hahajie.cn

Py:   str(uuid.uuid4())
来源：http://qx.newstarts.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://aq.yuexingan06.cn

JS:   crypto.randomUUID()
来源：http://ao.panjiajie.cn

TS:   crypto.randomUUID()
来源：http://kl.shxzukj.cn

Java: UUID.randomUUID().toString()
来源：http://tm.newstarts.cn

Go:   // 用 github.com/google/uuid
来源：http://zc.nicolike.cn

Ruby: SecureRandom.uuid
来源：http://up.bookmarksfly.cn

C#:   Guid.NewGuid().ToString()
来源：http://iw.asd995.cn

[P02] MD5 / SHA256 摘要
来源：http://rk.muxihuayi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://cb.shtwfgs.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ek.yuexingan06.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dp.shxzukj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://uw.nszjky.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hg.521024.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hq.shxzskj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://nt.colortex.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://pr.lnxyls.cn

[P03] 生成短随机字符串
来源：http://qn.newstarts.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ao.haigaiapp.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://cg.chemitech.net.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://po.shtwfgs.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xg.huixinmuqiang.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ll.lnxyls.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tt.yuexingan06.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://oj.shtwfgs.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://em.9csxet.cn

[P04] 求长度
来源：http://zh.newstarts.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hd.hahajie.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ra.gzmigu.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wp.huixiangedu.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ot.yuexingan06.cn

Java: list.size();  map.size();  s.length()
来源：http://aa.shxzskj.cn

Go:   len(arr);  len(m)
来源：http://zg.bjjhwx.cn

Ruby: x.length;  x.size
来源：http://ss.521024.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://fu.newstarts.cn

[P05] 判断两个对象内容是否相等
来源：http://uh.muxihuayi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://jp.hnjuh.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rq.huixinmuqiang.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://dn.chemitech.net.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wj.yuexingan06.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ty.yuexingan06.cn

Go:   reflect.DeepEqual(a, b)
来源：http://xp.jctech888.com.cn

Ruby: a == b
来源：http://kv.haigaiapp.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tu.haigaiapp.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://uy.9csxet.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ss.huixiangedu.cn

PHP:  if (empty($x)) {}
来源：http://jp.jianghongdianzi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://oo.yuntaijiaju.cn

TS:   if (x == null) {}
来源：http://dz.panjiajie.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ps.huixinmuqiang.cn

Go:   if x == nil {}
来源：http://uj.wgjwhj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://yb.huanxung.cn

C#:   if (x is null) {}
来源：http://if.muxihuayi.cn

[P07] 防抖与节流
来源：http://mh.bookmarksfly.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://tq.nszjky.cn

PHP:  // 手写时间戳比较
来源：http://rc.gzmigu.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ko.lnxyls.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dh.jianghongdianzi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mb.bjjhwx.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fb.huanxung.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://uq.jctech888.com.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://nk.lnxyls.cn

[P08] 处理浮点精度问题
来源：http://cz.shxzukj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wy.521024.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://yi.hahajie.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pf.szsharing.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://cj.panjiajie.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://oc.chemitech.net.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cj.muxihuayi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://bc.huanxung.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fv.yuntaijiaju.cn

================================================================================
来源：http://sm.lnxyls.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hp.yuntaijiaju.cn

================================================================================
来源：http://gu.newstarts.cn

[Q01] 创建表
来源：http://vu.shxzukj.cn

CREATE TABLE users (
来源：http://np.yuntaijiaju.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jh.shxzukj.cn

name VARCHAR(50) NOT NULL,
来源：http://lp.chemitech.net.cn

email VARCHAR(100) UNIQUE,
来源：http://em.wgjwhj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bp.9csxet.cn

);
来源：http://ja.szsharing.cn

[Q02] 创建带外键的表
来源：http://rz.szxytkj.cn

CREATE TABLE orders (
来源：http://od.szsharing.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wj.shtwfgs.cn

user_id INT NOT NULL,
来源：http://uq.yuntaijiaju.cn

amount DECIMAL(10, 2),
来源：http://il.yuexingan06.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://gx.szsharing.cn

);
来源：http://we.bookmarksfly.cn

[Q03] 增加列
来源：http://ng.muxihuayi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gh.hnjuh.cn

[Q04] 修改列类型
来源：http://gl.muxihuayi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ov.yuntaijiaju.cn

[Q05] 重命名列
来源：http://zf.yuexingan06.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dh.521024.cn

[Q06] 删除列
来源：http://bk.newstarts.cn

ALTER TABLE users DROP COLUMN age;
来源：http://xb.nicolike.cn

[Q07] 删除表
来源：http://dn.colortex.cn

DROP TABLE IF EXISTS orders;
来源：http://ia.colortex.cn

[Q08] 创建普通索引
来源：http://bn.haigaiapp.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://vr.chemitech.net.cn

[Q09] 创建唯一索引
来源：http://xk.lnxyls.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://tp.newstarts.cn

[Q10] 插入单行
来源：http://ov.huixiangedu.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://us.jianghongdianzi.cn

[Q11] 一次插入多行
来源：http://ff.bookmarksfly.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ja.szsharing.cn

[Q12] 插入后取自增 ID
来源：http://lc.shxzukj.cn

INSERT INTO users (name) VALUES ('C');
来源：http://cr.hnjuh.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://is.shxzukj.cn

[Q13] 忽略重复插入
来源：http://bz.szxytkj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ud.szsharing.cn

[Q14] 存在则更新（upsert）
来源：http://kj.szxytkj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xq.haigaiapp.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://sg.haigaiapp.cn

[Q15] 查询全部
来源：http://uk.521024.cn

SELECT * FROM users;
来源：http://pd.huixinmuqiang.cn

[Q16] 查询指定列
来源：http://yl.wgjwhj.cn

SELECT id, name FROM users;
来源：http://mj.shxzukj.cn

[Q17] 条件查询
来源：http://th.panjiajie.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ct.colortex.cn

[Q18] 模糊匹配
来源：http://vd.shtwfgs.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://er.panjiajie.cn

[Q19] 范围查询
来源：http://lj.newstarts.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://fe.jianghongdianzi.cn

[Q20] IN 列表
来源：http://ei.szsharing.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wj.9csxet.cn

[Q21] 空值判断
来源：http://wy.shtwfgs.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://te.jctech888.com.cn

[Q22] 排序
来源：http://sx.yuntaijiaju.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gl.newstarts.cn

[Q23] 分页
来源：http://xu.wgjwhj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lq.hahajie.cn

[Q24] 去重
来源：http://at.bookmarksfly.cn

SELECT DISTINCT city FROM users;
来源：http://bu.hahajie.cn

[Q25] 只取前 N 条
来源：http://is.shtwfgs.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ay.wgjwhj.cn

[Q26] 计数
来源：http://cp.shxzukj.cn

SELECT COUNT(*) FROM users;
来源：http://cl.huanxung.cn

[Q27] 条件计数
来源：http://cu.szxytkj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fz.yuntaijiaju.cn

[Q28] 求和与平均
来源：http://xe.hahajie.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://uf.gzmigu.cn

[Q29] 最大最小值
来源：http://hv.bookmarksfly.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://eo.panjiajie.cn

[Q30] 分组统计
来源：http://va.huanxung.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hf.hnjuh.cn

[Q31] 分组后过滤
来源：http://vo.shxzukj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kt.hahajie.cn

[Q32] 分组拼接字符串
来源：http://nh.panjiajie.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ab.lnxyls.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ed.szsharing.cn

[Q33] 多列分组
来源：http://dx.521024.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://db.gzmigu.cn

[Q34] 每组取第一条
来源：http://ss.haigaiapp.cn

SELECT * FROM (
来源：http://cv.muxihuayi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://kp.9csxet.cn

) t WHERE rn = 1;
来源：http://bv.colortex.cn

[Q35] 内连接
来源：http://ot.colortex.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vo.shxzskj.cn

[Q36] 左连接
来源：http://qi.gzmigu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://au.9csxet.cn

[Q37] 右连接
来源：http://qv.colortex.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://li.hahajie.cn

[Q38] 全外连接（PostgreSQL）
来源：http://zs.szxytkj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ul.haigaiapp.cn

[Q39] 自连接（查上下级）
来源：http://lq.asd995.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://gn.nszjky.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://it.hahajie.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://rp.panjiajie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bs.jctech888.com.cn

[Q41] 多表连接
来源：http://yt.9csxet.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://pq.bookmarksfly.cn

JOIN users u ON u.id = o.user_id
来源：http://dl.panjiajie.cn

JOIN products p ON p.id = o.product_id;
来源：http://hi.nicolike.cn

[Q42] 连接条件附加过滤
来源：http://ei.gzmigu.cn


<!-- 参考信息 -->