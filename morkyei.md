代发 wailian999

[N09] 栈与队列
来源：http://cs.haigaiapp.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://og.haigaiapp.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fz.szxytkj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://uw.szxytkj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fu.jctech888.com.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vi.szxytkj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://iu.wgjwhj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ny.9csxet.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bn.yuexingan06.cn

[N10] 链表节点定义
来源：http://bx.shxzskj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lg.asd995.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://za.shxzskj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ic.chemitech.net.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ag.bjjhwx.cn

Java: class Node { int v; Node next; }
来源：http://gj.yuexingan06.cn

Go:   type Node struct { V int; Next *Node }
来源：http://lr.haigaiapp.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://tj.lnxyls.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://xl.huixinmuqiang.cn

[N11] 二叉树中序遍历
来源：http://du.szsharing.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lf.bookmarksfly.cn

PHP:  // 手写递归函数
来源：http://cd.wgjwhj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ue.yuntaijiaju.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zc.haigaiapp.cn

Java: // 手写递归
来源：http://ul.colortex.cn

Go:   // 手写递归
来源：http://lp.szxytkj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kt.chemitech.net.cn

C#:   // 手写递归
来源：http://gf.huanxung.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wh.gzmigu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://px.huixiangedu.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://nu.9csxet.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fs.lnxyls.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nm.jctech888.com.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://rn.jctech888.com.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://le.gzmigu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ea.yuexingan06.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://li.chemitech.net.cn

================================================================================
来源：http://hd.nszjky.cn

O. 并发与异步
来源：http://gb.asd995.cn

================================================================================
来源：http://wd.521024.cn

[O01] 启动一个线程
来源：http://wp.shxzskj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ml.szsharing.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jk.panjiajie.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ng.yuntaijiaju.cn

TS:   // 同 JS
来源：http://hl.asd995.cn

Java: new Thread(() -> f()).start()
来源：http://oz.chemitech.net.cn

Go:   go f()
来源：http://en.colortex.cn

Ruby: Thread.new { f }
来源：http://cq.panjiajie.cn

C#:   Task.Run(() => F());
来源：http://ga.szsharing.cn

[O02] 使用线程池
来源：http://bh.hnjuh.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qh.9csxet.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rd.nicolike.cn

JS:   // worker_threads 线程池
来源：http://wd.asd995.cn

TS:   // worker_threads 线程池
来源：http://ud.jctech888.com.cn

Java: Executors.newFixedThreadPool(4)
来源：http://bf.szxytkj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://gq.haigaiapp.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tg.9csxet.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ey.gzmigu.cn

[O03] 加锁保护共享数据
来源：http://db.jianghongdianzi.cn

Py:   with lock: shared += 1
来源：http://is.521024.cn

PHP:  // 用 flock() 做文件锁
来源：http://nu.jctech888.com.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xd.hahajie.cn

TS:   // 同 JS
来源：http://ve.newstarts.cn

Java: synchronized (this) { shared++; }
来源：http://jf.szxytkj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://md.asd995.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://fz.gzmigu.cn

C#:   lock (gate) { shared++; }
来源：http://rl.huixinmuqiang.cn

[O04] 定义异步函数并等待
来源：http://gx.shxzukj.cn

Py:   async def f():⏎    await g()
来源：http://zb.jianghongdianzi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yg.muxihuayi.cn

JS:   async function f() { await g(); }
来源：http://pz.asd995.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.9csxet.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vu.szxytkj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ne.shxzukj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ut.huixinmuqiang.cn

C#:   async Task F() { await G(); }
来源：http://yc.panjiajie.cn

[O05] 并发执行并等待全部完成
来源：http://kp.wgjwhj.cn

Py:   asyncio.gather(*tasks)
来源：http://rb.asd995.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cx.asd995.cn

JS:   await Promise.all(tasks)
来源：http://zq.nicolike.cn

TS:   await Promise.all(tasks)
来源：http://lq.huixinmuqiang.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://sa.szsharing.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ra.lnxyls.cn

Ruby: threads.map(&:join)
来源：http://ul.huixinmuqiang.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://zl.jctech888.com.cn

[O06] 使用进程池
来源：http://er.hnjuh.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jz.bjjhwx.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://jb.nszjky.cn

JS:   // child_process / cluster 模块
来源：http://go.shxzukj.cn

TS:   // child_process / cluster 模块
来源：http://kg.muxihuayi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vj.yuntaijiaju.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ib.shxzukj.cn

Ruby: // fork 块
来源：http://hv.huixiangedu.cn

C#:   Parallel.For
来源：http://ew.panjiajie.cn

================================================================================
来源：http://uc.szsharing.cn

P. 常用工具函数
来源：http://qg.szsharing.cn

================================================================================
来源：http://ru.huixiangedu.cn

[P01] 生成 UUID
来源：http://bm.szxytkj.cn

Py:   str(uuid.uuid4())
来源：http://wo.shxzukj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gs.asd995.cn

JS:   crypto.randomUUID()
来源：http://ac.shxzskj.cn

