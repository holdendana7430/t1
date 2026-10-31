代发 wailian999

[N09] 栈与队列
来源：http://ty.shxzukj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://cd.nszjky.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ey.hnjuh.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ox.wgjwhj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ls.muxihuayi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ob.yuexingan06.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mw.jctech888.com.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jo.shxzskj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dj.bjjhwx.cn

[N10] 链表节点定义
来源：http://tr.huanxung.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rr.jctech888.com.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://fs.muxihuayi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qb.yuntaijiaju.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://om.hahajie.cn

Java: class Node { int v; Node next; }
来源：http://ar.yuexingan06.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ef.nszjky.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://nz.huixiangedu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ni.gzmigu.cn

[N11] 二叉树中序遍历
来源：http://ua.asd995.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://on.shtwfgs.cn

PHP:  // 手写递归函数
来源：http://bj.yuexingan06.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qt.chemitech.net.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ol.gzmigu.cn

Java: // 手写递归
来源：http://vq.huixinmuqiang.cn

Go:   // 手写递归
来源：http://ga.chemitech.net.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bf.nszjky.cn

C#:   // 手写递归
来源：http://ph.asd995.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mp.bjjhwx.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rx.shxzskj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ig.nszjky.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nw.yuexingan06.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qb.521024.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://sr.haigaiapp.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jy.newstarts.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bd.gzmigu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://me.panjiajie.cn

================================================================================
来源：http://lo.hnjuh.cn

O. 并发与异步
来源：http://hq.chemitech.net.cn

================================================================================
来源：http://ra.shxzukj.cn

[O01] 启动一个线程
来源：http://om.asd995.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zi.szsharing.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qp.521024.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gq.shxzukj.cn

TS:   // 同 JS
来源：http://id.haigaiapp.cn

Java: new Thread(() -> f()).start()
来源：http://ov.gzmigu.cn

Go:   go f()
来源：http://gi.shtwfgs.cn

Ruby: Thread.new { f }
来源：http://pt.szxytkj.cn

C#:   Task.Run(() => F());
来源：http://rf.lnxyls.cn

[O02] 使用线程池
来源：http://pr.haigaiapp.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fe.nszjky.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ml.huixinmuqiang.cn

JS:   // worker_threads 线程池
来源：http://sk.bjjhwx.cn

TS:   // worker_threads 线程池
来源：http://hn.muxihuayi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://xu.szsharing.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hr.huixiangedu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wn.chemitech.net.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://az.haigaiapp.cn

[O03] 加锁保护共享数据
来源：http://ht.muxihuayi.cn

Py:   with lock: shared += 1
来源：http://av.haigaiapp.cn

PHP:  // 用 flock() 做文件锁
来源：http://bb.asd995.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fe.521024.cn

TS:   // 同 JS
来源：http://go.bjjhwx.cn

Java: synchronized (this) { shared++; }
来源：http://ny.bookmarksfly.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dd.huixiangedu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://vi.newstarts.cn

C#:   lock (gate) { shared++; }
来源：http://it.yuntaijiaju.cn

[O04] 定义异步函数并等待
来源：http://lj.shxzskj.cn

Py:   async def f():⏎    await g()
来源：http://rf.9csxet.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://nc.yuexingan06.cn

JS:   async function f() { await g(); }
来源：http://mx.yuntaijiaju.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://by.chemitech.net.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ya.521024.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gk.nicolike.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ik.nicolike.cn

C#:   async Task F() { await G(); }
来源：http://wj.hnjuh.cn

[O05] 并发执行并等待全部完成
来源：http://xg.lnxyls.cn

Py:   asyncio.gather(*tasks)
来源：http://qy.shxzukj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fq.colortex.cn

JS:   await Promise.all(tasks)
来源：http://ak.panjiajie.cn

TS:   await Promise.all(tasks)
来源：http://fd.jctech888.com.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yj.szxytkj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ic.szsharing.cn

Ruby: threads.map(&:join)
来源：http://kq.yuexingan06.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://fs.huanxung.cn

[O06] 使用进程池
来源：http://lz.huanxung.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ob.yuexingan06.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://yd.shxzukj.cn

JS:   // child_process / cluster 模块
来源：http://dp.huanxung.cn

TS:   // child_process / cluster 模块
来源：http://cz.jctech888.com.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://af.hnjuh.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ux.chemitech.net.cn

Ruby: // fork 块
来源：http://ap.muxihuayi.cn

C#:   Parallel.For
来源：http://pw.haigaiapp.cn

================================================================================
来源：http://tr.szsharing.cn

P. 常用工具函数
来源：http://ro.panjiajie.cn

================================================================================
来源：http://tp.szxytkj.cn

[P01] 生成 UUID
来源：http://kt.nszjky.cn

Py:   str(uuid.uuid4())
来源：http://qx.wgjwhj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://we.shtwfgs.cn

JS:   crypto.randomUUID()
来源：http://co.panjiajie.cn

TS:   crypto.randomUUID()
来源：http://vp.yuexingan06.cn

