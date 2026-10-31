代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vt.newstarts.cn

[N06] 判断回文字符串
来源：http://hr.521024.cn

Py:   s == s[::-1]
来源：http://xd.shxzukj.cn

PHP:  $s === strrev($s);
来源：http://la.jianghongdianzi.cn

JS:   s === [...s].reverse().join("")
来源：http://ye.521024.cn

TS:   s === [...s].reverse().join("")
来源：http://en.muxihuayi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xw.521024.cn

Go:   // 双指针从两端比较
来源：http://ds.huixiangedu.cn

Ruby: s == s.reverse
来源：http://rf.hahajie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://al.chemitech.net.cn

[N07] 两数之和（返回下标）
来源：http://xa.nszjky.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ve.bookmarksfly.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hk.chemitech.net.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ue.asd995.cn

TS:   // 手写 Map<string, number>
来源：http://nz.chemitech.net.cn

Java: // 手写 HashMap
来源：http://dz.jctech888.com.cn

Go:   // 手写 map[int]int
来源：http://gy.huixiangedu.cn

Ruby: // 手写 Hash
来源：http://sa.shxzskj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://cy.jctech888.com.cn

[N08] 生成全排列
来源：http://re.shxzukj.cn

Py:   itertools.permutations(arr)
来源：http://to.szxytkj.cn

PHP:  // 手写递归交换
来源：http://qr.shxzukj.cn

JS:   // 手写回溯递归
来源：http://wv.hnjuh.cn

TS:   // 手写回溯递归
来源：http://ct.gzmigu.cn

Java: // 手写回溯递归
来源：http://xb.shxzskj.cn

Go:   // 手写回溯递归
来源：http://sb.yuexingan06.cn

Ruby: arr.permutation.to_a
来源：http://iw.shxzukj.cn

C#:   // 手写回溯递归
来源：http://gp.wgjwhj.cn

[N09] 栈与队列
来源：http://yx.jianghongdianzi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qk.huanxung.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ud.hahajie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://di.huixiangedu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://da.jctech888.com.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wz.chemitech.net.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ji.521024.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fr.hnjuh.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://db.szsharing.cn

[N10] 链表节点定义
来源：http://sm.wgjwhj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qc.shtwfgs.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://xg.szsharing.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xt.panjiajie.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://yo.nicolike.cn

Java: class Node { int v; Node next; }
来源：http://iv.nicolike.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ea.jctech888.com.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://fz.jianghongdianzi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ad.huixiangedu.cn

[N11] 二叉树中序遍历
来源：http://xm.szxytkj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://yo.huixiangedu.cn

PHP:  // 手写递归函数
来源：http://ok.521024.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wg.shtwfgs.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mx.jctech888.com.cn

Java: // 手写递归
来源：http://pw.lnxyls.cn

Go:   // 手写递归
来源：http://cr.hahajie.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fa.hahajie.cn

C#:   // 手写递归
来源：http://cn.newstarts.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://si.huixiangedu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tp.shxzskj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lk.muxihuayi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dh.asd995.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xa.521024.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ub.bjjhwx.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xd.lnxyls.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ya.yuntaijiaju.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ap.muxihuayi.cn

================================================================================
来源：http://on.shtwfgs.cn

O. 并发与异步
来源：http://hu.shxzskj.cn

================================================================================
来源：http://dw.521024.cn

[O01] 启动一个线程
来源：http://cf.muxihuayi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vj.lnxyls.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://py.bjjhwx.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ri.gzmigu.cn

TS:   // 同 JS
来源：http://dr.szxytkj.cn

Java: new Thread(() -> f()).start()
来源：http://om.nszjky.cn

Go:   go f()
来源：http://dj.lnxyls.cn

Ruby: Thread.new { f }
来源：http://fz.huanxung.cn

C#:   Task.Run(() => F());
来源：http://qb.colortex.cn

[O02] 使用线程池
来源：http://xc.lnxyls.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ar.newstarts.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://im.szxytkj.cn

JS:   // worker_threads 线程池
来源：http://mx.nszjky.cn

TS:   // worker_threads 线程池
来源：http://nv.jianghongdianzi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://dv.nszjky.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lr.bjjhwx.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hq.shxzukj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ox.haigaiapp.cn

[O03] 加锁保护共享数据
来源：http://oh.haigaiapp.cn

Py:   with lock: shared += 1
来源：http://dt.colortex.cn

PHP:  // 用 flock() 做文件锁
来源：http://qn.yuexingan06.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://yc.huanxung.cn

TS:   // 同 JS
来源：http://ub.yuntaijiaju.cn

Java: synchronized (this) { shared++; }
来源：http://ef.521024.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gj.hnjuh.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://de.yuntaijiaju.cn

C#:   lock (gate) { shared++; }
来源：http://rj.huanxung.cn

[O04] 定义异步函数并等待
来源：http://cg.szsharing.cn

Py:   async def f():⏎    await g()
来源：http://yn.521024.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ut.newstarts.cn

JS:   async function f() { await g(); }
来源：http://se.wgjwhj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ko.jctech888.com.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ii.szxytkj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://go.nicolike.cn

