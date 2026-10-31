代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dr.newstarts.cn

[N10] 链表节点定义
来源：http://sh.nicolike.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://eg.hnjuh.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://cq.newstarts.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://nb.wgjwhj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ay.nicolike.cn

Java: class Node { int v; Node next; }
来源：http://by.huixiangedu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://gq.shxzukj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://yh.newstarts.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://xp.lnxyls.cn

[N11] 二叉树中序遍历
来源：http://yy.shxzukj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mt.nszjky.cn

PHP:  // 手写递归函数
来源：http://sj.szsharing.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ue.shxzskj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wf.huixinmuqiang.cn

Java: // 手写递归
来源：http://vd.9csxet.cn

Go:   // 手写递归
来源：http://xz.haigaiapp.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://uh.nszjky.cn

C#:   // 手写递归
来源：http://uv.521024.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hh.shxzukj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jj.haigaiapp.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rx.wgjwhj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xf.panjiajie.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yo.huanxung.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hk.hahajie.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nr.yuexingan06.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yn.newstarts.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bl.wgjwhj.cn

================================================================================
来源：http://vh.521024.cn

O. 并发与异步
来源：http://pa.521024.cn

================================================================================
来源：http://pf.9csxet.cn

[O01] 启动一个线程
来源：http://jm.panjiajie.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ly.9csxet.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nu.yuexingan06.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://oi.nszjky.cn

TS:   // 同 JS
来源：http://uy.huixinmuqiang.cn

Java: new Thread(() -> f()).start()
来源：http://gk.panjiajie.cn

Go:   go f()
来源：http://iw.shtwfgs.cn

Ruby: Thread.new { f }
来源：http://ql.chemitech.net.cn

C#:   Task.Run(() => F());
来源：http://hr.shtwfgs.cn

[O02] 使用线程池
来源：http://wa.nicolike.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vk.hnjuh.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dl.shxzskj.cn

JS:   // worker_threads 线程池
来源：http://zc.jianghongdianzi.cn

TS:   // worker_threads 线程池
来源：http://td.nszjky.cn

Java: Executors.newFixedThreadPool(4)
来源：http://pt.panjiajie.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://my.shtwfgs.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gv.wgjwhj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ir.huixinmuqiang.cn

[O03] 加锁保护共享数据
来源：http://fg.jctech888.com.cn

Py:   with lock: shared += 1
来源：http://xc.huixinmuqiang.cn

PHP:  // 用 flock() 做文件锁
来源：http://eb.jctech888.com.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dv.newstarts.cn

TS:   // 同 JS
来源：http://rq.bookmarksfly.cn

Java: synchronized (this) { shared++; }
来源：http://pe.lnxyls.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cv.haigaiapp.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://wl.shtwfgs.cn

C#:   lock (gate) { shared++; }
来源：http://en.yuntaijiaju.cn

[O04] 定义异步函数并等待
来源：http://tb.haigaiapp.cn

Py:   async def f():⏎    await g()
来源：http://ez.nicolike.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://au.newstarts.cn

JS:   async function f() { await g(); }
来源：http://ul.huixiangedu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://yg.nszjky.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ia.shxzukj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cp.huanxung.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ra.lnxyls.cn

C#:   async Task F() { await G(); }
来源：http://il.muxihuayi.cn

[O05] 并发执行并等待全部完成
来源：http://bi.nicolike.cn

Py:   asyncio.gather(*tasks)
来源：http://ao.szxytkj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ms.shxzskj.cn

JS:   await Promise.all(tasks)
来源：http://fc.jianghongdianzi.cn

TS:   await Promise.all(tasks)
来源：http://pn.yuexingan06.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bq.nszjky.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gy.chemitech.net.cn

Ruby: threads.map(&:join)
来源：http://ma.panjiajie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://pr.huanxung.cn

[O06] 使用进程池
来源：http://eg.nszjky.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tm.chemitech.net.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ww.521024.cn

JS:   // child_process / cluster 模块
来源：http://ui.jianghongdianzi.cn

TS:   // child_process / cluster 模块
来源：http://op.newstarts.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gg.szxytkj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mj.wgjwhj.cn

Ruby: // fork 块
来源：http://jw.huanxung.cn

C#:   Parallel.For
来源：http://og.nicolike.cn

================================================================================
来源：http://oe.nicolike.cn

P. 常用工具函数
来源：http://ra.muxihuayi.cn

================================================================================
来源：http://rx.szsharing.cn

[P01] 生成 UUID
来源：http://rd.panjiajie.cn

Py:   str(uuid.uuid4())
来源：http://ox.jianghongdianzi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://yo.521024.cn

JS:   crypto.randomUUID()
来源：http://fm.hahajie.cn

TS:   crypto.randomUUID()
来源：http://vt.nszjky.cn

Java: UUID.randomUUID().toString()
来源：http://qi.haigaiapp.cn

Go:   // 用 github.com/google/uuid
来源：http://zn.nicolike.cn

Ruby: SecureRandom.uuid
来源：http://jm.jianghongdianzi.cn

C#:   Guid.NewGuid().ToString()
来源：http://mg.jctech888.com.cn

