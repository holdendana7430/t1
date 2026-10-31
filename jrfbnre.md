代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hp.newstarts.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zm.huixiangedu.cn

Java: class Node { int v; Node next; }
来源：http://jm.yuntaijiaju.cn

Go:   type Node struct { V int; Next *Node }
来源：http://vx.nszjky.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://dc.szsharing.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://cc.szxytkj.cn

[N11] 二叉树中序遍历
来源：http://ub.huixinmuqiang.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jo.newstarts.cn

PHP:  // 手写递归函数
来源：http://pr.lnxyls.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zu.521024.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zn.chemitech.net.cn

Java: // 手写递归
来源：http://hr.newstarts.cn

Go:   // 手写递归
来源：http://oa.jctech888.com.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xp.szsharing.cn

C#:   // 手写递归
来源：http://rk.hahajie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cy.muxihuayi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://nn.huanxung.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rw.hahajie.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ms.chemitech.net.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hi.newstarts.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://cy.muxihuayi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://it.shxzukj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vm.nicolike.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://oc.chemitech.net.cn

================================================================================
来源：http://ul.szsharing.cn

O. 并发与异步
来源：http://vn.muxihuayi.cn

================================================================================
来源：http://je.shtwfgs.cn

[O01] 启动一个线程
来源：http://do.jctech888.com.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ug.gzmigu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ei.panjiajie.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qf.hahajie.cn

TS:   // 同 JS
来源：http://ow.gzmigu.cn

Java: new Thread(() -> f()).start()
来源：http://rv.lnxyls.cn

Go:   go f()
来源：http://kh.wgjwhj.cn

Ruby: Thread.new { f }
来源：http://uc.yuexingan06.cn

C#:   Task.Run(() => F());
来源：http://xd.huixinmuqiang.cn

[O02] 使用线程池
来源：http://yy.jctech888.com.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cw.yuexingan06.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://tt.szsharing.cn

JS:   // worker_threads 线程池
来源：http://kf.newstarts.cn

TS:   // worker_threads 线程池
来源：http://rb.panjiajie.cn

Java: Executors.newFixedThreadPool(4)
来源：http://jo.muxihuayi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vx.shtwfgs.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ax.yuntaijiaju.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ho.szsharing.cn

[O03] 加锁保护共享数据
来源：http://aw.nszjky.cn

Py:   with lock: shared += 1
来源：http://di.lnxyls.cn

PHP:  // 用 flock() 做文件锁
来源：http://sf.521024.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ja.yuexingan06.cn

TS:   // 同 JS
来源：http://vv.colortex.cn

Java: synchronized (this) { shared++; }
来源：http://dz.haigaiapp.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sq.huanxung.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://rp.newstarts.cn

C#:   lock (gate) { shared++; }
来源：http://vr.panjiajie.cn

[O04] 定义异步函数并等待
来源：http://bh.newstarts.cn

Py:   async def f():⏎    await g()
来源：http://it.huixiangedu.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rx.nszjky.cn

JS:   async function f() { await g(); }
来源：http://jm.wgjwhj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ez.colortex.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xg.shxzskj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://oz.hahajie.cn

Ruby: # 用 Fiber 或 async gem
来源：http://yh.szxytkj.cn

C#:   async Task F() { await G(); }
来源：http://rv.521024.cn

[O05] 并发执行并等待全部完成
来源：http://ew.wgjwhj.cn

Py:   asyncio.gather(*tasks)
来源：http://iy.nszjky.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rr.haigaiapp.cn

JS:   await Promise.all(tasks)
来源：http://xh.szsharing.cn

TS:   await Promise.all(tasks)
来源：http://rs.9csxet.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rz.bookmarksfly.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nb.wgjwhj.cn

Ruby: threads.map(&:join)
来源：http://wb.hahajie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://xu.haigaiapp.cn

[O06] 使用进程池
来源：http://ih.nicolike.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zc.huixinmuqiang.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://in.hahajie.cn

