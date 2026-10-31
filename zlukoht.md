代发 wailian999

[N09] 栈与队列
来源：http://je.asd995.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ys.hahajie.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://oc.shxzskj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://sw.shtwfgs.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://eu.gzmigu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fk.nicolike.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cs.szsharing.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ao.lnxyls.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kp.szxytkj.cn

[N10] 链表节点定义
来源：http://ve.jctech888.com.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ug.shtwfgs.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ot.haigaiapp.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://sx.chemitech.net.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xb.asd995.cn

Java: class Node { int v; Node next; }
来源：http://rz.newstarts.cn

Go:   type Node struct { V int; Next *Node }
来源：http://fn.yuntaijiaju.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://pv.9csxet.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://vz.521024.cn

[N11] 二叉树中序遍历
来源：http://nv.wgjwhj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://fa.chemitech.net.cn

PHP:  // 手写递归函数
来源：http://fq.shxzskj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nj.lnxyls.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qg.shxzukj.cn

Java: // 手写递归
来源：http://il.panjiajie.cn

Go:   // 手写递归
来源：http://oe.shxzskj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://cm.jianghongdianzi.cn

C#:   // 手写递归
来源：http://xx.shtwfgs.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ze.9csxet.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ez.nszjky.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ra.newstarts.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hd.lnxyls.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sc.gzmigu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qc.colortex.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dk.521024.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wg.jctech888.com.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fr.yuntaijiaju.cn

================================================================================
来源：http://ls.muxihuayi.cn

O. 并发与异步
来源：http://cg.huixiangedu.cn

================================================================================
来源：http://ko.nszjky.cn

[O01] 启动一个线程
来源：http://gz.yuntaijiaju.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hy.yuntaijiaju.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fb.hnjuh.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mh.bjjhwx.cn

TS:   // 同 JS
来源：http://fx.jianghongdianzi.cn

Java: new Thread(() -> f()).start()
来源：http://ok.hnjuh.cn

Go:   go f()
来源：http://wr.9csxet.cn

Ruby: Thread.new { f }
来源：http://dy.hnjuh.cn

C#:   Task.Run(() => F());
来源：http://hv.haigaiapp.cn

[O02] 使用线程池
来源：http://ye.panjiajie.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://oy.colortex.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cq.lnxyls.cn

JS:   // worker_threads 线程池
来源：http://fd.shxzukj.cn

TS:   // worker_threads 线程池
来源：http://ou.szxytkj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://it.521024.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://we.colortex.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vg.huixinmuqiang.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://px.yuexingan06.cn

[O03] 加锁保护共享数据
来源：http://gg.asd995.cn

Py:   with lock: shared += 1
来源：http://by.jianghongdianzi.cn

PHP:  // 用 flock() 做文件锁
来源：http://ko.colortex.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mq.jianghongdianzi.cn

TS:   // 同 JS
来源：http://db.chemitech.net.cn

Java: synchronized (this) { shared++; }
来源：http://dl.9csxet.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://up.chemitech.net.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://fq.bookmarksfly.cn

C#:   lock (gate) { shared++; }
来源：http://jt.muxihuayi.cn

[O04] 定义异步函数并等待
来源：http://we.huixinmuqiang.cn

Py:   async def f():⏎    await g()
来源：http://mr.colortex.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jr.521024.cn

JS:   async function f() { await g(); }
来源：http://ah.yuntaijiaju.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://wg.haigaiapp.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ib.gzmigu.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ju.hahajie.cn

Ruby: # 用 Fiber 或 async gem
来源：http://si.hahajie.cn

C#:   async Task F() { await G(); }
来源：http://bs.chemitech.net.cn

[O05] 并发执行并等待全部完成
来源：http://yu.muxihuayi.cn

Py:   asyncio.gather(*tasks)
来源：http://gt.colortex.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lu.colortex.cn

JS:   await Promise.all(tasks)
来源：http://cy.jctech888.com.cn

TS:   await Promise.all(tasks)
来源：http://bd.szxytkj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hx.shxzskj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dx.nszjky.cn

Ruby: threads.map(&:join)
来源：http://zr.yuntaijiaju.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ut.chemitech.net.cn

[O06] 使用进程池
来源：http://mt.9csxet.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://sn.jianghongdianzi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://tc.9csxet.cn

JS:   // child_process / cluster 模块
来源：http://vx.hahajie.cn

TS:   // child_process / cluster 模块
来源：http://he.shxzukj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vr.szsharing.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://rm.bjjhwx.cn

Ruby: // fork 块
来源：http://vg.bookmarksfly.cn

C#:   Parallel.For
来源：http://oh.szsharing.cn

================================================================================
来源：http://ww.huanxung.cn

P. 常用工具函数
来源：http://gk.haigaiapp.cn

================================================================================
来源：http://ru.colortex.cn

[P01] 生成 UUID
来源：http://kp.lnxyls.cn

Py:   str(uuid.uuid4())
来源：http://yd.hahajie.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xo.huixiangedu.cn

JS:   crypto.randomUUID()
来源：http://lv.panjiajie.cn