[P02] MD5 / SHA256 摘要
来源：http://uc.jianghongdianzi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://tc.colortex.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ez.521024.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://am.hnjuh.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://er.jctech888.com.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bb.yuntaijiaju.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qo.panjiajie.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://it.huanxung.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fy.hnjuh.cn

[P03] 生成短随机字符串
来源：http://oh.colortex.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mu.lnxyls.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hk.9csxet.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lp.yuntaijiaju.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yy.huanxung.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nd.panjiajie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://py.huixinmuqiang.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://yw.shxzukj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zt.szxytkj.cn

[P04] 求长度
来源：http://lg.panjiajie.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://am.colortex.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vc.asd995.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ix.9csxet.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bq.hahajie.cn

Java: list.size();  map.size();  s.length()
来源：http://tj.jctech888.com.cn

Go:   len(arr);  len(m)
来源：http://yt.hnjuh.cn

Ruby: x.length;  x.size
来源：http://bz.asd995.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://fw.colortex.cn

[P05] 判断两个对象内容是否相等
来源：http://zm.hnjuh.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://nu.asd995.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://km.jctech888.com.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qg.shxzukj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ge.hahajie.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://jz.szxytkj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ay.chemitech.net.cn

Ruby: a == b
来源：http://zp.asd995.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://md.shxzukj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://af.szsharing.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://aj.nicolike.cn

PHP:  if (empty($x)) {}
来源：http://wl.colortex.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ge.huixiangedu.cn

TS:   if (x == null) {}
来源：http://gg.jctech888.com.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://zb.huanxung.cn

Go:   if x == nil {}
来源：http://wf.chemitech.net.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://jc.haigaiapp.cn

C#:   if (x is null) {}
来源：http://ry.huixiangedu.cn

[P07] 防抖与节流
来源：http://ht.lnxyls.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://my.huixinmuqiang.cn

PHP:  // 手写时间戳比较
来源：http://gx.bjjhwx.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://on.yuexingan06.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rf.panjiajie.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://eb.szsharing.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fj.haigaiapp.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://jl.newstarts.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mr.huixinmuqiang.cn

[P08] 处理浮点精度问题
来源：http://kz.nicolike.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vm.shxzukj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ds.shxzskj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ul.yuntaijiaju.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lw.shtwfgs.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pw.muxihuayi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://sz.hnjuh.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gv.szxytkj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jy.9csxet.cn

================================================================================
来源：http://rh.jianghongdianzi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://bd.huixiangedu.cn

================================================================================
来源：http://sh.asd995.cn

[Q01] 创建表
来源：http://lj.yuntaijiaju.cn

CREATE TABLE users (
来源：http://oz.huanxung.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://lu.nszjky.cn

name VARCHAR(50) NOT NULL,
来源：http://ry.wgjwhj.cn

email VARCHAR(100) UNIQUE,
来源：http://mc.huixiangedu.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hm.colortex.cn

);
来源：http://bi.szxytkj.cn

[Q02] 创建带外键的表
来源：http://ko.9csxet.cn

CREATE TABLE orders (
来源：http://io.jianghongdianzi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ll.chemitech.net.cn

user_id INT NOT NULL,
来源：http://oa.hnjuh.cn

amount DECIMAL(10, 2),
来源：http://ug.szsharing.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://cy.hnjuh.cn

);
来源：http://td.chemitech.net.cn

[Q03] 增加列
来源：http://we.chemitech.net.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://iz.hahajie.cn

[Q04] 修改列类型
来源：http://rw.hnjuh.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cb.muxihuayi.cn

[Q05] 重命名列
来源：http://va.shxzukj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://tj.chemitech.net.cn

[Q06] 删除列
来源：http://od.jctech888.com.cn

ALTER TABLE users DROP COLUMN age;
来源：http://be.szxytkj.cn

[Q07] 删除表
来源：http://dq.shtwfgs.cn

DROP TABLE IF EXISTS orders;
来源：http://od.huanxung.cn

[Q08] 创建普通索引
来源：http://ey.lnxyls.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://bl.shxzukj.cn

[Q09] 创建唯一索引
来源：http://uf.huixiangedu.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://up.haigaiapp.cn

[Q10] 插入单行
来源：http://fx.haigaiapp.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://rm.haigaiapp.cn

[Q11] 一次插入多行
来源：http://kv.yuntaijiaju.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ff.wgjwhj.cn

[Q12] 插入后取自增 ID
来源：http://ok.newstarts.cn

INSERT INTO users (name) VALUES ('C');
来源：http://gg.szsharing.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://bp.panjiajie.cn

[Q13] 忽略重复插入
来源：http://wj.9csxet.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ab.hnjuh.cn

[Q14] 存在则更新（upsert）
来源：http://du.jianghongdianzi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://tz.9csxet.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ja.colortex.cn

[Q15] 查询全部
来源：http://rv.bjjhwx.cn

SELECT * FROM users;
来源：http://fp.nicolike.cn

[Q16] 查询指定列
来源：http://vo.wgjwhj.cn

SELECT id, name FROM users;
来源：http://sv.jctech888.com.cn