Java: UUID.randomUUID().toString()
来源：http://ds.hnjuh.cn

Go:   // 用 github.com/google/uuid
来源：http://su.huixiangedu.cn

Ruby: SecureRandom.uuid
来源：http://ie.shtwfgs.cn

C#:   Guid.NewGuid().ToString()
来源：http://zq.shtwfgs.cn

[P02] MD5 / SHA256 摘要
来源：http://vy.asd995.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fz.huixiangedu.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://sr.szsharing.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ja.asd995.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://np.jianghongdianzi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://kj.hnjuh.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qs.colortex.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://aa.asd995.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://iy.huixinmuqiang.cn

[P03] 生成短随机字符串
来源：http://en.huixinmuqiang.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://bj.yuexingan06.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ce.yuexingan06.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sb.yuntaijiaju.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xt.haigaiapp.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ad.chemitech.net.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://td.asd995.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://lp.9csxet.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://nt.lnxyls.cn

[P04] 求长度
来源：http://zo.yuntaijiaju.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://dx.asd995.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uy.hnjuh.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ai.huanxung.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vs.hahajie.cn

Java: list.size();  map.size();  s.length()
来源：http://ww.colortex.cn

Go:   len(arr);  len(m)
来源：http://pw.muxihuayi.cn

Ruby: x.length;  x.size
来源：http://db.shtwfgs.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://qk.wgjwhj.cn

[P05] 判断两个对象内容是否相等
来源：http://lw.wgjwhj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://uq.shxzskj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lt.wgjwhj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://pp.yuexingan06.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zu.nszjky.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://cv.jianghongdianzi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://pu.hnjuh.cn

Ruby: a == b
来源：http://ut.newstarts.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dl.yuexingan06.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ja.panjiajie.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zd.asd995.cn

PHP:  if (empty($x)) {}
来源：http://ld.9csxet.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://nt.lnxyls.cn

TS:   if (x == null) {}
来源：http://en.szsharing.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://nb.9csxet.cn

Go:   if x == nil {}
来源：http://wa.nszjky.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://uo.521024.cn

C#:   if (x is null) {}
来源：http://qz.nicolike.cn

[P07] 防抖与节流
来源：http://vx.yuntaijiaju.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://cp.9csxet.cn

PHP:  // 手写时间戳比较
来源：http://ho.shtwfgs.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zv.chemitech.net.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://om.yuntaijiaju.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://eh.panjiajie.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qm.lnxyls.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://xb.shxzskj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://nn.szsharing.cn

[P08] 处理浮点精度问题
来源：http://mv.9csxet.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vf.bjjhwx.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kq.haigaiapp.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://lx.huixiangedu.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://gn.521024.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://al.jianghongdianzi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ya.hahajie.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://et.haigaiapp.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://kh.huanxung.cn

================================================================================
来源：http://ca.newstarts.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vp.shxzukj.cn

================================================================================
来源：http://op.szxytkj.cn

[Q01] 创建表
来源：http://fp.shxzskj.cn

CREATE TABLE users (
来源：http://qa.lnxyls.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ob.newstarts.cn

name VARCHAR(50) NOT NULL,
来源：http://lv.newstarts.cn

email VARCHAR(100) UNIQUE,
来源：http://ui.colortex.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wm.nicolike.cn

);
来源：http://io.shxzskj.cn

[Q02] 创建带外键的表
来源：http://jq.jianghongdianzi.cn

CREATE TABLE orders (
来源：http://fr.szsharing.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://gx.newstarts.cn

user_id INT NOT NULL,
来源：http://yw.gzmigu.cn

amount DECIMAL(10, 2),
来源：http://zm.newstarts.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ia.nszjky.cn

);
来源：http://du.gzmigu.cn

[Q03] 增加列
来源：http://id.shxzskj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wj.huixinmuqiang.cn

[Q04] 修改列类型
来源：http://lm.szxytkj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yl.haigaiapp.cn

[Q05] 重命名列
来源：http://wh.haigaiapp.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://sm.haigaiapp.cn

[Q06] 删除列
来源：http://mh.gzmigu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://tq.nicolike.cn

[Q07] 删除表
来源：http://mw.szsharing.cn

DROP TABLE IF EXISTS orders;
来源：http://me.haigaiapp.cn

[Q08] 创建普通索引
来源：http://gv.muxihuayi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://yq.wgjwhj.cn

[Q09] 创建唯一索引
来源：http://lt.bookmarksfly.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://km.bookmarksfly.cn

[Q10] 插入单行
来源：http://oc.huanxung.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://lb.haigaiapp.cn

[Q11] 一次插入多行
来源：http://bl.huixinmuqiang.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://nd.huixiangedu.cn

[Q12] 插入后取自增 ID
来源：http://tm.9csxet.cn

INSERT INTO users (name) VALUES ('C');
来源：http://xo.asd995.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ia.521024.cn

[Q13] 忽略重复插入
来源：http://ct.wgjwhj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ta.lnxyls.cn