JS:   // child_process / cluster 模块
来源：http://wd.521024.cn

TS:   // child_process / cluster 模块
来源：http://ne.nicolike.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://yr.bookmarksfly.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://pa.shtwfgs.cn

Ruby: // fork 块
来源：http://mv.wgjwhj.cn

C#:   Parallel.For
来源：http://dp.chemitech.net.cn

================================================================================
来源：http://mw.hnjuh.cn

P. 常用工具函数
来源：http://yv.9csxet.cn

================================================================================
来源：http://ll.shxzukj.cn

[P01] 生成 UUID
来源：http://uv.yuexingan06.cn

Py:   str(uuid.uuid4())
来源：http://jf.jctech888.com.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hq.bjjhwx.cn

JS:   crypto.randomUUID()
来源：http://ly.huixinmuqiang.cn

TS:   crypto.randomUUID()
来源：http://gw.szxytkj.cn

Java: UUID.randomUUID().toString()
来源：http://pj.bjjhwx.cn

Go:   // 用 github.com/google/uuid
来源：http://fh.wgjwhj.cn

Ruby: SecureRandom.uuid
来源：http://xe.lnxyls.cn

C#:   Guid.NewGuid().ToString()
来源：http://et.haigaiapp.cn

[P02] MD5 / SHA256 摘要
来源：http://ip.haigaiapp.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zc.lnxyls.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://hc.szsharing.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bw.bjjhwx.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://yv.jctech888.com.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qk.nicolike.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xk.wgjwhj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vp.jctech888.com.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hn.huixinmuqiang.cn

[P03] 生成短随机字符串
来源：http://bq.wgjwhj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hm.bjjhwx.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vg.nicolike.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ka.9csxet.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kf.shxzskj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xo.9csxet.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bj.wgjwhj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ds.bookmarksfly.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://pp.bookmarksfly.cn

[P04] 求长度
来源：http://vu.szsharing.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ad.lnxyls.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://af.huixinmuqiang.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lf.nicolike.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ob.gzmigu.cn

Java: list.size();  map.size();  s.length()
来源：http://ho.muxihuayi.cn

Go:   len(arr);  len(m)
来源：http://tn.huanxung.cn

Ruby: x.length;  x.size
来源：http://qu.jctech888.com.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://cm.nszjky.cn

[P05] 判断两个对象内容是否相等
来源：http://iq.yuexingan06.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://rr.szxytkj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ly.huanxung.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ef.asd995.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vp.bjjhwx.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hx.muxihuayi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://gl.huixinmuqiang.cn

Ruby: a == b
来源：http://aa.muxihuayi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://kd.hnjuh.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://pz.nszjky.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gk.jctech888.com.cn

PHP:  if (empty($x)) {}
来源：http://id.nszjky.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xv.huixiangedu.cn

TS:   if (x == null) {}
来源：http://bz.newstarts.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://fk.wgjwhj.cn

Go:   if x == nil {}
来源：http://ca.huixiangedu.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://be.nicolike.cn

C#:   if (x is null) {}
来源：http://hd.muxihuayi.cn

[P07] 防抖与节流
来源：http://vr.bjjhwx.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://af.colortex.cn

PHP:  // 手写时间戳比较
来源：http://ce.gzmigu.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pq.bjjhwx.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lo.yuexingan06.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wm.huixiangedu.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://gk.panjiajie.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://fb.huixiangedu.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lm.jctech888.com.cn

[P08] 处理浮点精度问题
来源：http://rr.shxzskj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hw.9csxet.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jc.newstarts.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://rh.hnjuh.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mx.nszjky.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://sl.lnxyls.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nw.newstarts.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://in.jctech888.com.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xe.jianghongdianzi.cn

================================================================================
来源：http://fn.jianghongdianzi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://aw.colortex.cn

================================================================================
来源：http://ba.muxihuayi.cn

[Q01] 创建表
来源：http://gg.asd995.cn

