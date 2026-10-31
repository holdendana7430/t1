代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bd.nszjky.cn

[N06] 判断回文字符串
来源：http://yq.huixinmuqiang.cn

Py:   s == s[::-1]
来源：http://pn.shtwfgs.cn

PHP:  $s === strrev($s);
来源：http://qp.shxzskj.cn

JS:   s === [...s].reverse().join("")
来源：http://zc.haigaiapp.cn

TS:   s === [...s].reverse().join("")
来源：http://jl.nszjky.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wl.jianghongdianzi.cn

Go:   // 双指针从两端比较
来源：http://bm.bjjhwx.cn

Ruby: s == s.reverse
来源：http://tp.jianghongdianzi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://go.huanxung.cn

[N07] 两数之和（返回下标）
来源：http://je.bjjhwx.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://om.shtwfgs.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wl.hnjuh.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://tl.9csxet.cn

TS:   // 手写 Map<string, number>
来源：http://js.9csxet.cn

Java: // 手写 HashMap
来源：http://fw.yuexingan06.cn

Go:   // 手写 map[int]int
来源：http://ud.hnjuh.cn

Ruby: // 手写 Hash
来源：http://bb.panjiajie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://xm.huixiangedu.cn

[N08] 生成全排列
来源：http://gp.yuntaijiaju.cn

Py:   itertools.permutations(arr)
来源：http://wi.huanxung.cn

PHP:  // 手写递归交换
来源：http://ja.hnjuh.cn

JS:   // 手写回溯递归
来源：http://kr.asd995.cn

TS:   // 手写回溯递归
来源：http://te.gzmigu.cn

Java: // 手写回溯递归
来源：http://xt.newstarts.cn

Go:   // 手写回溯递归
来源：http://ho.nicolike.cn

Ruby: arr.permutation.to_a
来源：http://ls.muxihuayi.cn

C#:   // 手写回溯递归
来源：http://jv.gzmigu.cn

[N09] 栈与队列
来源：http://lq.szsharing.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ui.521024.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qd.nszjky.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jk.huixinmuqiang.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://lv.szxytkj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fy.shxzskj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wi.yuntaijiaju.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ct.nszjky.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gm.yuntaijiaju.cn

[N10] 链表节点定义
来源：http://ei.panjiajie.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gl.9csxet.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://gt.lnxyls.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wf.shxzskj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://od.nszjky.cn

Java: class Node { int v; Node next; }
来源：http://gz.shtwfgs.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ky.newstarts.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://xt.shtwfgs.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://cb.bjjhwx.cn

[N11] 二叉树中序遍历
来源：http://dd.yuntaijiaju.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://sk.asd995.cn

PHP:  // 手写递归函数
来源：http://bi.bjjhwx.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ag.bookmarksfly.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://di.hnjuh.cn

Java: // 手写递归
来源：http://ix.bjjhwx.cn

Go:   // 手写递归
来源：http://ay.bookmarksfly.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ep.huanxung.cn

C#:   // 手写递归
来源：http://fx.nicolike.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ta.hnjuh.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ha.szxytkj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gm.newstarts.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fu.szxytkj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yq.newstarts.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://gz.hahajie.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pj.szxytkj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lg.521024.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://gp.asd995.cn

================================================================================
来源：http://bx.newstarts.cn

O. 并发与异步
来源：http://hm.gzmigu.cn

================================================================================
来源：http://zf.nicolike.cn

[O01] 启动一个线程
来源：http://qz.wgjwhj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://za.chemitech.net.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://uq.nicolike.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yx.colortex.cn

TS:   // 同 JS
来源：http://rs.haigaiapp.cn

Java: new Thread(() -> f()).start()
来源：http://cn.asd995.cn

Go:   go f()
来源：http://om.szsharing.cn

Ruby: Thread.new { f }
来源：http://hw.huixiangedu.cn

