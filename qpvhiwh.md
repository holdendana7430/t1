代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://sl.521024.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://vo.szxytkj.cn

TS:   // 手写 Map<string, number>
来源：http://hx.chemitech.net.cn

Java: // 手写 HashMap
来源：http://tg.bjjhwx.cn

Go:   // 手写 map[int]int
来源：http://at.gzmigu.cn

Ruby: // 手写 Hash
来源：http://iy.szsharing.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ws.521024.cn

[N08] 生成全排列
来源：http://nv.colortex.cn

Py:   itertools.permutations(arr)
来源：http://gd.colortex.cn

PHP:  // 手写递归交换
来源：http://ty.yuexingan06.cn

JS:   // 手写回溯递归
来源：http://th.shxzukj.cn

TS:   // 手写回溯递归
来源：http://ti.lnxyls.cn

Java: // 手写回溯递归
来源：http://to.szxytkj.cn

Go:   // 手写回溯递归
来源：http://au.huixiangedu.cn

Ruby: arr.permutation.to_a
来源：http://lm.bjjhwx.cn

C#:   // 手写回溯递归
来源：http://ql.bjjhwx.cn

[N09] 栈与队列
来源：http://zu.haigaiapp.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kc.521024.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ah.huixiangedu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://te.yuntaijiaju.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tt.panjiajie.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nj.lnxyls.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hw.asd995.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ul.shxzskj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gy.szxytkj.cn

[N10] 链表节点定义
来源：http://si.wgjwhj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://il.nicolike.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://iv.shxzskj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ct.lnxyls.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tb.huixiangedu.cn

Java: class Node { int v; Node next; }
来源：http://bx.huixiangedu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://wp.szsharing.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://pm.hnjuh.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://dx.jianghongdianzi.cn

[N11] 二叉树中序遍历
来源：http://cx.hahajie.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dd.gzmigu.cn

PHP:  // 手写递归函数
来源：http://vs.bookmarksfly.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yz.szxytkj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jw.huixinmuqiang.cn

Java: // 手写递归
来源：http://kt.chemitech.net.cn

Go:   // 手写递归
来源：http://fb.521024.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pa.gzmigu.cn

C#:   // 手写递归
来源：http://kx.jianghongdianzi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://up.chemitech.net.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ld.chemitech.net.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://iq.521024.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nt.bookmarksfly.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wk.chemitech.net.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ge.9csxet.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jg.shxzskj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pg.hnjuh.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://sy.panjiajie.cn

================================================================================
来源：http://fx.shxzukj.cn

O. 并发与异步
来源：http://rd.shxzskj.cn

================================================================================
来源：http://iz.hnjuh.cn

[O01] 启动一个线程
来源：http://kj.shtwfgs.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ok.gzmigu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ga.hahajie.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xm.huanxung.cn

TS:   // 同 JS
来源：http://wg.jctech888.com.cn

Java: new Thread(() -> f()).start()
来源：http://zg.huixiangedu.cn

Go:   go f()
来源：http://xa.wgjwhj.cn

Ruby: Thread.new { f }
来源：http://hz.panjiajie.cn

C#:   Task.Run(() => F());
来源：http://cv.hahajie.cn

[O02] 使用线程池
来源：http://vy.bookmarksfly.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://db.shxzukj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mg.haigaiapp.cn

JS:   // worker_threads 线程池
来源：http://lp.panjiajie.cn

TS:   // worker_threads 线程池
来源：http://ay.szsharing.cn

Java: Executors.newFixedThreadPool(4)
来源：http://qw.muxihuayi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://gv.bjjhwx.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://do.gzmigu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ui.yuntaijiaju.cn

[O03] 加锁保护共享数据
来源：http://zy.jianghongdianzi.cn

Py:   with lock: shared += 1
来源：http://xw.chemitech.net.cn

PHP:  // 用 flock() 做文件锁
来源：http://nq.huixinmuqiang.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zp.hnjuh.cn

TS:   // 同 JS
来源：http://ik.wgjwhj.cn

Java: synchronized (this) { shared++; }
来源：http://nu.panjiajie.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://oa.huixiangedu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://dh.huixinmuqiang.cn

C#:   lock (gate) { shared++; }
来源：http://zi.9csxet.cn

[O04] 定义异步函数并等待
来源：http://gh.newstarts.cn

Py:   async def f():⏎    await g()
来源：http://my.shxzskj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wp.huixinmuqiang.cn

JS:   async function f() { await g(); }
来源：http://hm.jctech888.com.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://dx.hnjuh.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://tx.muxihuayi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jx.chemitech.net.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ik.yuntaijiaju.cn

C#:   async Task F() { await G(); }
来源：http://rw.jianghongdianzi.cn

[O05] 并发执行并等待全部完成
来源：http://xg.9csxet.cn

Py:   asyncio.gather(*tasks)
来源：http://tm.huanxung.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xg.shxzskj.cn

JS:   await Promise.all(tasks)
来源：http://oh.521024.cn

TS:   await Promise.all(tasks)
来源：http://cs.shtwfgs.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yq.521024.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qc.szsharing.cn

