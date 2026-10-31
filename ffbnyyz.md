代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rc.haigaiapp.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://yt.hahajie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yg.shxzukj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dv.yuexingan06.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xi.gzmigu.cn

[N10] 链表节点定义
来源：http://wg.nicolike.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://bg.szxytkj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://cn.shxzukj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wy.huixinmuqiang.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ii.chemitech.net.cn

Java: class Node { int v; Node next; }
来源：http://mf.hahajie.cn

Go:   type Node struct { V int; Next *Node }
来源：http://qj.szsharing.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://dr.chemitech.net.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://lx.colortex.cn

[N11] 二叉树中序遍历
来源：http://ap.hahajie.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://sx.colortex.cn

PHP:  // 手写递归函数
来源：http://tt.nicolike.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yz.wgjwhj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uu.huixinmuqiang.cn

Java: // 手写递归
来源：http://nl.newstarts.cn

Go:   // 手写递归
来源：http://rw.hnjuh.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://nb.colortex.cn

C#:   // 手写递归
来源：http://hr.huixinmuqiang.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xt.nicolike.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ia.bjjhwx.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xo.shxzskj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fc.szsharing.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jg.jctech888.com.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xo.chemitech.net.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hh.muxihuayi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ab.jctech888.com.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://or.colortex.cn

================================================================================
来源：http://jd.wgjwhj.cn

O. 并发与异步
来源：http://jm.asd995.cn

================================================================================
来源：http://oy.muxihuayi.cn

[O01] 启动一个线程
来源：http://xe.muxihuayi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wi.hahajie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://kn.lnxyls.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rq.szsharing.cn

TS:   // 同 JS
来源：http://cs.bookmarksfly.cn

Java: new Thread(() -> f()).start()
来源：http://lp.yuexingan06.cn

Go:   go f()
来源：http://nm.newstarts.cn

Ruby: Thread.new { f }
来源：http://rw.newstarts.cn

C#:   Task.Run(() => F());
来源：http://ix.haigaiapp.cn

[O02] 使用线程池
来源：http://og.muxihuayi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pn.gzmigu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cn.bookmarksfly.cn

JS:   // worker_threads 线程池
来源：http://hx.panjiajie.cn

TS:   // worker_threads 线程池
来源：http://ur.huixinmuqiang.cn

Java: Executors.newFixedThreadPool(4)
来源：http://id.panjiajie.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ek.nszjky.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://pb.yuexingan06.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://an.hahajie.cn

[O03] 加锁保护共享数据
来源：http://np.muxihuayi.cn

Py:   with lock: shared += 1
来源：http://iz.haigaiapp.cn

PHP:  // 用 flock() 做文件锁
来源：http://qj.jianghongdianzi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fu.asd995.cn

TS:   // 同 JS
来源：http://bl.521024.cn

Java: synchronized (this) { shared++; }
来源：http://jl.muxihuayi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jg.521024.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://xl.bjjhwx.cn

C#:   lock (gate) { shared++; }
来源：http://co.nicolike.cn

[O04] 定义异步函数并等待
来源：http://bs.521024.cn

Py:   async def f():⏎    await g()
来源：http://xz.haigaiapp.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fi.shxzukj.cn

JS:   async function f() { await g(); }
来源：http://qd.panjiajie.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://vq.nszjky.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jl.huanxung.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ke.panjiajie.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ie.colortex.cn

C#:   async Task F() { await G(); }
来源：http://jq.bjjhwx.cn

[O05] 并发执行并等待全部完成
来源：http://pj.yuntaijiaju.cn

Py:   asyncio.gather(*tasks)
来源：http://ky.muxihuayi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xe.colortex.cn

JS:   await Promise.all(tasks)
来源：http://kw.asd995.cn

TS:   await Promise.all(tasks)
来源：http://tx.521024.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zg.asd995.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://jc.jctech888.com.cn

Ruby: threads.map(&:join)
来源：http://qh.szxytkj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://tf.shxzskj.cn

[O06] 使用进程池
来源：http://df.nicolike.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rw.lnxyls.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://nu.bjjhwx.cn

JS:   // child_process / cluster 模块
来源：http://ap.bjjhwx.cn

TS:   // child_process / cluster 模块
来源：http://yr.panjiajie.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://is.colortex.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zt.hahajie.cn

Ruby: // fork 块
来源：http://np.nszjky.cn

C#:   Parallel.For
来源：http://mp.panjiajie.cn

================================================================================
来源：http://qa.yuntaijiaju.cn

P. 常用工具函数
来源：http://cc.newstarts.cn

================================================================================
来源：http://rh.hahajie.cn

[P01] 生成 UUID
来源：http://ld.haigaiapp.cn

Py:   str(uuid.uuid4())
来源：http://ax.bjjhwx.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rw.lnxyls.cn

JS:   crypto.randomUUID()
来源：http://mt.huixiangedu.cn

TS:   crypto.randomUUID()
来源：http://iz.newstarts.cn

Java: UUID.randomUUID().toString()
来源：http://yx.bjjhwx.cn

Go:   // 用 github.com/google/uuid
来源：http://lx.521024.cn

