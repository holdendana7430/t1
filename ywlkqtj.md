代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kv.gzmigu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://iq.colortex.cn

TS:   // 手写 Map<string, number>
来源：http://au.colortex.cn

Java: // 手写 HashMap
来源：http://ts.gzmigu.cn

Go:   // 手写 map[int]int
来源：http://zt.jctech888.com.cn

Ruby: // 手写 Hash
来源：http://yd.szxytkj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://wm.haigaiapp.cn

[N08] 生成全排列
来源：http://oc.521024.cn

Py:   itertools.permutations(arr)
来源：http://ex.wgjwhj.cn

PHP:  // 手写递归交换
来源：http://pf.bookmarksfly.cn

JS:   // 手写回溯递归
来源：http://hx.huixinmuqiang.cn

TS:   // 手写回溯递归
来源：http://vr.shxzukj.cn

Java: // 手写回溯递归
来源：http://rq.shxzukj.cn

Go:   // 手写回溯递归
来源：http://xd.wgjwhj.cn

Ruby: arr.permutation.to_a
来源：http://uj.muxihuayi.cn

C#:   // 手写回溯递归
来源：http://jw.hahajie.cn

[N09] 栈与队列
来源：http://iv.panjiajie.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gh.chemitech.net.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fw.panjiajie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jx.shtwfgs.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ra.panjiajie.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xr.chemitech.net.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xh.wgjwhj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gr.hnjuh.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qc.szsharing.cn

[N10] 链表节点定义
来源：http://uy.9csxet.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://il.asd995.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://rq.yuntaijiaju.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://la.bookmarksfly.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ac.shxzskj.cn

Java: class Node { int v; Node next; }
来源：http://qm.nicolike.cn

Go:   type Node struct { V int; Next *Node }
来源：http://cb.jctech888.com.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://be.hnjuh.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://sh.gzmigu.cn

[N11] 二叉树中序遍历
来源：http://wz.huixinmuqiang.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gv.newstarts.cn

PHP:  // 手写递归函数
来源：http://av.shtwfgs.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ek.yuexingan06.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ov.bjjhwx.cn

Java: // 手写递归
来源：http://ji.huixinmuqiang.cn

Go:   // 手写递归
来源：http://uk.haigaiapp.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://th.shxzskj.cn

C#:   // 手写递归
来源：http://uh.huixiangedu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xf.panjiajie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://cs.lnxyls.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jp.jianghongdianzi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://oh.asd995.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mq.asd995.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bu.wgjwhj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ev.newstarts.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://su.chemitech.net.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mq.yuntaijiaju.cn

================================================================================
来源：http://jv.jianghongdianzi.cn

O. 并发与异步
来源：http://sd.bookmarksfly.cn

================================================================================
来源：http://xd.hnjuh.cn

[O01] 启动一个线程
来源：http://qa.panjiajie.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://na.shtwfgs.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ga.521024.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bw.lnxyls.cn

TS:   // 同 JS
来源：http://kf.gzmigu.cn

Java: new Thread(() -> f()).start()
来源：http://pf.wgjwhj.cn

Go:   go f()
来源：http://ub.chemitech.net.cn

Ruby: Thread.new { f }
来源：http://cr.yuntaijiaju.cn

C#:   Task.Run(() => F());
来源：http://ts.yuntaijiaju.cn

[O02] 使用线程池
来源：http://ak.chemitech.net.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gj.muxihuayi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gg.chemitech.net.cn

JS:   // worker_threads 线程池
来源：http://fn.colortex.cn

TS:   // worker_threads 线程池
来源：http://li.shxzukj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://mi.chemitech.net.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://yp.yuntaijiaju.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bd.9csxet.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hv.colortex.cn

[O03] 加锁保护共享数据
来源：http://vi.9csxet.cn

Py:   with lock: shared += 1
来源：http://av.521024.cn

PHP:  // 用 flock() 做文件锁
来源：http://am.colortex.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ye.hahajie.cn

TS:   // 同 JS
来源：http://sl.huixiangedu.cn

Java: synchronized (this) { shared++; }
来源：http://iq.hnjuh.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ow.nszjky.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://sq.yuntaijiaju.cn

C#:   lock (gate) { shared++; }
来源：http://ud.shxzukj.cn

[O04] 定义异步函数并等待
来源：http://nh.jctech888.com.cn

Py:   async def f():⏎    await g()
来源：http://vr.yuntaijiaju.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://di.huanxung.cn

JS:   async function f() { await g(); }
来源：http://cq.gzmigu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://qo.jianghongdianzi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://en.nszjky.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zv.nicolike.cn

Ruby: # 用 Fiber 或 async gem
来源：http://nj.yuntaijiaju.cn

C#:   async Task F() { await G(); }
来源：http://cp.lnxyls.cn

[O05] 并发执行并等待全部完成
来源：http://ea.wgjwhj.cn

Py:   asyncio.gather(*tasks)
来源：http://js.newstarts.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://sj.9csxet.cn

JS:   await Promise.all(tasks)
来源：http://iy.yuexingan06.cn