TS:   crypto.randomUUID()
来源：http://dh.huixinmuqiang.cn

Java: UUID.randomUUID().toString()
来源：http://ev.9csxet.cn

Go:   // 用 github.com/google/uuid
来源：http://fc.lnxyls.cn

Ruby: SecureRandom.uuid
来源：http://dh.jctech888.com.cn

C#:   Guid.NewGuid().ToString()
来源：http://ny.bjjhwx.cn

[P02] MD5 / SHA256 摘要
来源：http://nv.nicolike.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dl.jianghongdianzi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://vi.colortex.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://cw.521024.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hx.gzmigu.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ux.huixiangedu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://du.yuntaijiaju.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ad.shxzskj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zm.szsharing.cn

[P03] 生成短随机字符串
来源：http://ye.lnxyls.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wn.jianghongdianzi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://fe.panjiajie.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ab.hahajie.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tl.521024.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://if.newstarts.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pd.shxzskj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://qa.hahajie.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://sv.colortex.cn

[P04] 求长度
来源：http://kq.szxytkj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://cx.nicolike.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://um.huixiangedu.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ax.colortex.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hx.huixinmuqiang.cn

Java: list.size();  map.size();  s.length()
来源：http://vy.huixinmuqiang.cn

Go:   len(arr);  len(m)
来源：http://lk.bjjhwx.cn

Ruby: x.length;  x.size
来源：http://pl.haigaiapp.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://lx.gzmigu.cn

[P05] 判断两个对象内容是否相等
来源：http://hf.gzmigu.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://he.shxzskj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bo.huixinmuqiang.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://na.bjjhwx.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://si.muxihuayi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://en.asd995.cn

Go:   reflect.DeepEqual(a, b)
来源：http://tn.jctech888.com.cn

Ruby: a == b
来源：http://hu.muxihuayi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://iu.chemitech.net.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ln.huanxung.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://kz.shtwfgs.cn

PHP:  if (empty($x)) {}
来源：http://bi.shxzskj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://uz.chemitech.net.cn

TS:   if (x == null) {}
来源：http://iy.yuntaijiaju.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://sh.9csxet.cn

Go:   if x == nil {}
来源：http://lc.wgjwhj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pb.huixinmuqiang.cn

C#:   if (x is null) {}
来源：http://rl.shxzskj.cn

[P07] 防抖与节流
来源：http://wl.yuntaijiaju.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mj.muxihuayi.cn

PHP:  // 手写时间戳比较
来源：http://on.colortex.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hn.nicolike.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://so.huixiangedu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://rx.muxihuayi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nv.asd995.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://be.chemitech.net.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wh.newstarts.cn

[P08] 处理浮点精度问题
来源：http://rr.nszjky.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ry.hahajie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wr.asd995.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://un.lnxyls.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xl.colortex.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lx.haigaiapp.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jz.9csxet.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://cq.muxihuayi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jd.521024.cn

================================================================================
来源：http://sm.521024.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ig.nszjky.cn

================================================================================
来源：http://rn.panjiajie.cn

[Q01] 创建表
来源：http://qw.panjiajie.cn

CREATE TABLE users (
来源：http://do.wgjwhj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hi.haigaiapp.cn

name VARCHAR(50) NOT NULL,
来源：http://ua.bookmarksfly.cn

email VARCHAR(100) UNIQUE,
来源：http://kg.9csxet.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://px.szsharing.cn

);
来源：http://cn.haigaiapp.cn

[Q02] 创建带外键的表
来源：http://ll.chemitech.net.cn

CREATE TABLE orders (
来源：http://ak.huanxung.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hb.shtwfgs.cn

user_id INT NOT NULL,
来源：http://gk.bjjhwx.cn

amount DECIMAL(10, 2),
来源：http://yb.521024.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://op.huixiangedu.cn

);
来源：http://pc.panjiajie.cn

[Q03] 增加列
来源：http://ep.wgjwhj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://sl.chemitech.net.cn

[Q04] 修改列类型
来源：http://sq.bookmarksfly.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://el.colortex.cn

[Q05] 重命名列
来源：http://fx.hahajie.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fs.huixiangedu.cn

[Q06] 删除列
来源：http://ka.huixinmuqiang.cn

ALTER TABLE users DROP COLUMN age;
来源：http://oe.muxihuayi.cn

[Q07] 删除表
来源：http://wo.muxihuayi.cn

DROP TABLE IF EXISTS orders;
来源：http://kq.wgjwhj.cn

[Q08] 创建普通索引
来源：http://gz.newstarts.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://gk.nicolike.cn

[Q09] 创建唯一索引
来源：http://os.gzmigu.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nc.yuexingan06.cn

[Q10] 插入单行
来源：http://ed.chemitech.net.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://rq.lnxyls.cn

[Q11] 一次插入多行
来源：http://bm.muxihuayi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://de.yuexingan06.cn

[Q12] 插入后取自增 ID
来源：http://cx.huanxung.cn

INSERT INTO users (name) VALUES ('C');
来源：http://hu.szsharing.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ze.9csxet.cn

[Q13] 忽略重复插入
来源：http://zt.szxytkj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.huixiangedu.cn

