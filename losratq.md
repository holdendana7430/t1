代发 wailian999

[N09] 栈与队列
来源：http://yf.hnjuh.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jv.newstarts.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://kb.shxzskj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ht.bjjhwx.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://iz.wgjwhj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kg.hnjuh.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ck.hahajie.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qb.jianghongdianzi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://up.jctech888.com.cn

[N10] 链表节点定义
来源：http://vn.nicolike.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wg.huixinmuqiang.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://zh.haigaiapp.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zy.haigaiapp.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wl.haigaiapp.cn

Java: class Node { int v; Node next; }
来源：http://aa.yuexingan06.cn

Go:   type Node struct { V int; Next *Node }
来源：http://yo.nszjky.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://yy.szsharing.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://kg.asd995.cn

[N11] 二叉树中序遍历
来源：http://qk.bjjhwx.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lf.521024.cn

PHP:  // 手写递归函数
来源：http://ko.gzmigu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pb.huixiangedu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://op.jianghongdianzi.cn

Java: // 手写递归
来源：http://vy.wgjwhj.cn

Go:   // 手写递归
来源：http://to.asd995.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://cv.muxihuayi.cn

C#:   // 手写递归
来源：http://np.panjiajie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ct.newstarts.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://gp.bookmarksfly.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ek.newstarts.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sv.muxihuayi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dx.jctech888.com.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vy.newstarts.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://gs.wgjwhj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tp.jianghongdianzi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kx.newstarts.cn

================================================================================
来源：http://ni.huixinmuqiang.cn

O. 并发与异步
来源：http://gw.shtwfgs.cn

================================================================================
来源：http://lz.asd995.cn

[O01] 启动一个线程
来源：http://mo.hahajie.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pk.bjjhwx.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xr.shxzskj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hk.muxihuayi.cn

TS:   // 同 JS
来源：http://cv.szsharing.cn

Java: new Thread(() -> f()).start()
来源：http://ug.asd995.cn

Go:   go f()
来源：http://kc.nszjky.cn

Ruby: Thread.new { f }
来源：http://vp.9csxet.cn

C#:   Task.Run(() => F());
来源：http://jf.hahajie.cn

[O02] 使用线程池
来源：http://uv.nszjky.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qf.muxihuayi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ja.hahajie.cn

JS:   // worker_threads 线程池
来源：http://yw.panjiajie.cn

TS:   // worker_threads 线程池
来源：http://me.yuexingan06.cn

Java: Executors.newFixedThreadPool(4)
来源：http://gk.huixinmuqiang.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xi.asd995.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xo.huanxung.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mg.muxihuayi.cn

[O03] 加锁保护共享数据
来源：http://mu.gzmigu.cn

Py:   with lock: shared += 1
来源：http://dn.gzmigu.cn

PHP:  // 用 flock() 做文件锁
来源：http://kb.gzmigu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://kh.nszjky.cn

TS:   // 同 JS
来源：http://dh.shtwfgs.cn

Java: synchronized (this) { shared++; }
来源：http://cd.colortex.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://om.9csxet.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://cz.bookmarksfly.cn

C#:   lock (gate) { shared++; }
来源：http://ik.bookmarksfly.cn

[O04] 定义异步函数并等待
来源：http://ck.jctech888.com.cn

Py:   async def f():⏎    await g()
来源：http://ky.newstarts.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tf.hnjuh.cn

JS:   async function f() { await g(); }
来源：http://em.huixiangedu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://sx.hnjuh.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jd.wgjwhj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dn.9csxet.cn

Ruby: # 用 Fiber 或 async gem
来源：http://pn.bookmarksfly.cn

C#:   async Task F() { await G(); }
来源：http://nf.hnjuh.cn

[O05] 并发执行并等待全部完成
来源：http://tr.wgjwhj.cn

Py:   asyncio.gather(*tasks)
来源：http://mf.jctech888.com.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cj.lnxyls.cn

JS:   await Promise.all(tasks)
来源：http://yt.shxzskj.cn

TS:   await Promise.all(tasks)
来源：http://bd.lnxyls.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://di.shxzskj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ri.shxzukj.cn

Ruby: threads.map(&:join)
来源：http://ne.haigaiapp.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://eg.9csxet.cn

[O06] 使用进程池
来源：http://wn.nicolike.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vz.huixiangedu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://if.szxytkj.cn

JS:   // child_process / cluster 模块
来源：http://bp.shxzskj.cn

TS:   // child_process / cluster 模块
来源：http://wy.521024.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://cw.asd995.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wv.szsharing.cn

Ruby: // fork 块
来源：http://fu.hahajie.cn

C#:   Parallel.For
来源：http://rq.jianghongdianzi.cn

================================================================================
来源：http://fp.huixiangedu.cn

P. 常用工具函数
来源：http://zs.yuexingan06.cn

================================================================================
来源：http://iw.asd995.cn

[P01] 生成 UUID
来源：http://we.newstarts.cn

Py:   str(uuid.uuid4())
来源：http://if.chemitech.net.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jz.lnxyls.cn

