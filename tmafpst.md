代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://cy.nszjky.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ot.szxytkj.cn

Java: class Node { int v; Node next; }
来源：http://il.wgjwhj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ko.lnxyls.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://hc.huixinmuqiang.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://nn.bookmarksfly.cn

[N11] 二叉树中序遍历
来源：http://ug.shtwfgs.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pe.shxzskj.cn

PHP:  // 手写递归函数
来源：http://ff.chemitech.net.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hf.jctech888.com.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qf.bjjhwx.cn

Java: // 手写递归
来源：http://ov.bookmarksfly.cn

Go:   // 手写递归
来源：http://eh.szsharing.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://si.hahajie.cn

C#:   // 手写递归
来源：http://tm.wgjwhj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bc.panjiajie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vu.chemitech.net.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://sk.huixinmuqiang.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://li.hahajie.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uw.hahajie.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mg.shxzskj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yn.muxihuayi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jy.shxzukj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://nj.nszjky.cn

================================================================================
来源：http://uj.chemitech.net.cn

O. 并发与异步
来源：http://gb.wgjwhj.cn

================================================================================
来源：http://kb.yuntaijiaju.cn

[O01] 启动一个线程
来源：http://rj.wgjwhj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fn.jianghongdianzi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://aw.wgjwhj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://aj.asd995.cn

TS:   // 同 JS
来源：http://df.shxzukj.cn

Java: new Thread(() -> f()).start()
来源：http://ie.huixinmuqiang.cn

Go:   go f()
来源：http://fu.hahajie.cn

Ruby: Thread.new { f }
来源：http://as.asd995.cn

C#:   Task.Run(() => F());
来源：http://je.shxzukj.cn

[O02] 使用线程池
来源：http://ed.yuntaijiaju.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bg.jianghongdianzi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bq.jctech888.com.cn

JS:   // worker_threads 线程池
来源：http://ql.szsharing.cn

TS:   // worker_threads 线程池
来源：http://id.huixinmuqiang.cn

Java: Executors.newFixedThreadPool(4)
来源：http://pf.chemitech.net.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zu.shxzukj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bg.shxzskj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://lk.shtwfgs.cn

[O03] 加锁保护共享数据
来源：http://qc.chemitech.net.cn

Py:   with lock: shared += 1
来源：http://qo.haigaiapp.cn

PHP:  // 用 flock() 做文件锁
来源：http://fu.muxihuayi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mt.yuntaijiaju.cn

TS:   // 同 JS
来源：http://yh.haigaiapp.cn

Java: synchronized (this) { shared++; }
来源：http://ra.szsharing.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dz.jctech888.com.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://gv.hahajie.cn

C#:   lock (gate) { shared++; }
来源：http://vg.bjjhwx.cn

[O04] 定义异步函数并等待
来源：http://fx.shxzukj.cn

Py:   async def f():⏎    await g()
来源：http://vm.nszjky.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wf.szsharing.cn

JS:   async function f() { await g(); }
来源：http://bs.hnjuh.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://pz.gzmigu.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mk.panjiajie.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cv.bookmarksfly.cn

Ruby: # 用 Fiber 或 async gem
来源：http://rq.newstarts.cn

C#:   async Task F() { await G(); }
来源：http://bm.nszjky.cn

[O05] 并发执行并等待全部完成
来源：http://sk.yuntaijiaju.cn

Py:   asyncio.gather(*tasks)
来源：http://lb.bookmarksfly.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gk.jctech888.com.cn

JS:   await Promise.all(tasks)
来源：http://gl.jctech888.com.cn

TS:   await Promise.all(tasks)
来源：http://ev.nszjky.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://we.newstarts.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://pc.szxytkj.cn

Ruby: threads.map(&:join)
来源：http://yy.muxihuayi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://sh.bookmarksfly.cn

[O06] 使用进程池
来源：http://gj.shxzskj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xo.shxzskj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://oa.jianghongdianzi.cn

JS:   // child_process / cluster 模块
来源：http://xq.gzmigu.cn

TS:   // child_process / cluster 模块
来源：http://wf.gzmigu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fv.jctech888.com.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://os.nszjky.cn

Ruby: // fork 块
来源：http://en.huanxung.cn

C#:   Parallel.For
来源：http://ad.huixiangedu.cn

================================================================================
来源：http://re.gzmigu.cn

P. 常用工具函数
来源：http://mn.jctech888.com.cn

================================================================================
来源：http://uo.szxytkj.cn

[P01] 生成 UUID
来源：http://aq.asd995.cn

Py:   str(uuid.uuid4())
来源：http://up.bookmarksfly.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://kc.szsharing.cn

JS:   crypto.randomUUID()
来源：http://nu.521024.cn

TS:   crypto.randomUUID()
来源：http://of.newstarts.cn

Java: UUID.randomUUID().toString()
来源：http://bn.bjjhwx.cn

Go:   // 用 github.com/google/uuid
来源：http://ji.panjiajie.cn

Ruby: SecureRandom.uuid
来源：http://gw.shxzskj.cn

C#:   Guid.NewGuid().ToString()
来源：http://su.asd995.cn