TS:   await Promise.all(tasks)
来源：http://ox.jctech888.com.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rn.9csxet.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mp.shtwfgs.cn

Ruby: threads.map(&:join)
来源：http://aa.yuexingan06.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ot.hnjuh.cn

[O06] 使用进程池
来源：http://ih.newstarts.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://iq.bookmarksfly.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://eh.shtwfgs.cn

JS:   // child_process / cluster 模块
来源：http://do.nicolike.cn

TS:   // child_process / cluster 模块
来源：http://ff.nszjky.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://si.shxzskj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zi.yuexingan06.cn

Ruby: // fork 块
来源：http://rc.asd995.cn

C#:   Parallel.For
来源：http://eq.huanxung.cn

================================================================================
来源：http://qj.szxytkj.cn

P. 常用工具函数
来源：http://bu.gzmigu.cn

================================================================================
来源：http://bo.huixiangedu.cn

[P01] 生成 UUID
来源：http://xd.haigaiapp.cn

Py:   str(uuid.uuid4())
来源：http://qc.521024.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://do.gzmigu.cn

JS:   crypto.randomUUID()
来源：http://ib.szxytkj.cn

TS:   crypto.randomUUID()
来源：http://gn.nicolike.cn

Java: UUID.randomUUID().toString()
来源：http://fg.shxzukj.cn

Go:   // 用 github.com/google/uuid
来源：http://ds.muxihuayi.cn

Ruby: SecureRandom.uuid
来源：http://uo.colortex.cn

C#:   Guid.NewGuid().ToString()
来源：http://jv.asd995.cn

[P02] MD5 / SHA256 摘要
来源：http://po.lnxyls.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://tm.newstarts.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://pg.muxihuayi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ke.nszjky.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fo.shxzskj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zb.521024.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nb.huixinmuqiang.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hb.szxytkj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://sl.newstarts.cn

[P03] 生成短随机字符串
来源：http://tg.newstarts.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://sf.huixiangedu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ja.muxihuayi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lt.chemitech.net.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xg.yuntaijiaju.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rd.hnjuh.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ao.nszjky.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://yg.jctech888.com.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gd.szsharing.cn

[P04] 求长度
来源：http://mw.shxzskj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://lf.panjiajie.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bp.asd995.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rt.yuntaijiaju.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://of.bjjhwx.cn

Java: list.size();  map.size();  s.length()
来源：http://gj.huixiangedu.cn

Go:   len(arr);  len(m)
来源：http://aw.haigaiapp.cn

Ruby: x.length;  x.size
来源：http://av.gzmigu.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://xr.panjiajie.cn

[P05] 判断两个对象内容是否相等
来源：http://uo.shxzskj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ct.asd995.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://eo.wgjwhj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fe.hahajie.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qc.shxzukj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xe.nicolike.cn

Go:   reflect.DeepEqual(a, b)
来源：http://jj.huanxung.cn

Ruby: a == b
来源：http://lt.colortex.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dj.jctech888.com.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://sh.bookmarksfly.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ij.bookmarksfly.cn

PHP:  if (empty($x)) {}
来源：http://tn.wgjwhj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rg.asd995.cn

TS:   if (x == null) {}
来源：http://br.chemitech.net.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://cz.haigaiapp.cn

Go:   if x == nil {}
来源：http://di.huanxung.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hl.hnjuh.cn

C#:   if (x is null) {}
来源：http://pt.nicolike.cn

[P07] 防抖与节流
来源：http://rp.wgjwhj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ie.haigaiapp.cn

PHP:  // 手写时间戳比较
来源：http://xl.panjiajie.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zw.shxzukj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kn.shxzukj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dx.bookmarksfly.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pg.huanxung.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://pk.hnjuh.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://oj.gzmigu.cn

[P08] 处理浮点精度问题
来源：http://jo.521024.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://cv.jianghongdianzi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lj.gzmigu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nj.shtwfgs.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lm.yuexingan06.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qw.hnjuh.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://up.shtwfgs.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ix.jianghongdianzi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://yn.bookmarksfly.cn

================================================================================
来源：http://io.muxihuayi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://km.szxytkj.cn

================================================================================
来源：http://ws.hnjuh.cn

[Q01] 创建表
来源：http://so.shtwfgs.cn

CREATE TABLE users (
来源：http://aa.asd995.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hm.newstarts.cn

name VARCHAR(50) NOT NULL,
来源：http://iu.bookmarksfly.cn

email VARCHAR(100) UNIQUE,
来源：http://fx.nszjky.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://io.nszjky.cn

);
来源：http://md.huanxung.cn

[Q02] 创建带外键的表
来源：http://ew.haigaiapp.cn

CREATE TABLE orders (
来源：http://ei.haigaiapp.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://tc.asd995.cn

user_id INT NOT NULL,
来源：http://qo.lnxyls.cn

amount DECIMAL(10, 2),
来源：http://yu.muxihuayi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qr.521024.cn

);
来源：http://cw.9csxet.cn

[Q03] 增加列
来源：http://xz.haigaiapp.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vv.panjiajie.cn

[Q04] 修改列类型
来源：http://od.chemitech.net.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gc.9csxet.cn