JS:   crypto.randomUUID()
来源：http://ax.shxzukj.cn

TS:   crypto.randomUUID()
来源：http://fw.chemitech.net.cn

Java: UUID.randomUUID().toString()
来源：http://mx.nszjky.cn

Go:   // 用 github.com/google/uuid
来源：http://qw.asd995.cn

Ruby: SecureRandom.uuid
来源：http://oj.yuntaijiaju.cn

C#:   Guid.NewGuid().ToString()
来源：http://tl.shxzukj.cn

[P02] MD5 / SHA256 摘要
来源：http://em.nicolike.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://nm.muxihuayi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://sx.shxzskj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ts.huixinmuqiang.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jb.yuntaijiaju.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://oy.asd995.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fo.haigaiapp.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://xp.jianghongdianzi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ut.asd995.cn

[P03] 生成短随机字符串
来源：http://hn.nicolike.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zk.jctech888.com.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://oh.shtwfgs.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vv.hnjuh.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ev.muxihuayi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vz.9csxet.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://sn.jctech888.com.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://at.haigaiapp.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://aj.wgjwhj.cn

[P04] 求长度
来源：http://fh.nicolike.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://lf.muxihuayi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qs.shxzskj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sx.gzmigu.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://oc.szxytkj.cn

Java: list.size();  map.size();  s.length()
来源：http://oq.asd995.cn

Go:   len(arr);  len(m)
来源：http://ci.shtwfgs.cn

Ruby: x.length;  x.size
来源：http://sm.bjjhwx.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://fa.huixiangedu.cn

[P05] 判断两个对象内容是否相等
来源：http://af.szsharing.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ea.haigaiapp.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://zv.nicolike.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://av.szxytkj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ap.chemitech.net.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://nx.huixiangedu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://pz.nszjky.cn

Ruby: a == b
来源：http://qu.bookmarksfly.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mp.jianghongdianzi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vm.panjiajie.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ne.gzmigu.cn

PHP:  if (empty($x)) {}
来源：http://xk.newstarts.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ew.huixiangedu.cn

TS:   if (x == null) {}
来源：http://mp.bookmarksfly.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://sc.huixiangedu.cn

Go:   if x == nil {}
来源：http://dr.yuexingan06.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://cv.yuntaijiaju.cn

C#:   if (x is null) {}
来源：http://so.huixinmuqiang.cn

[P07] 防抖与节流
来源：http://jg.chemitech.net.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://st.colortex.cn

PHP:  // 手写时间戳比较
来源：http://kv.wgjwhj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bh.nszjky.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lh.hnjuh.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pw.shtwfgs.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mm.hahajie.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://nc.haigaiapp.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ev.bjjhwx.cn

[P08] 处理浮点精度问题
来源：http://sp.huixinmuqiang.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://by.szxytkj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://yx.colortex.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qr.521024.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vj.bjjhwx.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://sw.muxihuayi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jy.shxzukj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zr.newstarts.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ec.shtwfgs.cn

================================================================================
来源：http://ll.lnxyls.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://kh.bookmarksfly.cn

================================================================================
来源：http://rj.huanxung.cn

[Q01] 创建表
来源：http://tu.yuntaijiaju.cn

CREATE TABLE users (
来源：http://ui.lnxyls.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://un.huixiangedu.cn

name VARCHAR(50) NOT NULL,
来源：http://ku.chemitech.net.cn

email VARCHAR(100) UNIQUE,
来源：http://xj.nicolike.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://fp.nszjky.cn

);
来源：http://mh.szsharing.cn

[Q02] 创建带外键的表
来源：http://gk.yuexingan06.cn

CREATE TABLE orders (
来源：http://ij.szsharing.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ac.newstarts.cn

user_id INT NOT NULL,
来源：http://sk.shxzskj.cn

amount DECIMAL(10, 2),
来源：http://lt.nszjky.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://kp.asd995.cn

);
来源：http://pb.haigaiapp.cn

[Q03] 增加列
来源：http://ss.jctech888.com.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qu.jianghongdianzi.cn

[Q04] 修改列类型
来源：http://hg.asd995.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yh.jctech888.com.cn

[Q05] 重命名列
来源：http://kr.lnxyls.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ry.muxihuayi.cn

[Q06] 删除列
来源：http://ia.yuexingan06.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ty.chemitech.net.cn

[Q07] 删除表
来源：http://tw.huixiangedu.cn

DROP TABLE IF EXISTS orders;
来源：http://iz.nicolike.cn

[Q08] 创建普通索引
来源：http://zw.haigaiapp.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://jw.hnjuh.cn

[Q09] 创建唯一索引
来源：http://ne.chemitech.net.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://we.shxzskj.cn

[Q10] 插入单行
来源：http://ub.9csxet.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qf.shtwfgs.cn

[Q11] 一次插入多行
来源：http://py.shxzskj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rj.hahajie.cn

[Q12] 插入后取自增 ID
来源：http://kc.szxytkj.cn

INSERT INTO users (name) VALUES ('C');
来源：http://hj.yuexingan06.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://st.shtwfgs.cn