Ruby: threads.map(&:join)
来源：http://tx.muxihuayi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://iv.wgjwhj.cn

[O06] 使用进程池
来源：http://zx.shtwfgs.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pj.gzmigu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://vx.yuntaijiaju.cn

JS:   // child_process / cluster 模块
来源：http://pp.chemitech.net.cn

TS:   // child_process / cluster 模块
来源：http://bw.jctech888.com.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://kl.huixiangedu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://it.panjiajie.cn

Ruby: // fork 块
来源：http://wi.nicolike.cn

C#:   Parallel.For
来源：http://bn.9csxet.cn

================================================================================
来源：http://dp.shxzukj.cn

P. 常用工具函数
来源：http://cl.bookmarksfly.cn

================================================================================
来源：http://fu.szxytkj.cn

[P01] 生成 UUID
来源：http://ld.muxihuayi.cn

Py:   str(uuid.uuid4())
来源：http://tp.colortex.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hj.hahajie.cn

JS:   crypto.randomUUID()
来源：http://xf.chemitech.net.cn

TS:   crypto.randomUUID()
来源：http://xg.nicolike.cn

Java: UUID.randomUUID().toString()
来源：http://ba.521024.cn

Go:   // 用 github.com/google/uuid
来源：http://or.jctech888.com.cn

Ruby: SecureRandom.uuid
来源：http://du.521024.cn

C#:   Guid.NewGuid().ToString()
来源：http://oa.haigaiapp.cn

[P02] MD5 / SHA256 摘要
来源：http://ye.nicolike.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jn.haigaiapp.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ix.gzmigu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ly.huixiangedu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jn.yuntaijiaju.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vu.521024.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ei.nicolike.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ne.shxzskj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wf.nicolike.cn

[P03] 生成短随机字符串
来源：http://do.hahajie.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rb.bjjhwx.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ce.asd995.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qe.huanxung.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sf.szxytkj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lm.hnjuh.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ys.huanxung.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://jd.asd995.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://cv.colortex.cn

[P04] 求长度
来源：http://pq.bjjhwx.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ug.bookmarksfly.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vf.newstarts.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tb.newstarts.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yh.muxihuayi.cn

Java: list.size();  map.size();  s.length()
来源：http://zn.jctech888.com.cn

Go:   len(arr);  len(m)
来源：http://kh.yuntaijiaju.cn

Ruby: x.length;  x.size
来源：http://ml.jianghongdianzi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://kh.newstarts.cn

[P05] 判断两个对象内容是否相等
来源：http://ui.shxzukj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://mb.yuntaijiaju.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mz.wgjwhj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ie.jianghongdianzi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ss.jctech888.com.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mv.hahajie.cn

Go:   reflect.DeepEqual(a, b)
来源：http://tq.yuexingan06.cn

Ruby: a == b
来源：http://hm.hnjuh.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qd.yuexingan06.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://cc.lnxyls.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pg.bjjhwx.cn

PHP:  if (empty($x)) {}
来源：http://kz.hahajie.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://gj.hahajie.cn

TS:   if (x == null) {}
来源：http://yz.hahajie.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://yq.szsharing.cn

Go:   if x == nil {}
来源：http://bo.szsharing.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://bu.asd995.cn

C#:   if (x is null) {}
来源：http://vt.9csxet.cn

[P07] 防抖与节流
来源：http://ug.lnxyls.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://cu.huixiangedu.cn

PHP:  // 手写时间戳比较
来源：http://cj.huixinmuqiang.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://de.szsharing.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.muxihuayi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://re.jctech888.com.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://po.521024.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ps.shxzukj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vt.yuntaijiaju.cn

[P08] 处理浮点精度问题
来源：http://yr.hnjuh.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fx.gzmigu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ah.hahajie.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://oh.lnxyls.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://uf.haigaiapp.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kn.panjiajie.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://lk.wgjwhj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://yr.9csxet.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://dy.panjiajie.cn

================================================================================
来源：http://hq.asd995.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://pi.huixiangedu.cn

================================================================================
来源：http://vh.shxzukj.cn

[Q01] 创建表
来源：http://ar.nszjky.cn

CREATE TABLE users (
来源：http://gf.muxihuayi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bo.bjjhwx.cn

name VARCHAR(50) NOT NULL,
来源：http://ze.shxzskj.cn

email VARCHAR(100) UNIQUE,
来源：http://jn.shxzukj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zm.huixinmuqiang.cn

);
来源：http://eh.nszjky.cn

[Q02] 创建带外键的表
来源：http://eq.nicolike.cn

CREATE TABLE orders (
来源：http://vi.9csxet.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hj.szsharing.cn

user_id INT NOT NULL,
来源：http://cy.huanxung.cn

amount DECIMAL(10, 2),
来源：http://hp.bjjhwx.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ow.521024.cn

);
来源：http://io.szsharing.cn

[Q03] 增加列
来源：http://zw.bookmarksfly.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zj.muxihuayi.cn

[Q04] 修改列类型
来源：http://ki.yuntaijiaju.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cy.szsharing.cn