[Q17] 条件查询
来源：http://uv.chemitech.net.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://bd.yuntaijiaju.cn

[Q18] 模糊匹配
来源：http://on.shxzskj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://iw.huixiangedu.cn

[Q19] 范围查询
来源：http://in.muxihuayi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qj.hahajie.cn

[Q20] IN 列表
来源：http://ae.colortex.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://eo.yuntaijiaju.cn

[Q21] 空值判断
来源：http://ft.huanxung.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://jc.colortex.cn

[Q22] 排序
来源：http://cy.hnjuh.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tc.yuntaijiaju.cn

[Q23] 分页
来源：http://zb.521024.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ns.gzmigu.cn

[Q24] 去重
来源：http://of.nicolike.cn

SELECT DISTINCT city FROM users;
来源：http://ap.newstarts.cn

[Q25] 只取前 N 条
来源：http://mf.huixinmuqiang.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hp.asd995.cn

[Q26] 计数
来源：http://tg.huixiangedu.cn

SELECT COUNT(*) FROM users;
来源：http://hx.hnjuh.cn

[Q27] 条件计数
来源：http://yi.szsharing.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qn.yuexingan06.cn

[Q28] 求和与平均
来源：http://be.shtwfgs.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://gz.wgjwhj.cn

[Q29] 最大最小值
来源：http://xn.huanxung.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://dd.muxihuayi.cn

[Q30] 分组统计
来源：http://bl.shtwfgs.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wy.huanxung.cn

[Q31] 分组后过滤
来源：http://cl.newstarts.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ey.lnxyls.cn

[Q32] 分组拼接字符串
来源：http://vm.shtwfgs.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ng.shxzskj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gx.haigaiapp.cn

[Q33] 多列分组
来源：http://un.chemitech.net.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gh.jianghongdianzi.cn

[Q34] 每组取第一条
来源：http://ym.yuntaijiaju.cn

SELECT * FROM (
来源：http://ed.yuexingan06.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://sk.wgjwhj.cn

) t WHERE rn = 1;
来源：http://vz.9csxet.cn

[Q35] 内连接
来源：http://xv.jctech888.com.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ny.hahajie.cn

[Q36] 左连接
来源：http://hn.gzmigu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mf.jianghongdianzi.cn

[Q37] 右连接
来源：http://os.colortex.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qw.lnxyls.cn

[Q38] 全外连接（PostgreSQL）
来源：http://jv.yuexingan06.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jz.panjiajie.cn

[Q39] 自连接（查上下级）
来源：http://jt.gzmigu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://tf.huixiangedu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://pf.wgjwhj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://pd.gzmigu.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ny.wgjwhj.cn

[Q41] 多表连接
来源：http://vx.wgjwhj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://kc.panjiajie.cn

JOIN users u ON u.id = o.user_id
来源：http://gf.huixinmuqiang.cn

JOIN products p ON p.id = o.product_id;
来源：http://ej.bjjhwx.cn

[Q42] 连接条件附加过滤
来源：http://fo.muxihuayi.cn

SELECT u.name, o.amount FROM users u
来源：http://iy.lnxyls.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://du.yuexingan06.cn

[Q43] 标量子查询
来源：http://sk.wgjwhj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qs.gzmigu.cn

[Q44] IN 子查询
来源：http://cg.yuexingan06.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ao.asd995.cn

[Q45] EXISTS 判断存在
来源：http://mt.bjjhwx.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://br.chemitech.net.cn

[Q46] NOT EXISTS 判断不存在
来源：http://zx.panjiajie.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jn.jianghongdianzi.cn

[Q47] 与平均值比较
来源：http://hg.521024.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ut.colortex.cn

[Q48] CTE 公用表表达式
来源：http://ce.hahajie.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://iw.nszjky.cn

SELECT * FROM t WHERE c > 5;
来源：http://fw.wgjwhj.cn

[Q49] 更新单行
来源：http://zh.shxzukj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zn.nicolike.cn

[Q50] 批量更新
来源：http://rf.yuexingan06.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mg.yuexingan06.cn

[Q51] 用子查询更新
来源：http://hn.yuexingan06.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://tf.wgjwhj.cn

[Q52] 删除指定行
来源：http://nk.bjjhwx.cn

DELETE FROM users WHERE id = 10;
来源：http://pk.jctech888.com.cn

[Q53] 按条件删除
来源：http://bx.shxzskj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ah.hahajie.cn

[Q54] 清空表
来源：http://ag.lnxyls.cn

TRUNCATE TABLE logs;
来源：http://as.chemitech.net.cn

[Q55] 排名（并列占位）
来源：http://vl.shxzukj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hu.hahajie.cn

[Q56] 密集排名（并列不占位）
来源：http://lb.jianghongdianzi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://oe.yuntaijiaju.cn

[Q57] 行号
来源：http://rn.jianghongdianzi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ca.wgjwhj.cn

[Q58] 累计求和
来源：http://rq.szxytkj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ri.lnxyls.cn

[Q59] 分组内累计
来源：http://pf.bookmarksfly.cn


<!-- 参考信息 -->