[P02] MD5 / SHA256 摘要
来源：http://bq.bookmarksfly.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rm.jctech888.com.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ar.yuexingan06.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://af.muxihuayi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bq.szsharing.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://yx.shxzukj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://pz.521024.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gu.hnjuh.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://nk.newstarts.cn

[P03] 生成短随机字符串
来源：http://pl.gzmigu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cf.lnxyls.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://sk.chemitech.net.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bk.yuntaijiaju.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vl.9csxet.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://si.hnjuh.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gk.asd995.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://rc.shxzukj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gy.hahajie.cn

[P04] 求长度
来源：http://ml.haigaiapp.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wz.colortex.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://js.shxzukj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ur.muxihuayi.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sb.huanxung.cn

Java: list.size();  map.size();  s.length()
来源：http://ck.nszjky.cn

Go:   len(arr);  len(m)
来源：http://of.yuexingan06.cn

Ruby: x.length;  x.size
来源：http://uo.shxzukj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://hu.gzmigu.cn

[P05] 判断两个对象内容是否相等
来源：http://dg.shxzukj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://mg.yuntaijiaju.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hi.shxzskj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fo.szsharing.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://go.lnxyls.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://sx.shxzskj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://su.hahajie.cn

Ruby: a == b
来源：http://ud.huanxung.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://co.521024.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ia.panjiajie.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://bg.haigaiapp.cn

PHP:  if (empty($x)) {}
来源：http://xa.colortex.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hc.jctech888.com.cn

TS:   if (x == null) {}
来源：http://iu.lnxyls.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://jj.haigaiapp.cn

Go:   if x == nil {}
来源：http://mf.muxihuayi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hx.colortex.cn

C#:   if (x is null) {}
来源：http://wv.jianghongdianzi.cn

[P07] 防抖与节流
来源：http://zr.muxihuayi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ox.huanxung.cn

PHP:  // 手写时间戳比较
来源：http://fj.panjiajie.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qp.lnxyls.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wh.gzmigu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tu.huixiangedu.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://bn.yuntaijiaju.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://pb.hahajie.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ke.haigaiapp.cn

[P08] 处理浮点精度问题
来源：http://gd.nicolike.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://az.huanxung.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vu.9csxet.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://uf.bjjhwx.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://tk.panjiajie.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vq.shxzukj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ks.szsharing.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://eo.yuntaijiaju.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://te.muxihuayi.cn

================================================================================
来源：http://gr.szxytkj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://or.colortex.cn

================================================================================
来源：http://cr.shxzukj.cn

[Q01] 创建表
来源：http://lt.newstarts.cn

CREATE TABLE users (
来源：http://jp.yuntaijiaju.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dg.shxzukj.cn

name VARCHAR(50) NOT NULL,
来源：http://se.bjjhwx.cn

email VARCHAR(100) UNIQUE,
来源：http://rb.hnjuh.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jx.jctech888.com.cn

);
来源：http://xg.haigaiapp.cn

[Q02] 创建带外键的表
来源：http://gb.szxytkj.cn

CREATE TABLE orders (
来源：http://dk.shxzskj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rw.shxzukj.cn

user_id INT NOT NULL,
来源：http://xf.panjiajie.cn

amount DECIMAL(10, 2),
来源：http://nt.colortex.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rn.chemitech.net.cn

);
来源：http://pp.shtwfgs.cn

[Q03] 增加列
来源：http://xm.yuntaijiaju.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wx.newstarts.cn

[Q04] 修改列类型
来源：http://bi.bookmarksfly.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://eu.nicolike.cn

[Q05] 重命名列
来源：http://mm.521024.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://kd.shxzukj.cn

[Q06] 删除列
来源：http://zr.yuntaijiaju.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ze.hahajie.cn

[Q07] 删除表
来源：http://yz.9csxet.cn

DROP TABLE IF EXISTS orders;
来源：http://gu.gzmigu.cn

[Q08] 创建普通索引
来源：http://nc.huanxung.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://zx.bookmarksfly.cn

[Q09] 创建唯一索引
来源：http://nr.muxihuayi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nr.shtwfgs.cn

[Q10] 插入单行
来源：http://sl.shtwfgs.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://oh.521024.cn

[Q11] 一次插入多行
来源：http://dq.huixiangedu.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://eo.521024.cn

[Q12] 插入后取自增 ID
来源：http://pk.haigaiapp.cn

INSERT INTO users (name) VALUES ('C');
来源：http://va.gzmigu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rg.hahajie.cn

[Q13] 忽略重复插入
来源：http://xj.jctech888.com.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ik.szsharing.cn

[Q14] 存在则更新（upsert）
来源：http://nb.colortex.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://yo.huixiangedu.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://tp.nicolike.cn

[Q15] 查询全部
来源：http://jg.gzmigu.cn

SELECT * FROM users;
来源：http://ap.nszjky.cn

[Q16] 查询指定列
来源：http://mw.asd995.cn

SELECT id, name FROM users;
来源：http://xh.huixinmuqiang.cn

[Q17] 条件查询
来源：http://nw.yuntaijiaju.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lu.jianghongdianzi.cn