Ruby: # 用 Fiber 或 async gem
来源：http://am.muxihuayi.cn

C#:   async Task F() { await G(); }
来源：http://nu.szsharing.cn

[O05] 并发执行并等待全部完成
来源：http://zf.521024.cn

Py:   asyncio.gather(*tasks)
来源：http://vb.haigaiapp.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mf.huixinmuqiang.cn

JS:   await Promise.all(tasks)
来源：http://ii.hnjuh.cn

TS:   await Promise.all(tasks)
来源：http://hj.lnxyls.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pb.wgjwhj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://oy.shxzukj.cn

Ruby: threads.map(&:join)
来源：http://hj.lnxyls.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://tc.huanxung.cn

[O06] 使用进程池
来源：http://ei.shtwfgs.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://lq.huixiangedu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://hv.chemitech.net.cn

JS:   // child_process / cluster 模块
来源：http://ft.asd995.cn

TS:   // child_process / cluster 模块
来源：http://qu.lnxyls.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://op.shxzukj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qx.9csxet.cn

Ruby: // fork 块
来源：http://cd.colortex.cn

C#:   Parallel.For
来源：http://gs.muxihuayi.cn

================================================================================
来源：http://hi.wgjwhj.cn

P. 常用工具函数
来源：http://hp.chemitech.net.cn

================================================================================
来源：http://ot.nicolike.cn

[P01] 生成 UUID
来源：http://ca.hahajie.cn

Py:   str(uuid.uuid4())
来源：http://dl.shxzskj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jg.yuexingan06.cn

JS:   crypto.randomUUID()
来源：http://kg.jctech888.com.cn

TS:   crypto.randomUUID()
来源：http://wy.lnxyls.cn

Java: UUID.randomUUID().toString()
来源：http://nf.hahajie.cn

Go:   // 用 github.com/google/uuid
来源：http://it.9csxet.cn

Ruby: SecureRandom.uuid
来源：http://yi.muxihuayi.cn

C#:   Guid.NewGuid().ToString()
来源：http://od.yuexingan06.cn

[P02] MD5 / SHA256 摘要
来源：http://pp.jianghongdianzi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xp.newstarts.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ig.haigaiapp.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://cx.muxihuayi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://pm.jianghongdianzi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bv.szxytkj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cx.nicolike.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://nl.szxytkj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://sr.asd995.cn

[P03] 生成短随机字符串
来源：http://kf.shxzskj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qz.shxzukj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jb.asd995.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nn.huixinmuqiang.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ld.panjiajie.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://iz.521024.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pc.gzmigu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://iu.bjjhwx.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vw.hahajie.cn

[P04] 求长度
来源：http://rn.nszjky.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ve.bookmarksfly.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zd.huixiangedu.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wv.shxzskj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fj.bookmarksfly.cn

Java: list.size();  map.size();  s.length()
来源：http://gn.szsharing.cn

Go:   len(arr);  len(m)
来源：http://jb.yuntaijiaju.cn

Ruby: x.length;  x.size
来源：http://xb.shxzukj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://wm.9csxet.cn

[P05] 判断两个对象内容是否相等
来源：http://su.huixinmuqiang.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://cw.muxihuayi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hy.huixinmuqiang.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ci.yuexingan06.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ec.lnxyls.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fe.huanxung.cn

Go:   reflect.DeepEqual(a, b)
来源：http://pk.huixiangedu.cn

Ruby: a == b
来源：http://sv.shxzukj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gg.hahajie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://fg.yuexingan06.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.shtwfgs.cn

PHP:  if (empty($x)) {}
来源：http://pl.huixinmuqiang.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xw.hahajie.cn

TS:   if (x == null) {}
来源：http://dc.jianghongdianzi.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://kj.nszjky.cn

Go:   if x == nil {}
来源：http://vn.gzmigu.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://yh.yuntaijiaju.cn

C#:   if (x is null) {}
来源：http://lh.shxzskj.cn

[P07] 防抖与节流
来源：http://ux.szsharing.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gk.huixiangedu.cn

PHP:  // 手写时间戳比较
来源：http://wa.huixiangedu.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xo.haigaiapp.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cj.bjjhwx.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://gi.muxihuayi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://sl.yuntaijiaju.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://em.newstarts.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://qb.bookmarksfly.cn

[P08] 处理浮点精度问题
来源：http://ek.wgjwhj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://bo.shtwfgs.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kg.muxihuayi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gn.szsharing.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qy.yuntaijiaju.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://sb.bookmarksfly.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://lt.shtwfgs.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fq.hnjuh.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gc.shxzukj.cn

================================================================================
来源：http://om.newstarts.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ep.hnjuh.cn

================================================================================
来源：http://wh.nicolike.cn

[Q01] 创建表
来源：http://ih.huixiangedu.cn

CREATE TABLE users (
来源：http://kz.haigaiapp.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://of.9csxet.cn

name VARCHAR(50) NOT NULL,
来源：http://zb.hnjuh.cn

email VARCHAR(100) UNIQUE,
来源：http://wb.huanxung.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rf.wgjwhj.cn

);
来源：http://db.shxzskj.cn