[Q13] 忽略重复插入
来源：http://tz.lnxyls.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ju.9csxet.cn

[Q14] 存在则更新（upsert）
来源：http://es.hnjuh.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ic.huanxung.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://uo.szsharing.cn

[Q15] 查询全部
来源：http://vz.521024.cn

SELECT * FROM users;
来源：http://is.asd995.cn

[Q16] 查询指定列
来源：http://vt.jianghongdianzi.cn

SELECT id, name FROM users;
来源：http://yi.nszjky.cn

[Q17] 条件查询
来源：http://gt.521024.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://pp.yuexingan06.cn

[Q18] 模糊匹配
来源：http://ja.9csxet.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://im.bookmarksfly.cn

[Q19] 范围查询
来源：http://xy.newstarts.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ev.chemitech.net.cn

[Q20] IN 列表
来源：http://ej.wgjwhj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zm.wgjwhj.cn

[Q21] 空值判断
来源：http://iy.shtwfgs.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://wv.huixinmuqiang.cn

[Q22] 排序
来源：http://au.huixinmuqiang.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://rv.muxihuayi.cn

[Q23] 分页
来源：http://pu.chemitech.net.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mm.newstarts.cn

[Q24] 去重
来源：http://in.jctech888.com.cn

SELECT DISTINCT city FROM users;
来源：http://mz.bookmarksfly.cn

[Q25] 只取前 N 条
来源：http://gk.hnjuh.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://nh.huixinmuqiang.cn

[Q26] 计数
来源：http://bn.muxihuayi.cn

SELECT COUNT(*) FROM users;
来源：http://js.haigaiapp.cn

[Q27] 条件计数
来源：http://lk.haigaiapp.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ma.huixinmuqiang.cn

[Q28] 求和与平均
来源：http://oa.colortex.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vn.haigaiapp.cn

[Q29] 最大最小值
来源：http://xd.newstarts.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://pz.hahajie.cn

[Q30] 分组统计
来源：http://te.chemitech.net.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://yq.haigaiapp.cn

[Q31] 分组后过滤
来源：http://kc.asd995.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xj.haigaiapp.cn

[Q32] 分组拼接字符串
来源：http://fz.szsharing.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vf.huixinmuqiang.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://zy.gzmigu.cn

[Q33] 多列分组
来源：http://op.nszjky.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://nv.521024.cn

[Q34] 每组取第一条
来源：http://af.huanxung.cn

SELECT * FROM (
来源：http://xk.lnxyls.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ue.jianghongdianzi.cn

) t WHERE rn = 1;
来源：http://qi.shxzskj.cn

[Q35] 内连接
来源：http://yu.nicolike.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://un.huixinmuqiang.cn

[Q36] 左连接
来源：http://bq.9csxet.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://yb.9csxet.cn

[Q37] 右连接
来源：http://ro.gzmigu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://nk.yuexingan06.cn

[Q38] 全外连接（PostgreSQL）
来源：http://qu.lnxyls.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ga.521024.cn

[Q39] 自连接（查上下级）
来源：http://ls.huixiangedu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://zz.jctech888.com.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xv.newstarts.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ns.huixiangedu.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zq.nszjky.cn

[Q41] 多表连接
来源：http://bu.szxytkj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://py.hahajie.cn

JOIN users u ON u.id = o.user_id
来源：http://gs.521024.cn

JOIN products p ON p.id = o.product_id;
来源：http://zv.9csxet.cn

[Q42] 连接条件附加过滤
来源：http://rb.muxihuayi.cn

SELECT u.name, o.amount FROM users u
来源：http://ij.yuexingan06.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ss.chemitech.net.cn

[Q43] 标量子查询
来源：http://ap.bjjhwx.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gv.huixiangedu.cn

[Q44] IN 子查询
来源：http://ws.hnjuh.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bt.9csxet.cn

[Q45] EXISTS 判断存在
来源：http://ri.shtwfgs.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wn.shxzskj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://xe.muxihuayi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tc.nicolike.cn

[Q47] 与平均值比较
来源：http://dk.huanxung.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ap.521024.cn

[Q48] CTE 公用表表达式
来源：http://hm.szxytkj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zx.lnxyls.cn

SELECT * FROM t WHERE c > 5;
来源：http://zo.hnjuh.cn

[Q49] 更新单行
来源：http://sr.panjiajie.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xn.hnjuh.cn

[Q50] 批量更新
来源：http://yi.szsharing.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wj.szsharing.cn

[Q51] 用子查询更新
来源：http://ue.gzmigu.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bz.szsharing.cn

[Q52] 删除指定行
来源：http://ht.shxzskj.cn

DELETE FROM users WHERE id = 10;
来源：http://is.szsharing.cn

[Q53] 按条件删除
来源：http://qt.521024.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://cf.jianghongdianzi.cn

[Q54] 清空表
来源：http://si.hnjuh.cn

TRUNCATE TABLE logs;
来源：http://tv.huixiangedu.cn

[Q55] 排名（并列占位）
来源：http://ep.panjiajie.cn


<!-- 参考信息 -->