[Q14] 存在则更新（upsert）
来源：http://oo.shxzukj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gb.muxihuayi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qw.shtwfgs.cn

[Q15] 查询全部
来源：http://wv.huixiangedu.cn

SELECT * FROM users;
来源：http://yn.wgjwhj.cn

[Q16] 查询指定列
来源：http://vw.chemitech.net.cn

SELECT id, name FROM users;
来源：http://bp.521024.cn

[Q17] 条件查询
来源：http://ne.szxytkj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://yd.nszjky.cn

[Q18] 模糊匹配
来源：http://aq.chemitech.net.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ry.lnxyls.cn

[Q19] 范围查询
来源：http://zz.wgjwhj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pc.chemitech.net.cn

[Q20] IN 列表
来源：http://xy.yuntaijiaju.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://le.hnjuh.cn

[Q21] 空值判断
来源：http://ba.wgjwhj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ls.bookmarksfly.cn

[Q22] 排序
来源：http://xk.colortex.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://cp.521024.cn

[Q23] 分页
来源：http://dy.9csxet.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://bb.yuntaijiaju.cn

[Q24] 去重
来源：http://vl.9csxet.cn

SELECT DISTINCT city FROM users;
来源：http://eo.shxzukj.cn

[Q25] 只取前 N 条
来源：http://wf.chemitech.net.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://bn.bookmarksfly.cn

[Q26] 计数
来源：http://no.huixinmuqiang.cn

SELECT COUNT(*) FROM users;
来源：http://rk.jianghongdianzi.cn

[Q27] 条件计数
来源：http://ey.shxzukj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://np.yuntaijiaju.cn

[Q28] 求和与平均
来源：http://qd.jianghongdianzi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dh.szxytkj.cn

[Q29] 最大最小值
来源：http://lh.521024.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://qg.muxihuayi.cn

[Q30] 分组统计
来源：http://yj.panjiajie.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wa.huixiangedu.cn

[Q31] 分组后过滤
来源：http://zj.yuntaijiaju.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://pb.jianghongdianzi.cn

[Q32] 分组拼接字符串
来源：http://kq.huixinmuqiang.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lv.newstarts.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fa.haigaiapp.cn

[Q33] 多列分组
来源：http://zp.huanxung.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zz.panjiajie.cn

[Q34] 每组取第一条
来源：http://aa.szsharing.cn

SELECT * FROM (
来源：http://fy.yuntaijiaju.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://cp.panjiajie.cn

) t WHERE rn = 1;
来源：http://gk.9csxet.cn

[Q35] 内连接
来源：http://us.9csxet.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ku.lnxyls.cn

[Q36] 左连接
来源：http://th.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ug.shtwfgs.cn

[Q37] 右连接
来源：http://oj.gzmigu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://em.szsharing.cn

[Q38] 全外连接（PostgreSQL）
来源：http://yi.szxytkj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fw.521024.cn

[Q39] 自连接（查上下级）
来源：http://hg.wgjwhj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://vv.muxihuayi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dt.panjiajie.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://cp.shxzskj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fo.chemitech.net.cn

[Q41] 多表连接
来源：http://ah.yuntaijiaju.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ci.shxzskj.cn

JOIN users u ON u.id = o.user_id
来源：http://hc.521024.cn

JOIN products p ON p.id = o.product_id;
来源：http://wi.huixinmuqiang.cn

[Q42] 连接条件附加过滤
来源：http://yn.asd995.cn

SELECT u.name, o.amount FROM users u
来源：http://hf.szsharing.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fc.szsharing.cn

[Q43] 标量子查询
来源：http://iw.bjjhwx.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jz.yuexingan06.cn

[Q44] IN 子查询
来源：http://co.jctech888.com.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://or.hahajie.cn

[Q45] EXISTS 判断存在
来源：http://ga.yuntaijiaju.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zz.yuntaijiaju.cn

[Q46] NOT EXISTS 判断不存在
来源：http://qu.lnxyls.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://st.panjiajie.cn

[Q47] 与平均值比较
来源：http://lw.9csxet.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lp.nszjky.cn

[Q48] CTE 公用表表达式
来源：http://ii.szsharing.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://fk.yuntaijiaju.cn

SELECT * FROM t WHERE c > 5;
来源：http://hr.panjiajie.cn

[Q49] 更新单行
来源：http://lr.nszjky.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://dv.hahajie.cn

[Q50] 批量更新
来源：http://hb.hahajie.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hw.newstarts.cn

[Q51] 用子查询更新
来源：http://mw.newstarts.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hg.newstarts.cn

[Q52] 删除指定行
来源：http://tz.chemitech.net.cn

DELETE FROM users WHERE id = 10;
来源：http://xc.shxzskj.cn

[Q53] 按条件删除
来源：http://ng.yuexingan06.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qj.jianghongdianzi.cn

[Q54] 清空表
来源：http://dg.huixiangedu.cn

TRUNCATE TABLE logs;
来源：http://ta.asd995.cn

[Q55] 排名（并列占位）
来源：http://og.nszjky.cn


<!-- 参考信息 -->