Ruby: SecureRandom.uuid
来源：http://az.shtwfgs.cn

C#:   Guid.NewGuid().ToString()
来源：http://ii.asd995.cn

[P02] MD5 / SHA256 摘要
来源：http://ab.szxytkj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://sn.hahajie.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://xo.bjjhwx.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zj.bjjhwx.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://kx.bookmarksfly.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ey.chemitech.net.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gv.haigaiapp.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ld.huixinmuqiang.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://td.huanxung.cn

[P03] 生成短随机字符串
来源：http://yq.szsharing.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://yh.huixiangedu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://pf.chemitech.net.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nf.colortex.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ro.shxzskj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ii.shtwfgs.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mi.hnjuh.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://wt.yuntaijiaju.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://dj.hnjuh.cn

[P04] 求长度
来源：http://wt.shxzskj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://lu.hahajie.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gz.shtwfgs.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rm.huanxung.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://er.shxzskj.cn

Java: list.size();  map.size();  s.length()
来源：http://oa.yuntaijiaju.cn

Go:   len(arr);  len(m)
来源：http://me.panjiajie.cn

Ruby: x.length;  x.size
来源：http://hv.colortex.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://tf.yuexingan06.cn

[P05] 判断两个对象内容是否相等
来源：http://af.huixiangedu.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://wq.wgjwhj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xz.haigaiapp.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://um.muxihuayi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lm.521024.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://py.asd995.cn

Go:   reflect.DeepEqual(a, b)
来源：http://dq.chemitech.net.cn

Ruby: a == b
来源：http://es.jctech888.com.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://no.wgjwhj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://sa.jctech888.com.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ai.wgjwhj.cn

PHP:  if (empty($x)) {}
来源：http://ye.shtwfgs.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://he.huixinmuqiang.cn

TS:   if (x == null) {}
来源：http://gs.hahajie.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://mu.asd995.cn

Go:   if x == nil {}
来源：http://xi.shxzukj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ei.wgjwhj.cn

C#:   if (x is null) {}
来源：http://zv.haigaiapp.cn

[P07] 防抖与节流
来源：http://yr.yuexingan06.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mj.muxihuayi.cn

PHP:  // 手写时间戳比较
来源：http://mr.wgjwhj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vg.yuntaijiaju.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hb.jianghongdianzi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jb.gzmigu.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://kz.wgjwhj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://oo.shxzskj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ft.muxihuayi.cn

[P08] 处理浮点精度问题
来源：http://nm.bjjhwx.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://aw.chemitech.net.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cl.panjiajie.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://rc.muxihuayi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://oe.shxzukj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ke.521024.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ic.haigaiapp.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zm.colortex.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ut.yuexingan06.cn

================================================================================
来源：http://dj.huixiangedu.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ri.muxihuayi.cn

================================================================================
来源：http://pr.lnxyls.cn

[Q01] 创建表
来源：http://cv.szxytkj.cn

CREATE TABLE users (
来源：http://gr.huixiangedu.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dx.9csxet.cn

name VARCHAR(50) NOT NULL,
来源：http://ar.haigaiapp.cn

email VARCHAR(100) UNIQUE,
来源：http://yo.huixiangedu.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://is.huanxung.cn

);
来源：http://pp.szsharing.cn

[Q02] 创建带外键的表
来源：http://ic.huixiangedu.cn

CREATE TABLE orders (
来源：http://uu.haigaiapp.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://re.newstarts.cn

user_id INT NOT NULL,
来源：http://ms.yuexingan06.cn

amount DECIMAL(10, 2),
来源：http://yx.muxihuayi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://kv.szxytkj.cn

);
来源：http://zj.bjjhwx.cn

[Q03] 增加列
来源：http://zt.hnjuh.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://cz.bjjhwx.cn

[Q04] 修改列类型
来源：http://vd.panjiajie.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wy.bjjhwx.cn

[Q05] 重命名列
来源：http://it.hahajie.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zu.shxzskj.cn

[Q06] 删除列
来源：http://oc.yuexingan06.cn

ALTER TABLE users DROP COLUMN age;
来源：http://xs.panjiajie.cn

[Q07] 删除表
来源：http://ve.asd995.cn

DROP TABLE IF EXISTS orders;
来源：http://nv.yuexingan06.cn

[Q08] 创建普通索引
来源：http://qi.shtwfgs.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://uq.chemitech.net.cn

[Q09] 创建唯一索引
来源：http://yz.9csxet.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hg.bookmarksfly.cn

[Q10] 插入单行
来源：http://df.bjjhwx.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://id.bjjhwx.cn

[Q11] 一次插入多行
来源：http://sn.yuexingan06.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ja.jctech888.com.cn

[Q12] 插入后取自增 ID
来源：http://bm.yuexingan06.cn

INSERT INTO users (name) VALUES ('C');
来源：http://bu.colortex.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://gg.521024.cn

[Q13] 忽略重复插入
来源：http://qk.shtwfgs.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mi.haigaiapp.cn

[Q14] 存在则更新（upsert）
来源：http://ik.jctech888.com.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://jc.yuntaijiaju.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ul.panjiajie.cn