C#:   Task.Run(() => F());
来源：http://tt.asd995.cn

[O02] 使用线程池
来源：http://qd.lnxyls.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fg.yuntaijiaju.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kh.muxihuayi.cn

JS:   // worker_threads 线程池
来源：http://td.chemitech.net.cn

TS:   // worker_threads 线程池
来源：http://rh.yuexingan06.cn

Java: Executors.newFixedThreadPool(4)
来源：http://cx.yuexingan06.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://sr.hahajie.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ib.yuexingan06.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ee.yuexingan06.cn

[O03] 加锁保护共享数据
来源：http://sn.newstarts.cn

Py:   with lock: shared += 1
来源：http://uj.gzmigu.cn

PHP:  // 用 flock() 做文件锁
来源：http://ug.bjjhwx.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://us.bjjhwx.cn

TS:   // 同 JS
来源：http://mz.yuexingan06.cn

Java: synchronized (this) { shared++; }
来源：http://vl.bjjhwx.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wn.panjiajie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://dy.huixiangedu.cn

C#:   lock (gate) { shared++; }
来源：http://vs.szxytkj.cn

[O04] 定义异步函数并等待
来源：http://gf.yuntaijiaju.cn

Py:   async def f():⏎    await g()
来源：http://eb.nszjky.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zh.huixinmuqiang.cn

JS:   async function f() { await g(); }
来源：http://kg.panjiajie.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://rm.wgjwhj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ep.bjjhwx.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qe.nszjky.cn

Ruby: # 用 Fiber 或 async gem
来源：http://qt.muxihuayi.cn

C#:   async Task F() { await G(); }
来源：http://tk.asd995.cn

[O05] 并发执行并等待全部完成
来源：http://xc.shtwfgs.cn

Py:   asyncio.gather(*tasks)
来源：http://pl.nszjky.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fk.szxytkj.cn

JS:   await Promise.all(tasks)
来源：http://tl.szxytkj.cn

TS:   await Promise.all(tasks)
来源：http://pa.nszjky.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://oj.bjjhwx.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rc.hahajie.cn

Ruby: threads.map(&:join)
来源：http://uq.shtwfgs.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://bi.jctech888.com.cn

[O06] 使用进程池
来源：http://ad.huixiangedu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://va.newstarts.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://yv.nszjky.cn

JS:   // child_process / cluster 模块
来源：http://is.gzmigu.cn

TS:   // child_process / cluster 模块
来源：http://ed.chemitech.net.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hb.yuexingan06.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ra.szsharing.cn

Ruby: // fork 块
来源：http://lm.huanxung.cn

C#:   Parallel.For
来源：http://vt.shxzskj.cn

================================================================================
来源：http://gj.9csxet.cn

P. 常用工具函数
来源：http://xa.hnjuh.cn

================================================================================
来源：http://lz.wgjwhj.cn

[P01] 生成 UUID
来源：http://wc.muxihuayi.cn

Py:   str(uuid.uuid4())
来源：http://wt.muxihuayi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://uh.asd995.cn

JS:   crypto.randomUUID()
来源：http://fj.jianghongdianzi.cn

TS:   crypto.randomUUID()
来源：http://er.panjiajie.cn

Java: UUID.randomUUID().toString()
来源：http://ry.nicolike.cn

Go:   // 用 github.com/google/uuid
来源：http://qc.shxzskj.cn

Ruby: SecureRandom.uuid
来源：http://sa.huanxung.cn

C#:   Guid.NewGuid().ToString()
来源：http://bq.nicolike.cn

[P02] MD5 / SHA256 摘要
来源：http://yo.nicolike.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vz.newstarts.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://tm.lnxyls.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://kn.yuexingan06.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xw.huanxung.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://aw.huixiangedu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ez.asd995.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kq.huanxung.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mo.bjjhwx.cn