[Q14] 存在则更新（upsert）
来源：http://xv.hnjuh.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rp.9csxet.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://km.panjiajie.cn

[Q15] 查询全部
来源：http://ls.chemitech.net.cn

SELECT * FROM users;
来源：http://nj.wgjwhj.cn

[Q16] 查询指定列
来源：http://td.panjiajie.cn

SELECT id, name FROM users;
来源：http://zp.asd995.cn

[Q17] 条件查询
来源：http://da.newstarts.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zb.shxzskj.cn

[Q18] 模糊匹配
来源：http://oe.521024.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kv.bookmarksfly.cn

[Q19] 范围查询
来源：http://on.jianghongdianzi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://cs.newstarts.cn

[Q20] IN 列表
来源：http://kp.asd995.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tb.9csxet.cn

[Q21] 空值判断
来源：http://dt.bjjhwx.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://pd.yuntaijiaju.cn

[Q22] 排序
来源：http://nj.szxytkj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gz.szsharing.cn

[Q23] 分页
来源：http://ls.szxytkj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://sj.szsharing.cn

[Q24] 去重
来源：http://an.shtwfgs.cn

SELECT DISTINCT city FROM users;
来源：http://pw.jianghongdianzi.cn

[Q25] 只取前 N 条
来源：http://jx.nszjky.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wf.gzmigu.cn

[Q26] 计数
来源：http://zu.haigaiapp.cn

SELECT COUNT(*) FROM users;
来源：http://po.wgjwhj.cn

[Q27] 条件计数
来源：http://rb.shxzukj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xr.muxihuayi.cn

[Q28] 求和与平均
来源：http://ub.asd995.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lm.bjjhwx.cn

[Q29] 最大最小值
来源：http://pm.nszjky.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ql.huanxung.cn

[Q30] 分组统计
来源：http://em.lnxyls.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://du.nicolike.cn

[Q31] 分组后过滤
来源：http://ph.shtwfgs.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://om.shxzskj.cn

[Q32] 分组拼接字符串
来源：http://ty.chemitech.net.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mi.szxytkj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vw.9csxet.cn

[Q33] 多列分组
来源：http://ln.521024.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dt.jctech888.com.cn

[Q34] 每组取第一条
来源：http://wa.lnxyls.cn

SELECT * FROM (
来源：http://ok.muxihuayi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ed.haigaiapp.cn

) t WHERE rn = 1;
来源：http://ks.bjjhwx.cn

[Q35] 内连接
来源：http://br.haigaiapp.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lg.nicolike.cn

[Q36] 左连接
来源：http://my.muxihuayi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jk.asd995.cn

[Q37] 右连接
来源：http://ej.nicolike.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://eu.lnxyls.cn

[Q38] 全外连接（PostgreSQL）
来源：http://rb.wgjwhj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ui.hnjuh.cn

[Q39] 自连接（查上下级）
来源：http://ey.newstarts.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://jw.hahajie.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ln.jctech888.com.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://rg.wgjwhj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lg.muxihuayi.cn

[Q41] 多表连接
来源：http://yy.szxytkj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://nv.hahajie.cn

JOIN users u ON u.id = o.user_id
来源：http://wb.yuexingan06.cn

JOIN products p ON p.id = o.product_id;
来源：http://bx.asd995.cn

[Q42] 连接条件附加过滤
来源：http://gc.shxzukj.cn

SELECT u.name, o.amount FROM users u
来源：http://vb.nszjky.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yh.nicolike.cn

[Q43] 标量子查询
来源：http://xg.bookmarksfly.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mo.newstarts.cn

[Q44] IN 子查询
来源：http://ab.newstarts.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://kd.hnjuh.cn

[Q45] EXISTS 判断存在
来源：http://fr.wgjwhj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xt.huixinmuqiang.cn

[Q46] NOT EXISTS 判断不存在
来源：http://cm.bookmarksfly.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pm.bookmarksfly.cn

[Q47] 与平均值比较
来源：http://pj.wgjwhj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ww.yuexingan06.cn

[Q48] CTE 公用表表达式
来源：http://gc.wgjwhj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vt.yuexingan06.cn

SELECT * FROM t WHERE c > 5;
来源：http://rc.hnjuh.cn

[Q49] 更新单行
来源：http://js.muxihuayi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ry.bookmarksfly.cn

[Q50] 批量更新
来源：http://im.szsharing.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://nx.newstarts.cn

[Q51] 用子查询更新
来源：http://yz.jianghongdianzi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mz.bookmarksfly.cn

[Q52] 删除指定行
来源：http://vp.521024.cn

DELETE FROM users WHERE id = 10;
来源：http://ff.wgjwhj.cn

[Q53] 按条件删除
来源：http://or.newstarts.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qs.chemitech.net.cn

[Q54] 清空表
来源：http://vs.szxytkj.cn

TRUNCATE TABLE logs;
来源：http://al.shxzskj.cn

[Q55] 排名（并列占位）
来源：http://ab.yuntaijiaju.cn


<!-- 参考信息 -->