CREATE TABLE users (
来源：http://pm.newstarts.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ew.asd995.cn

name VARCHAR(50) NOT NULL,
来源：http://uz.yuexingan06.cn

email VARCHAR(100) UNIQUE,
来源：http://an.shxzukj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bf.asd995.cn

);
来源：http://xk.wgjwhj.cn

[Q02] 创建带外键的表
来源：http://bu.9csxet.cn

CREATE TABLE orders (
来源：http://hi.szsharing.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://cy.huanxung.cn

user_id INT NOT NULL,
来源：http://sm.gzmigu.cn

amount DECIMAL(10, 2),
来源：http://be.9csxet.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://sl.gzmigu.cn

);
来源：http://wy.chemitech.net.cn

[Q03] 增加列
来源：http://gy.newstarts.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bv.huixinmuqiang.cn

[Q04] 修改列类型
来源：http://ez.huixiangedu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dn.gzmigu.cn

[Q05] 重命名列
来源：http://qo.jianghongdianzi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ju.bjjhwx.cn

[Q06] 删除列
来源：http://bz.chemitech.net.cn

ALTER TABLE users DROP COLUMN age;
来源：http://fn.szxytkj.cn

[Q07] 删除表
来源：http://oa.hahajie.cn

DROP TABLE IF EXISTS orders;
来源：http://zz.wgjwhj.cn

[Q08] 创建普通索引
来源：http://hd.colortex.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ac.chemitech.net.cn

[Q09] 创建唯一索引
来源：http://hg.shxzskj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zw.jctech888.com.cn

[Q10] 插入单行
来源：http://wa.jianghongdianzi.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://pr.jctech888.com.cn

[Q11] 一次插入多行
来源：http://dy.haigaiapp.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ia.muxihuayi.cn

[Q12] 插入后取自增 ID
来源：http://yf.hahajie.cn

INSERT INTO users (name) VALUES ('C');
来源：http://mm.huixinmuqiang.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ws.wgjwhj.cn

[Q13] 忽略重复插入
来源：http://tm.jctech888.com.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ga.szxytkj.cn

[Q14] 存在则更新（upsert）
来源：http://ak.shtwfgs.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://uw.nicolike.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pb.shtwfgs.cn

[Q15] 查询全部
来源：http://wi.gzmigu.cn

SELECT * FROM users;
来源：http://im.shtwfgs.cn

[Q16] 查询指定列
来源：http://dr.szsharing.cn

SELECT id, name FROM users;
来源：http://mc.chemitech.net.cn

[Q17] 条件查询
来源：http://rn.yuntaijiaju.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://sb.shxzskj.cn

[Q18] 模糊匹配
来源：http://my.bookmarksfly.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dz.jianghongdianzi.cn

[Q19] 范围查询
来源：http://zp.nszjky.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ss.gzmigu.cn

[Q20] IN 列表
来源：http://zo.bjjhwx.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wq.newstarts.cn

[Q21] 空值判断
来源：http://ib.wgjwhj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://rd.shtwfgs.cn

[Q22] 排序
来源：http://nv.hahajie.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bi.9csxet.cn

[Q23] 分页
来源：http://kq.panjiajie.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://um.huixinmuqiang.cn

[Q24] 去重
来源：http://ez.yuntaijiaju.cn

SELECT DISTINCT city FROM users;
来源：http://qf.shtwfgs.cn

[Q25] 只取前 N 条
来源：http://js.nicolike.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://nv.hnjuh.cn

[Q26] 计数
来源：http://dw.shxzskj.cn

SELECT COUNT(*) FROM users;
来源：http://xc.hahajie.cn

[Q27] 条件计数
来源：http://hz.haigaiapp.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ar.huixiangedu.cn

[Q28] 求和与平均
来源：http://az.muxihuayi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ml.hnjuh.cn

[Q29] 最大最小值
来源：http://xv.huixiangedu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ik.colortex.cn