[Q18] 模糊匹配
来源：http://up.huixinmuqiang.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hu.lnxyls.cn

[Q19] 范围查询
来源：http://ep.gzmigu.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pt.asd995.cn

[Q20] IN 列表
来源：http://mq.szsharing.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://py.jianghongdianzi.cn

[Q21] 空值判断
来源：http://tj.shxzukj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://qj.nicolike.cn

[Q22] 排序
来源：http://ms.gzmigu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://pm.panjiajie.cn

[Q23] 分页
来源：http://ek.szxytkj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://sj.shxzskj.cn

[Q24] 去重
来源：http://hm.jianghongdianzi.cn

SELECT DISTINCT city FROM users;
来源：http://ul.szxytkj.cn

[Q25] 只取前 N 条
来源：http://iq.nszjky.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://pk.shxzukj.cn

[Q26] 计数
来源：http://rr.shxzukj.cn

SELECT COUNT(*) FROM users;
来源：http://pw.nszjky.cn

[Q27] 条件计数
来源：http://ey.shtwfgs.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mw.bjjhwx.cn

[Q28] 求和与平均
来源：http://xl.colortex.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bl.bookmarksfly.cn

[Q29] 最大最小值
来源：http://vr.shxzskj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ib.wgjwhj.cn

[Q30] 分组统计
来源：http://dl.wgjwhj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://yp.lnxyls.cn

[Q31] 分组后过滤
来源：http://zn.shxzukj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://bt.panjiajie.cn

[Q32] 分组拼接字符串
来源：http://fy.hnjuh.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gf.shxzukj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://cr.shtwfgs.cn

[Q33] 多列分组
来源：http://qh.shxzskj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ml.jctech888.com.cn

[Q34] 每组取第一条
来源：http://rp.szsharing.cn

SELECT * FROM (
来源：http://eg.huanxung.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pk.muxihuayi.cn

) t WHERE rn = 1;
来源：http://pj.nszjky.cn

[Q35] 内连接
来源：http://rb.szxytkj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://nq.huanxung.cn

[Q36] 左连接
来源：http://zi.9csxet.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ok.newstarts.cn

[Q37] 右连接
来源：http://po.gzmigu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qr.nicolike.cn

[Q38] 全外连接（PostgreSQL）
来源：http://yr.yuntaijiaju.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hk.szxytkj.cn

[Q39] 自连接（查上下级）
来源：http://vb.bjjhwx.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://nf.bookmarksfly.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://to.hnjuh.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://sp.bjjhwx.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://gu.bookmarksfly.cn

[Q41] 多表连接
来源：http://qq.huixiangedu.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://yl.chemitech.net.cn

JOIN users u ON u.id = o.user_id
来源：http://hv.huixinmuqiang.cn

JOIN products p ON p.id = o.product_id;
来源：http://bn.hahajie.cn

[Q42] 连接条件附加过滤
来源：http://lp.colortex.cn

SELECT u.name, o.amount FROM users u
来源：http://nb.asd995.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://oe.muxihuayi.cn

[Q43] 标量子查询
来源：http://dh.jianghongdianzi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://uu.haigaiapp.cn

[Q44] IN 子查询
来源：http://wp.huixiangedu.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://pc.shxzskj.cn

[Q45] EXISTS 判断存在
来源：http://ga.521024.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pr.hnjuh.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ua.wgjwhj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ur.jctech888.com.cn

[Q47] 与平均值比较
来源：http://un.huixiangedu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ky.szsharing.cn

[Q48] CTE 公用表表达式
来源：http://az.asd995.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://tb.huixinmuqiang.cn

SELECT * FROM t WHERE c > 5;
来源：http://pv.bookmarksfly.cn

[Q49] 更新单行
来源：http://nc.huixinmuqiang.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://th.lnxyls.cn

[Q50] 批量更新
来源：http://sf.shxzukj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zy.haigaiapp.cn

[Q51] 用子查询更新
来源：http://mi.haigaiapp.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://no.shtwfgs.cn

[Q52] 删除指定行
来源：http://se.szxytkj.cn

DELETE FROM users WHERE id = 10;
来源：http://ih.shxzskj.cn

[Q53] 按条件删除
来源：http://dr.jianghongdianzi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://pt.shxzskj.cn

[Q54] 清空表
来源：http://eb.szxytkj.cn

TRUNCATE TABLE logs;
来源：http://lh.yuexingan06.cn

[Q55] 排名（并列占位）
来源：http://md.huixinmuqiang.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gf.jianghongdianzi.cn

[Q56] 密集排名（并列不占位）
来源：http://ym.yuntaijiaju.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zq.muxihuayi.cn

[Q57] 行号
来源：http://bi.nszjky.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zj.hnjuh.cn

[Q58] 累计求和
来源：http://dt.szsharing.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://tp.lnxyls.cn

[Q59] 分组内累计
来源：http://qw.huixinmuqiang.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ic.newstarts.cn

[Q60] 取上一行 / 下一行
来源：http://bq.nszjky.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://yk.jctech888.com.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ei.huixinmuqiang.cn


<!-- 参考信息 -->