TS:   crypto.randomUUID()
来源：http://ms.szsharing.cn

Java: UUID.randomUUID().toString()
来源：http://hd.chemitech.net.cn

Go:   // 用 github.com/google/uuid
来源：http://nr.szsharing.cn

Ruby: SecureRandom.uuid
来源：http://yd.hnjuh.cn

C#:   Guid.NewGuid().ToString()
来源：http://ig.bookmarksfly.cn

[P02] MD5 / SHA256 摘要
来源：http://xc.nszjky.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mz.hnjuh.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ja.colortex.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hp.jianghongdianzi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ta.hahajie.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vv.haigaiapp.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://iu.lnxyls.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fp.yuexingan06.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gn.nszjky.cn

[P03] 生成短随机字符串
来源：http://ah.newstarts.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ce.hnjuh.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hc.yuntaijiaju.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gd.nicolike.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://si.jianghongdianzi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://en.chemitech.net.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ga.9csxet.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ry.asd995.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://bh.bookmarksfly.cn

[P04] 求长度
来源：http://gl.9csxet.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ir.asd995.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://aj.gzmigu.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ip.yuntaijiaju.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nj.jianghongdianzi.cn

Java: list.size();  map.size();  s.length()
来源：http://tw.muxihuayi.cn

Go:   len(arr);  len(m)
来源：http://ey.hnjuh.cn

Ruby: x.length;  x.size
来源：http://rd.jianghongdianzi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://zv.hnjuh.cn

[P05] 判断两个对象内容是否相等
来源：http://tr.muxihuayi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://lh.bjjhwx.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mz.gzmigu.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vv.bookmarksfly.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://sa.shtwfgs.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://so.szsharing.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ml.nszjky.cn

Ruby: a == b
来源：http://ad.lnxyls.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tx.yuexingan06.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ir.panjiajie.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://rh.wgjwhj.cn

PHP:  if (empty($x)) {}
来源：http://bs.bjjhwx.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://si.hnjuh.cn

TS:   if (x == null) {}
来源：http://hv.shtwfgs.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ma.newstarts.cn

Go:   if x == nil {}
来源：http://ug.hahajie.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://uj.shtwfgs.cn

C#:   if (x is null) {}
来源：http://cc.lnxyls.cn

[P07] 防抖与节流
来源：http://fb.hahajie.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bv.bookmarksfly.cn

PHP:  // 手写时间戳比较
来源：http://xc.shxzukj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://km.nszjky.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lp.521024.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://el.szsharing.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dr.nszjky.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://gt.chemitech.net.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://pf.bookmarksfly.cn

[P08] 处理浮点精度问题
来源：http://hg.nszjky.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ue.shtwfgs.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://pz.chemitech.net.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xp.colortex.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://st.bjjhwx.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://su.huanxung.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jn.gzmigu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://yq.nszjky.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rm.nicolike.cn

================================================================================
来源：http://ir.chemitech.net.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://bh.asd995.cn

================================================================================
来源：http://zv.bookmarksfly.cn

[Q01] 创建表
来源：http://ex.huixiangedu.cn

CREATE TABLE users (
来源：http://hn.hahajie.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://lp.huixiangedu.cn

name VARCHAR(50) NOT NULL,
来源：http://cx.jctech888.com.cn

email VARCHAR(100) UNIQUE,
来源：http://kx.muxihuayi.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://pn.yuexingan06.cn

);
来源：http://by.bookmarksfly.cn

[Q02] 创建带外键的表
来源：http://cy.panjiajie.cn

CREATE TABLE orders (
来源：http://nv.huanxung.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kc.wgjwhj.cn

user_id INT NOT NULL,
来源：http://da.shxzskj.cn

amount DECIMAL(10, 2),
来源：http://jc.colortex.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://lr.wgjwhj.cn

);
来源：http://fy.panjiajie.cn

[Q03] 增加列
来源：http://go.jianghongdianzi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lm.shtwfgs.cn

[Q04] 修改列类型
来源：http://tr.jianghongdianzi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jx.shxzskj.cn

[Q05] 重命名列
来源：http://ei.lnxyls.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hb.haigaiapp.cn

[Q06] 删除列
来源：http://sa.nszjky.cn

ALTER TABLE users DROP COLUMN age;
来源：http://sc.szsharing.cn

[Q07] 删除表
来源：http://lb.chemitech.net.cn

DROP TABLE IF EXISTS orders;
来源：http://wb.jianghongdianzi.cn

[Q08] 创建普通索引
来源：http://kj.gzmigu.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://tl.jctech888.com.cn

[Q09] 创建唯一索引
来源：http://sp.szxytkj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vc.wgjwhj.cn

[Q10] 插入单行
来源：http://sp.chemitech.net.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hm.haigaiapp.cn

[Q11] 一次插入多行
来源：http://dj.jctech888.com.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://yt.haigaiapp.cn

[Q12] 插入后取自增 ID
来源：http://uj.huixiangedu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://pm.huixinmuqiang.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ei.shtwfgs.cn