[P03] 生成短随机字符串
来源：http://mv.shxzukj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ht.9csxet.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mp.lnxyls.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qr.jianghongdianzi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nn.panjiajie.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://cy.colortex.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://yc.panjiajie.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://pa.jctech888.com.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://uk.yuntaijiaju.cn

[P04] 求长度
来源：http://an.newstarts.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://en.shxzskj.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lq.jctech888.com.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ez.yuntaijiaju.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bz.huixinmuqiang.cn

Java: list.size();  map.size();  s.length()
来源：http://eu.colortex.cn

Go:   len(arr);  len(m)
来源：http://nk.yuntaijiaju.cn

Ruby: x.length;  x.size
来源：http://ph.shxzukj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ey.szsharing.cn

[P05] 判断两个对象内容是否相等
来源：http://xb.lnxyls.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://xl.asd995.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rk.muxihuayi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://yu.newstarts.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bq.521024.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zk.colortex.cn

Go:   reflect.DeepEqual(a, b)
来源：http://je.newstarts.cn

Ruby: a == b
来源：http://nf.shxzukj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dj.lnxyls.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://pp.hahajie.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://bu.bookmarksfly.cn

PHP:  if (empty($x)) {}
来源：http://mm.szxytkj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zr.bjjhwx.cn

TS:   if (x == null) {}
来源：http://fv.hnjuh.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://lx.lnxyls.cn

Go:   if x == nil {}
来源：http://rv.huanxung.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://cw.newstarts.cn

C#:   if (x is null) {}
来源：http://sy.nicolike.cn

[P07] 防抖与节流
来源：http://hn.hahajie.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vr.wgjwhj.cn

PHP:  // 手写时间戳比较
来源：http://cl.huanxung.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iw.colortex.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oy.asd995.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qb.bookmarksfly.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://sq.bookmarksfly.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://fz.szsharing.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vx.gzmigu.cn

[P08] 处理浮点精度问题
来源：http://ed.lnxyls.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ez.hahajie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xf.shtwfgs.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mh.szxytkj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hp.hnjuh.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://jj.huixinmuqiang.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ah.yuntaijiaju.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jw.huixiangedu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://sv.huixinmuqiang.cn

================================================================================
来源：http://sb.huanxung.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ed.colortex.cn

================================================================================
来源：http://wp.huixinmuqiang.cn

[Q01] 创建表
来源：http://lx.bjjhwx.cn

CREATE TABLE users (
来源：http://mb.szxytkj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mg.newstarts.cn

name VARCHAR(50) NOT NULL,
来源：http://lk.muxihuayi.cn

email VARCHAR(100) UNIQUE,
来源：http://jm.huanxung.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ja.chemitech.net.cn

);
来源：http://jl.huixiangedu.cn

[Q02] 创建带外键的表
来源：http://bp.jianghongdianzi.cn

CREATE TABLE orders (
来源：http://kw.szsharing.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://uz.nszjky.cn

user_id INT NOT NULL,
来源：http://lc.wgjwhj.cn

amount DECIMAL(10, 2),
来源：http://da.hahajie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://pq.colortex.cn

);
来源：http://ig.muxihuayi.cn

[Q03] 增加列
来源：http://pg.szxytkj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rv.lnxyls.cn

[Q04] 修改列类型
来源：http://dp.gzmigu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://sa.hnjuh.cn

[Q05] 重命名列
来源：http://em.521024.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ys.huixinmuqiang.cn

[Q06] 删除列
来源：http://lg.panjiajie.cn

ALTER TABLE users DROP COLUMN age;
来源：http://vh.gzmigu.cn

[Q07] 删除表
来源：http://tq.szxytkj.cn

DROP TABLE IF EXISTS orders;
来源：http://fp.jianghongdianzi.cn

[Q08] 创建普通索引
来源：http://xf.jctech888.com.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://zw.asd995.cn

[Q09] 创建唯一索引
来源：http://um.chemitech.net.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xl.huixiangedu.cn