[Q05] 重命名列
来源：http://zj.huixinmuqiang.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://iv.panjiajie.cn

[Q06] 删除列
来源：http://if.colortex.cn

ALTER TABLE users DROP COLUMN age;
来源：http://mz.lnxyls.cn

[Q07] 删除表
来源：http://xs.9csxet.cn

DROP TABLE IF EXISTS orders;
来源：http://zz.shtwfgs.cn

[Q08] 创建普通索引
来源：http://hw.yuntaijiaju.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://mw.shxzukj.cn

[Q09] 创建唯一索引
来源：http://ug.521024.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qk.shxzskj.cn

[Q10] 插入单行
来源：http://pk.huixiangedu.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mx.lnxyls.cn

[Q11] 一次插入多行
来源：http://yp.9csxet.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ot.jctech888.com.cn

[Q12] 插入后取自增 ID
来源：http://jz.haigaiapp.cn

INSERT INTO users (name) VALUES ('C');
来源：http://wm.shxzskj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wj.shxzskj.cn

[Q13] 忽略重复插入
来源：http://xv.bjjhwx.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ws.9csxet.cn

[Q14] 存在则更新（upsert）
来源：http://lp.szsharing.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://db.hahajie.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://cj.jianghongdianzi.cn

[Q15] 查询全部
来源：http://mz.muxihuayi.cn

SELECT * FROM users;
来源：http://gj.jctech888.com.cn

[Q16] 查询指定列
来源：http://eg.chemitech.net.cn

SELECT id, name FROM users;
来源：http://gp.muxihuayi.cn

[Q17] 条件查询
来源：http://fk.huixinmuqiang.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hu.huixinmuqiang.cn

[Q18] 模糊匹配
来源：http://np.yuntaijiaju.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ps.huixiangedu.cn

[Q19] 范围查询
来源：http://xg.szsharing.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://dv.asd995.cn

[Q20] IN 列表
来源：http://tk.panjiajie.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://yj.shxzskj.cn

[Q21] 空值判断
来源：http://ld.huixiangedu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ha.9csxet.cn

[Q22] 排序
来源：http://gm.nszjky.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xh.shtwfgs.cn

[Q23] 分页
来源：http://tu.shxzukj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pc.lnxyls.cn

[Q24] 去重
来源：http://dz.chemitech.net.cn

SELECT DISTINCT city FROM users;
来源：http://oj.gzmigu.cn

[Q25] 只取前 N 条
来源：http://uy.huanxung.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://tv.521024.cn

[Q26] 计数
来源：http://jw.bjjhwx.cn

SELECT COUNT(*) FROM users;
来源：http://nv.wgjwhj.cn

[Q27] 条件计数
来源：http://lx.wgjwhj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jd.hahajie.cn

[Q28] 求和与平均
来源：http://yb.hahajie.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://pl.nicolike.cn

[Q29] 最大最小值
来源：http://nc.szxytkj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://td.huixiangedu.cn

[Q30] 分组统计
来源：http://ke.huixinmuqiang.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vj.shxzukj.cn

[Q31] 分组后过滤
来源：http://va.lnxyls.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fw.9csxet.cn

[Q32] 分组拼接字符串
来源：http://bh.szsharing.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ql.huanxung.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gk.bjjhwx.cn

[Q33] 多列分组
来源：http://sb.chemitech.net.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qg.huixiangedu.cn

[Q34] 每组取第一条
来源：http://ge.hnjuh.cn

SELECT * FROM (
来源：http://zr.nszjky.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://cd.hahajie.cn

) t WHERE rn = 1;
来源：http://up.haigaiapp.cn

[Q35] 内连接
来源：http://hp.gzmigu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://eg.muxihuayi.cn

[Q36] 左连接
来源：http://mt.9csxet.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ig.9csxet.cn

[Q37] 右连接
来源：http://za.nicolike.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://nv.szxytkj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ye.9csxet.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wn.muxihuayi.cn

[Q39] 自连接（查上下级）
来源：http://rv.hnjuh.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://uc.chemitech.net.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vy.chemitech.net.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://hw.panjiajie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ak.asd995.cn

[Q41] 多表连接
来源：http://fd.shtwfgs.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://st.9csxet.cn

JOIN users u ON u.id = o.user_id
来源：http://as.shxzukj.cn

JOIN products p ON p.id = o.product_id;
来源：http://ux.hnjuh.cn

[Q42] 连接条件附加过滤
来源：http://zq.huixiangedu.cn

SELECT u.name, o.amount FROM users u
来源：http://dc.newstarts.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://iv.9csxet.cn

[Q43] 标量子查询
来源：http://eh.nszjky.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ux.lnxyls.cn

[Q44] IN 子查询
来源：http://gc.colortex.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://aa.wgjwhj.cn

[Q45] EXISTS 判断存在
来源：http://uo.yuntaijiaju.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uh.shtwfgs.cn

[Q46] NOT EXISTS 判断不存在
来源：http://mn.hnjuh.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ra.wgjwhj.cn

[Q47] 与平均值比较
来源：http://ew.asd995.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://on.bjjhwx.cn


<!-- 参考信息 -->