[Q05] 重命名列
来源：http://lt.shtwfgs.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xm.hahajie.cn

[Q06] 删除列
来源：http://uk.haigaiapp.cn

ALTER TABLE users DROP COLUMN age;
来源：http://en.szxytkj.cn

[Q07] 删除表
来源：http://hx.szxytkj.cn

DROP TABLE IF EXISTS orders;
来源：http://ev.szsharing.cn

[Q08] 创建普通索引
来源：http://zn.521024.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://tq.chemitech.net.cn

[Q09] 创建唯一索引
来源：http://ix.panjiajie.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://op.jianghongdianzi.cn

[Q10] 插入单行
来源：http://vp.szxytkj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://el.bjjhwx.cn

[Q11] 一次插入多行
来源：http://rb.shxzskj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://oq.lnxyls.cn

[Q12] 插入后取自增 ID
来源：http://il.521024.cn

INSERT INTO users (name) VALUES ('C');
来源：http://pq.haigaiapp.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://bd.bookmarksfly.cn

[Q13] 忽略重复插入
来源：http://uq.newstarts.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ou.9csxet.cn

[Q14] 存在则更新（upsert）
来源：http://iv.gzmigu.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ys.nszjky.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bx.nszjky.cn

[Q15] 查询全部
来源：http://eh.huanxung.cn

SELECT * FROM users;
来源：http://zy.hahajie.cn

[Q16] 查询指定列
来源：http://kp.huixinmuqiang.cn

SELECT id, name FROM users;
来源：http://ea.gzmigu.cn

[Q17] 条件查询
来源：http://km.szsharing.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ee.huanxung.cn

[Q18] 模糊匹配
来源：http://nl.nicolike.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dh.huixinmuqiang.cn

[Q19] 范围查询
来源：http://xs.haigaiapp.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://di.nicolike.cn

[Q20] IN 列表
来源：http://nv.shtwfgs.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ye.521024.cn

[Q21] 空值判断
来源：http://pv.haigaiapp.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://nq.szxytkj.cn

[Q22] 排序
来源：http://ga.colortex.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fm.haigaiapp.cn

[Q23] 分页
来源：http://es.yuexingan06.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ta.szxytkj.cn

[Q24] 去重
来源：http://vf.jianghongdianzi.cn

SELECT DISTINCT city FROM users;
来源：http://cb.521024.cn

[Q25] 只取前 N 条
来源：http://gf.newstarts.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mj.bjjhwx.cn

[Q26] 计数
来源：http://mj.yuntaijiaju.cn

SELECT COUNT(*) FROM users;
来源：http://dm.szxytkj.cn

[Q27] 条件计数
来源：http://nb.huixinmuqiang.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://cq.yuntaijiaju.cn

[Q28] 求和与平均
来源：http://fv.muxihuayi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jn.9csxet.cn

[Q29] 最大最小值
来源：http://ve.lnxyls.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ff.huanxung.cn

[Q30] 分组统计
来源：http://ts.521024.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ow.szxytkj.cn

[Q31] 分组后过滤
来源：http://uu.huanxung.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://iy.jianghongdianzi.cn

[Q32] 分组拼接字符串
来源：http://th.wgjwhj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ts.bookmarksfly.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lj.wgjwhj.cn

[Q33] 多列分组
来源：http://er.yuntaijiaju.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://pm.yuntaijiaju.cn

[Q34] 每组取第一条
来源：http://os.lnxyls.cn

SELECT * FROM (
来源：http://vk.jctech888.com.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://po.bookmarksfly.cn

) t WHERE rn = 1;
来源：http://xq.szsharing.cn

[Q35] 内连接
来源：http://uz.nszjky.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://nu.jianghongdianzi.cn

[Q36] 左连接
来源：http://rz.hahajie.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ph.lnxyls.cn

[Q37] 右连接
来源：http://bp.521024.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rw.nszjky.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ys.colortex.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://co.shxzskj.cn

[Q39] 自连接（查上下级）
来源：http://sd.hahajie.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://fh.yuntaijiaju.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ip.asd995.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://yi.huixiangedu.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hq.panjiajie.cn

[Q41] 多表连接
来源：http://yt.jctech888.com.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://vm.shxzukj.cn

JOIN users u ON u.id = o.user_id
来源：http://ze.9csxet.cn

JOIN products p ON p.id = o.product_id;
来源：http://rh.wgjwhj.cn

[Q42] 连接条件附加过滤
来源：http://ih.521024.cn

SELECT u.name, o.amount FROM users u
来源：http://rk.lnxyls.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://uu.colortex.cn

[Q43] 标量子查询
来源：http://pq.colortex.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lg.hnjuh.cn

[Q44] IN 子查询
来源：http://oe.gzmigu.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ni.bookmarksfly.cn

[Q45] EXISTS 判断存在
来源：http://ac.asd995.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sh.muxihuayi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://rq.nszjky.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vw.shxzskj.cn

[Q47] 与平均值比较
来源：http://gm.newstarts.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vi.haigaiapp.cn


<!-- 参考信息 -->