[Q30] 分组统计
来源：http://cf.huanxung.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://be.muxihuayi.cn

[Q31] 分组后过滤
来源：http://cq.huixiangedu.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yh.huixinmuqiang.cn

[Q32] 分组拼接字符串
来源：http://ox.wgjwhj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://uw.szsharing.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fi.hnjuh.cn

[Q33] 多列分组
来源：http://wv.hnjuh.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://sb.gzmigu.cn

[Q34] 每组取第一条
来源：http://zf.nszjky.cn

SELECT * FROM (
来源：http://xm.jianghongdianzi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://kp.colortex.cn

) t WHERE rn = 1;
来源：http://ts.huanxung.cn

[Q35] 内连接
来源：http://gr.nszjky.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://sn.haigaiapp.cn

[Q36] 左连接
来源：http://lw.yuexingan06.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://rd.szsharing.cn

[Q37] 右连接
来源：http://gp.huixinmuqiang.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tg.bjjhwx.cn

[Q38] 全外连接（PostgreSQL）
来源：http://jy.shtwfgs.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ub.huanxung.cn

[Q39] 自连接（查上下级）
来源：http://fj.huixinmuqiang.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://vi.asd995.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xe.hahajie.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://gg.hnjuh.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xo.shxzskj.cn

[Q41] 多表连接
来源：http://oh.hnjuh.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://pu.gzmigu.cn

JOIN users u ON u.id = o.user_id
来源：http://ll.lnxyls.cn

JOIN products p ON p.id = o.product_id;
来源：http://py.huanxung.cn

[Q42] 连接条件附加过滤
来源：http://ws.shxzukj.cn

SELECT u.name, o.amount FROM users u
来源：http://kq.szsharing.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zc.yuntaijiaju.cn

[Q43] 标量子查询
来源：http://ux.shxzskj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xh.shxzskj.cn

[Q44] IN 子查询
来源：http://ns.shxzskj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wk.haigaiapp.cn

[Q45] EXISTS 判断存在
来源：http://ef.jianghongdianzi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wa.haigaiapp.cn

[Q46] NOT EXISTS 判断不存在
来源：http://gk.haigaiapp.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bo.yuexingan06.cn

[Q47] 与平均值比较
来源：http://xr.huixiangedu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ir.lnxyls.cn

[Q48] CTE 公用表表达式
来源：http://je.huixinmuqiang.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pk.yuntaijiaju.cn

SELECT * FROM t WHERE c > 5;
来源：http://dg.huixiangedu.cn

[Q49] 更新单行
来源：http://ly.asd995.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://eo.bookmarksfly.cn

[Q50] 批量更新
来源：http://ym.shxzskj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ej.hnjuh.cn

[Q51] 用子查询更新
来源：http://xx.panjiajie.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://gq.nszjky.cn

[Q52] 删除指定行
来源：http://yc.colortex.cn

DELETE FROM users WHERE id = 10;
来源：http://uz.jctech888.com.cn

[Q53] 按条件删除
来源：http://zy.panjiajie.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://bd.jctech888.com.cn

[Q54] 清空表
来源：http://tc.yuntaijiaju.cn

TRUNCATE TABLE logs;
来源：http://ua.yuntaijiaju.cn

[Q55] 排名（并列占位）
来源：http://bv.newstarts.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qt.colortex.cn

[Q56] 密集排名（并列不占位）
来源：http://gx.shxzukj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://te.9csxet.cn

[Q57] 行号
来源：http://zy.jctech888.com.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dt.hnjuh.cn

[Q58] 累计求和
来源：http://iv.bjjhwx.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ug.yuntaijiaju.cn

[Q59] 分组内累计
来源：http://be.9csxet.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://tl.huanxung.cn

[Q60] 取上一行 / 下一行
来源：http://sk.colortex.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://lf.shtwfgs.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zq.yuntaijiaju.cn


<!-- 参考信息 -->