[Q13] 忽略重复插入
来源：http://fw.colortex.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://bo.9csxet.cn

[Q14] 存在则更新（upsert）
来源：http://lz.yuexingan06.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://qd.newstarts.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fu.hnjuh.cn

[Q15] 查询全部
来源：http://pg.szsharing.cn

SELECT * FROM users;
来源：http://fi.shtwfgs.cn

[Q16] 查询指定列
来源：http://ey.shxzukj.cn

SELECT id, name FROM users;
来源：http://oj.yuexingan06.cn

[Q17] 条件查询
来源：http://sf.szsharing.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kg.shxzskj.cn

[Q18] 模糊匹配
来源：http://rd.shtwfgs.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://an.bookmarksfly.cn

[Q19] 范围查询
来源：http://hh.szsharing.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gr.gzmigu.cn

[Q20] IN 列表
来源：http://ar.yuntaijiaju.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://lu.haigaiapp.cn

[Q21] 空值判断
来源：http://ou.szsharing.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ih.shxzskj.cn

[Q22] 排序
来源：http://qc.shxzskj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qr.jctech888.com.cn

[Q23] 分页
来源：http://so.huixiangedu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dl.shtwfgs.cn

[Q24] 去重
来源：http://mr.szxytkj.cn

SELECT DISTINCT city FROM users;
来源：http://dh.asd995.cn

[Q25] 只取前 N 条
来源：http://ah.szsharing.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wm.shxzskj.cn

[Q26] 计数
来源：http://vn.jctech888.com.cn

SELECT COUNT(*) FROM users;
来源：http://qn.wgjwhj.cn

[Q27] 条件计数
来源：http://oj.newstarts.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://nk.shtwfgs.cn

[Q28] 求和与平均
来源：http://xh.bjjhwx.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://co.hnjuh.cn

[Q29] 最大最小值
来源：http://ax.wgjwhj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://gd.panjiajie.cn

[Q30] 分组统计
来源：http://ad.bookmarksfly.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://en.jianghongdianzi.cn

[Q31] 分组后过滤
来源：http://pc.szsharing.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://aw.szxytkj.cn

[Q32] 分组拼接字符串
来源：http://th.hahajie.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wa.jctech888.com.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://le.huixiangedu.cn

[Q33] 多列分组
来源：http://wy.colortex.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rk.huixinmuqiang.cn

[Q34] 每组取第一条
来源：http://hf.hahajie.cn

SELECT * FROM (
来源：http://sk.hnjuh.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ix.szxytkj.cn

) t WHERE rn = 1;
来源：http://lj.huixiangedu.cn

[Q35] 内连接
来源：http://rt.shtwfgs.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gn.panjiajie.cn

[Q36] 左连接
来源：http://fo.9csxet.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pl.muxihuayi.cn

[Q37] 右连接
来源：http://in.shtwfgs.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://os.szxytkj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://fl.9csxet.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zp.jctech888.com.cn

[Q39] 自连接（查上下级）
来源：http://dg.huixiangedu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://io.huixinmuqiang.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://se.wgjwhj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://he.szsharing.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pa.colortex.cn

[Q41] 多表连接
来源：http://rc.yuexingan06.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://nr.asd995.cn

JOIN users u ON u.id = o.user_id
来源：http://tz.huixiangedu.cn

JOIN products p ON p.id = o.product_id;
来源：http://fp.shxzskj.cn

[Q42] 连接条件附加过滤
来源：http://ow.521024.cn

SELECT u.name, o.amount FROM users u
来源：http://qw.szsharing.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://si.jctech888.com.cn

[Q43] 标量子查询
来源：http://jv.haigaiapp.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://tk.521024.cn

[Q44] IN 子查询
来源：http://bl.panjiajie.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://sn.yuntaijiaju.cn

[Q45] EXISTS 判断存在
来源：http://lr.9csxet.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dh.bjjhwx.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ea.jctech888.com.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ga.huixinmuqiang.cn

[Q47] 与平均值比较
来源：http://xy.bjjhwx.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://zr.nicolike.cn

[Q48] CTE 公用表表达式
来源：http://ln.shxzskj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xf.shtwfgs.cn

SELECT * FROM t WHERE c > 5;
来源：http://qo.nicolike.cn

[Q49] 更新单行
来源：http://ar.nicolike.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xo.huixinmuqiang.cn

[Q50] 批量更新
来源：http://af.bookmarksfly.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xn.huixinmuqiang.cn

[Q51] 用子查询更新
来源：http://pq.521024.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://nn.shtwfgs.cn

[Q52] 删除指定行
来源：http://wg.nszjky.cn

DELETE FROM users WHERE id = 10;
来源：http://bg.huanxung.cn

[Q53] 按条件删除
来源：http://qv.asd995.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mz.shtwfgs.cn

[Q54] 清空表
来源：http://kz.jctech888.com.cn

TRUNCATE TABLE logs;
来源：http://vg.muxihuayi.cn

[Q55] 排名（并列占位）
来源：http://ou.muxihuayi.cn


<!-- 参考信息 -->