[Q10] 插入单行
来源：http://qr.shxzskj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gf.gzmigu.cn

[Q11] 一次插入多行
来源：http://oj.521024.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qd.shtwfgs.cn

[Q12] 插入后取自增 ID
来源：http://gl.hnjuh.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ix.nicolike.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mz.huixinmuqiang.cn

[Q13] 忽略重复插入
来源：http://bz.szsharing.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zq.bjjhwx.cn

[Q14] 存在则更新（upsert）
来源：http://gw.newstarts.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://cd.huixinmuqiang.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ru.colortex.cn

[Q15] 查询全部
来源：http://gi.gzmigu.cn

SELECT * FROM users;
来源：http://hq.shxzukj.cn

[Q16] 查询指定列
来源：http://we.yuntaijiaju.cn

SELECT id, name FROM users;
来源：http://yh.huixiangedu.cn

[Q17] 条件查询
来源：http://wb.nicolike.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://op.hahajie.cn

[Q18] 模糊匹配
来源：http://kq.szsharing.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qm.bookmarksfly.cn

[Q19] 范围查询
来源：http://po.lnxyls.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lm.colortex.cn

[Q20] IN 列表
来源：http://zz.szsharing.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ry.panjiajie.cn

[Q21] 空值判断
来源：http://kt.521024.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://vq.lnxyls.cn

[Q22] 排序
来源：http://zy.nszjky.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ar.wgjwhj.cn

[Q23] 分页
来源：http://fw.wgjwhj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://re.haigaiapp.cn

[Q24] 去重
来源：http://jg.lnxyls.cn

SELECT DISTINCT city FROM users;
来源：http://vm.yuntaijiaju.cn

[Q25] 只取前 N 条
来源：http://aq.szsharing.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ws.wgjwhj.cn

[Q26] 计数
来源：http://ma.yuexingan06.cn

SELECT COUNT(*) FROM users;
来源：http://ew.bookmarksfly.cn

[Q27] 条件计数
来源：http://rf.lnxyls.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vi.lnxyls.cn

[Q28] 求和与平均
来源：http://vq.muxihuayi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://pg.haigaiapp.cn

[Q29] 最大最小值
来源：http://if.panjiajie.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://nt.szsharing.cn

[Q30] 分组统计
来源：http://ya.nszjky.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://jf.yuexingan06.cn

[Q31] 分组后过滤
来源：http://xw.panjiajie.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ci.chemitech.net.cn

[Q32] 分组拼接字符串
来源：http://ns.yuexingan06.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://yc.asd995.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fe.huixinmuqiang.cn

[Q33] 多列分组
来源：http://zv.huixinmuqiang.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ct.szsharing.cn

[Q34] 每组取第一条
来源：http://yv.panjiajie.cn

SELECT * FROM (
来源：http://hd.jctech888.com.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bs.newstarts.cn

) t WHERE rn = 1;
来源：http://wx.newstarts.cn

[Q35] 内连接
来源：http://oh.jctech888.com.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ys.hnjuh.cn

[Q36] 左连接
来源：http://vf.chemitech.net.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bb.colortex.cn

[Q37] 右连接
来源：http://jo.asd995.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://sw.chemitech.net.cn

[Q38] 全外连接（PostgreSQL）
来源：http://tv.shtwfgs.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qt.9csxet.cn

[Q39] 自连接（查上下级）
来源：http://ko.9csxet.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://uy.huixiangedu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://az.jctech888.com.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://qh.nicolike.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jf.lnxyls.cn

[Q41] 多表连接
来源：http://bx.gzmigu.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://rz.yuexingan06.cn

JOIN users u ON u.id = o.user_id
来源：http://ee.haigaiapp.cn

JOIN products p ON p.id = o.product_id;
来源：http://eu.shxzskj.cn

[Q42] 连接条件附加过滤
来源：http://kr.lnxyls.cn


<!-- 参考信息 -->