[Q02] 创建带外键的表
来源：http://dm.yuntaijiaju.cn

CREATE TABLE orders (
来源：http://df.wgjwhj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mo.yuexingan06.cn

user_id INT NOT NULL,
来源：http://go.szsharing.cn

amount DECIMAL(10, 2),
来源：http://gs.lnxyls.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://pa.newstarts.cn

);
来源：http://tj.9csxet.cn

[Q03] 增加列
来源：http://yx.colortex.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ag.bjjhwx.cn

[Q04] 修改列类型
来源：http://lw.shxzskj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xn.yuntaijiaju.cn

[Q05] 重命名列
来源：http://td.521024.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vs.chemitech.net.cn

[Q06] 删除列
来源：http://uz.wgjwhj.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ru.chemitech.net.cn

[Q07] 删除表
来源：http://ma.huanxung.cn

DROP TABLE IF EXISTS orders;
来源：http://qo.shtwfgs.cn

[Q08] 创建普通索引
来源：http://ya.lnxyls.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://iy.shtwfgs.cn

[Q09] 创建唯一索引
来源：http://as.jianghongdianzi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gj.chemitech.net.cn

[Q10] 插入单行
来源：http://xd.huanxung.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ee.hahajie.cn

[Q11] 一次插入多行
来源：http://pp.yuexingan06.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hu.lnxyls.cn

[Q12] 插入后取自增 ID
来源：http://yy.gzmigu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ou.szxytkj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ao.yuexingan06.cn

[Q13] 忽略重复插入
来源：http://hd.jctech888.com.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://me.bookmarksfly.cn

[Q14] 存在则更新（upsert）
来源：http://qo.colortex.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://op.haigaiapp.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kx.shxzskj.cn

[Q15] 查询全部
来源：http://qn.huixiangedu.cn

SELECT * FROM users;
来源：http://zy.asd995.cn

[Q16] 查询指定列
来源：http://zu.huixiangedu.cn

SELECT id, name FROM users;
来源：http://mv.yuntaijiaju.cn

[Q17] 条件查询
来源：http://py.szxytkj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mi.asd995.cn

[Q18] 模糊匹配
来源：http://mm.nszjky.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vj.chemitech.net.cn

[Q19] 范围查询
来源：http://ta.bjjhwx.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pp.yuexingan06.cn

[Q20] IN 列表
来源：http://po.szxytkj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://aj.newstarts.cn

[Q21] 空值判断
来源：http://ux.yuexingan06.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ly.shxzukj.cn

[Q22] 排序
来源：http://xy.shxzskj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ca.huixinmuqiang.cn

[Q23] 分页
来源：http://gr.jianghongdianzi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://cs.jianghongdianzi.cn

[Q24] 去重
来源：http://id.bookmarksfly.cn

SELECT DISTINCT city FROM users;
来源：http://ia.jianghongdianzi.cn

[Q25] 只取前 N 条
来源：http://lj.bookmarksfly.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://at.asd995.cn

[Q26] 计数
来源：http://qa.9csxet.cn

SELECT COUNT(*) FROM users;
来源：http://ry.hnjuh.cn

[Q27] 条件计数
来源：http://lf.huanxung.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://lr.521024.cn

[Q28] 求和与平均
来源：http://mt.muxihuayi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ab.nszjky.cn

[Q29] 最大最小值
来源：http://wn.yuexingan06.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://mg.asd995.cn

[Q30] 分组统计
来源：http://ko.huixiangedu.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://jp.lnxyls.cn

[Q31] 分组后过滤
来源：http://qi.huixiangedu.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://uu.nicolike.cn

[Q32] 分组拼接字符串
来源：http://rv.9csxet.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ca.chemitech.net.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vz.colortex.cn

[Q33] 多列分组
来源：http://ec.colortex.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ab.nicolike.cn

[Q34] 每组取第一条
来源：http://pn.huixinmuqiang.cn

SELECT * FROM (
来源：http://yg.szsharing.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mr.asd995.cn

) t WHERE rn = 1;
来源：http://gs.521024.cn

[Q35] 内连接
来源：http://uf.gzmigu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://db.muxihuayi.cn

[Q36] 左连接
来源：http://jb.shtwfgs.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vw.wgjwhj.cn

[Q37] 右连接
来源：http://vj.shxzukj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ff.gzmigu.cn

[Q38] 全外连接（PostgreSQL）
来源：http://qz.haigaiapp.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://tf.jianghongdianzi.cn

[Q39] 自连接（查上下级）
来源：http://yq.haigaiapp.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://kf.szxytkj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vx.bookmarksfly.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://bg.yuexingan06.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://np.huanxung.cn

[Q41] 多表连接
来源：http://zy.hnjuh.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://on.panjiajie.cn

JOIN users u ON u.id = o.user_id
来源：http://qx.szsharing.cn

JOIN products p ON p.id = o.product_id;
来源：http://qd.yuntaijiaju.cn

[Q42] 连接条件附加过滤
来源：http://ni.szxytkj.cn


<!-- 参考信息 -->