[Q15] 查询全部
来源：http://pa.shxzukj.cn

SELECT * FROM users;
来源：http://cm.muxihuayi.cn

[Q16] 查询指定列
来源：http://uy.bjjhwx.cn

SELECT id, name FROM users;
来源：http://wb.shxzskj.cn

[Q17] 条件查询
来源：http://jd.shtwfgs.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zz.szxytkj.cn

[Q18] 模糊匹配
来源：http://ws.newstarts.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zg.shxzskj.cn

[Q19] 范围查询
来源：http://xv.nszjky.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hn.nszjky.cn

[Q20] IN 列表
来源：http://qv.haigaiapp.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ig.gzmigu.cn

[Q21] 空值判断
来源：http://dn.shxzskj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://pr.muxihuayi.cn

[Q22] 排序
来源：http://dn.huixinmuqiang.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://nv.muxihuayi.cn

[Q23] 分页
来源：http://mj.shxzukj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gj.yuntaijiaju.cn

[Q24] 去重
来源：http://kl.asd995.cn

SELECT DISTINCT city FROM users;
来源：http://kx.jianghongdianzi.cn

[Q25] 只取前 N 条
来源：http://hz.asd995.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ts.shxzukj.cn

[Q26] 计数
来源：http://lb.shtwfgs.cn

SELECT COUNT(*) FROM users;
来源：http://ee.hahajie.cn

[Q27] 条件计数
来源：http://qd.hahajie.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jd.shxzskj.cn

[Q28] 求和与平均
来源：http://bl.521024.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://la.huixinmuqiang.cn

[Q29] 最大最小值
来源：http://ui.jianghongdianzi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://yw.yuexingan06.cn

[Q30] 分组统计
来源：http://jk.jctech888.com.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fi.huixiangedu.cn

[Q31] 分组后过滤
来源：http://rb.asd995.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://tz.bjjhwx.cn

[Q32] 分组拼接字符串
来源：http://up.colortex.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wm.521024.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://tx.bookmarksfly.cn

[Q33] 多列分组
来源：http://at.yuexingan06.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wz.nicolike.cn

[Q34] 每组取第一条
来源：http://zd.panjiajie.cn

SELECT * FROM (
来源：http://kp.yuexingan06.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ft.nicolike.cn

) t WHERE rn = 1;
来源：http://an.haigaiapp.cn

[Q35] 内连接
来源：http://or.shtwfgs.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://oi.jianghongdianzi.cn

[Q36] 左连接
来源：http://ya.chemitech.net.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://gw.newstarts.cn

[Q37] 右连接
来源：http://qr.szsharing.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mg.wgjwhj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://iu.nicolike.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mo.huixiangedu.cn

[Q39] 自连接（查上下级）
来源：http://bz.yuntaijiaju.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://dn.jctech888.com.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://so.hnjuh.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://xb.yuntaijiaju.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://og.yuexingan06.cn

[Q41] 多表连接
来源：http://jl.9csxet.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://yi.wgjwhj.cn

JOIN users u ON u.id = o.user_id
来源：http://kv.jctech888.com.cn

JOIN products p ON p.id = o.product_id;
来源：http://qw.haigaiapp.cn

[Q42] 连接条件附加过滤
来源：http://np.shxzukj.cn

SELECT u.name, o.amount FROM users u
来源：http://xz.wgjwhj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vm.lnxyls.cn

[Q43] 标量子查询
来源：http://kq.jctech888.com.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://eb.yuntaijiaju.cn

[Q44] IN 子查询
来源：http://up.hahajie.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ch.yuntaijiaju.cn

[Q45] EXISTS 判断存在
来源：http://wf.huixinmuqiang.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ws.bookmarksfly.cn

[Q46] NOT EXISTS 判断不存在
来源：http://uw.hnjuh.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qu.521024.cn

[Q47] 与平均值比较
来源：http://vg.colortex.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vs.shxzukj.cn

[Q48] CTE 公用表表达式
来源：http://co.shxzskj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kr.hnjuh.cn

SELECT * FROM t WHERE c > 5;
来源：http://ol.huixiangedu.cn

[Q49] 更新单行
来源：http://kv.shtwfgs.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zo.huanxung.cn

[Q50] 批量更新
来源：http://ot.bookmarksfly.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://co.shtwfgs.cn

[Q51] 用子查询更新
来源：http://qx.chemitech.net.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://uw.nszjky.cn

[Q52] 删除指定行
来源：http://kx.521024.cn

DELETE FROM users WHERE id = 10;
来源：http://ja.shxzukj.cn

[Q53] 按条件删除
来源：http://xt.jctech888.com.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gu.colortex.cn

[Q54] 清空表
来源：http://df.hnjuh.cn

TRUNCATE TABLE logs;
来源：http://ho.huixinmuqiang.cn

[Q55] 排名（并列占位）
来源：http://hd.hahajie.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ow.colortex.cn

[Q56] 密集排名（并列不占位）
来源：http://se.muxihuayi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ol.newstarts.cn

[Q57] 行号
来源：http://hq.szsharing.cn


<!-- 参考信息 -->