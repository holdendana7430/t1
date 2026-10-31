代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://sm.yuntaijiaju.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bj.szsharing.cn

Java: class Node { int v; Node next; }
来源：http://hg.asd995.cn

Go:   type Node struct { V int; Next *Node }
来源：http://fb.panjiajie.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ds.nicolike.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://fp.yuexingan06.cn

[N11] 二叉树中序遍历
来源：http://gt.muxihuayi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ji.yuntaijiaju.cn

PHP:  // 手写递归函数
来源：http://vz.shxzukj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yq.hahajie.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vu.colortex.cn

Java: // 手写递归
来源：http://wg.521024.cn

Go:   // 手写递归
来源：http://bb.bjjhwx.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zl.lnxyls.cn

C#:   // 手写递归
来源：http://sl.huanxung.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gr.lnxyls.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jj.huanxung.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lp.wgjwhj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ss.yuexingan06.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wo.yuntaijiaju.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fa.hahajie.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ez.hnjuh.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ek.yuexingan06.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xx.wgjwhj.cn

================================================================================
来源：http://ny.shxzskj.cn

O. 并发与异步
来源：http://qx.haigaiapp.cn

================================================================================
来源：http://we.huixiangedu.cn

[O01] 启动一个线程
来源：http://zy.chemitech.net.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hl.hahajie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xh.szxytkj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gt.newstarts.cn

TS:   // 同 JS
来源：http://bd.shtwfgs.cn

Java: new Thread(() -> f()).start()
来源：http://iy.gzmigu.cn

Go:   go f()
来源：http://zh.panjiajie.cn

Ruby: Thread.new { f }
来源：http://up.jianghongdianzi.cn

C#:   Task.Run(() => F());
来源：http://ia.panjiajie.cn

[O02] 使用线程池
来源：http://ee.szsharing.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://uo.bjjhwx.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qt.muxihuayi.cn

JS:   // worker_threads 线程池
来源：http://wy.newstarts.cn

TS:   // worker_threads 线程池
来源：http://wi.bookmarksfly.cn

Java: Executors.newFixedThreadPool(4)
来源：http://os.gzmigu.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ec.yuexingan06.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gi.huixinmuqiang.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gu.huixiangedu.cn

[O03] 加锁保护共享数据
来源：http://nw.muxihuayi.cn

Py:   with lock: shared += 1
来源：http://ks.9csxet.cn

PHP:  // 用 flock() 做文件锁
来源：http://kx.bjjhwx.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dq.hnjuh.cn

TS:   // 同 JS
来源：http://sp.colortex.cn

Java: synchronized (this) { shared++; }
来源：http://rc.jctech888.com.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qr.wgjwhj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://rz.panjiajie.cn

C#:   lock (gate) { shared++; }
来源：http://jg.nicolike.cn

[O04] 定义异步函数并等待
来源：http://nf.nszjky.cn

Py:   async def f():⏎    await g()
来源：http://dp.huixiangedu.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yh.gzmigu.cn

JS:   async function f() { await g(); }
来源：http://um.huixiangedu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://gr.colortex.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jk.wgjwhj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hx.szsharing.cn

Ruby: # 用 Fiber 或 async gem
来源：http://cx.521024.cn

C#:   async Task F() { await G(); }
来源：http://jx.jianghongdianzi.cn

[O05] 并发执行并等待全部完成
来源：http://cb.shtwfgs.cn

Py:   asyncio.gather(*tasks)
来源：http://ab.shxzukj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wc.muxihuayi.cn

JS:   await Promise.all(tasks)
来源：http://bo.shxzukj.cn

TS:   await Promise.all(tasks)
来源：http://ji.chemitech.net.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qm.shtwfgs.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wq.shxzskj.cn

Ruby: threads.map(&:join)
来源：http://fs.haigaiapp.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://de.nicolike.cn

[O06] 使用进程池
来源：http://go.jctech888.com.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://sn.shxzskj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://wt.huanxung.cn

JS:   // child_process / cluster 模块
来源：http://zg.hahajie.cn

TS:   // child_process / cluster 模块
来源：http://cf.521024.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://he.gzmigu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xl.9csxet.cn

Ruby: // fork 块
来源：http://mm.hnjuh.cn

C#:   Parallel.For
来源：http://xv.hahajie.cn

================================================================================
来源：http://dv.szsharing.cn

P. 常用工具函数
来源：http://uq.hnjuh.cn

================================================================================
来源：http://zh.huixinmuqiang.cn

[P01] 生成 UUID
来源：http://kt.jianghongdianzi.cn

Py:   str(uuid.uuid4())
来源：http://st.bookmarksfly.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xh.shtwfgs.cn

JS:   crypto.randomUUID()
来源：http://fl.yuntaijiaju.cn

TS:   crypto.randomUUID()
来源：http://jc.huixiangedu.cn

Java: UUID.randomUUID().toString()
来源：http://fd.bookmarksfly.cn

Go:   // 用 github.com/google/uuid
来源：http://vv.hahajie.cn

Ruby: SecureRandom.uuid
来源：http://bq.chemitech.net.cn

C#:   Guid.NewGuid().ToString()
来源：http://zw.huixiangedu.cn

[P02] MD5 / SHA256 摘要
来源：http://ih.hahajie.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ln.yuntaijiaju.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ou.yuntaijiaju.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bc.shxzskj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://yw.szsharing.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nu.jctech888.com.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fs.jctech888.com.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://yr.asd995.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mi.chemitech.net.cn

[P03] 生成短随机字符串
来源：http://aq.shxzskj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xp.jctech888.com.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lr.haigaiapp.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uf.hahajie.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rj.huanxung.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://sm.szsharing.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qf.jianghongdianzi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ke.szxytkj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://dh.newstarts.cn

[P04] 求长度
来源：http://gu.wgjwhj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nr.muxihuayi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://np.hahajie.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://is.muxihuayi.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pg.521024.cn

Java: list.size();  map.size();  s.length()
来源：http://rt.newstarts.cn

Go:   len(arr);  len(m)
来源：http://bk.huixinmuqiang.cn

Ruby: x.length;  x.size
来源：http://gm.gzmigu.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://it.nszjky.cn

[P05] 判断两个对象内容是否相等
来源：http://ts.hahajie.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://wx.yuexingan06.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://fs.nszjky.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ez.wgjwhj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://py.asd995.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ko.wgjwhj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ot.muxihuayi.cn

Ruby: a == b
来源：http://yd.yuexingan06.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wr.lnxyls.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ot.colortex.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vf.wgjwhj.cn

PHP:  if (empty($x)) {}
来源：http://iy.gzmigu.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://id.hahajie.cn

TS:   if (x == null) {}
来源：http://yf.szxytkj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://rq.szsharing.cn

Go:   if x == nil {}
来源：http://iu.shxzukj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://nr.bookmarksfly.cn

C#:   if (x is null) {}
来源：http://qc.chemitech.net.cn

[P07] 防抖与节流
来源：http://jd.shtwfgs.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.nszjky.cn

PHP:  // 手写时间戳比较
来源：http://lq.jctech888.com.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jn.wgjwhj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ej.nszjky.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pd.shxzukj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://is.wgjwhj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://fo.shtwfgs.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://qt.bookmarksfly.cn

[P08] 处理浮点精度问题
来源：http://re.lnxyls.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ps.nszjky.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://uq.9csxet.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://py.huanxung.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://zn.muxihuayi.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xy.nszjky.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wr.huixinmuqiang.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://za.jctech888.com.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://uo.521024.cn

================================================================================
来源：http://gv.chemitech.net.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wh.yuexingan06.cn

================================================================================
来源：http://bl.jctech888.com.cn

[Q01] 创建表
来源：http://ox.huixinmuqiang.cn

CREATE TABLE users (
来源：http://hm.huixinmuqiang.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tl.newstarts.cn

name VARCHAR(50) NOT NULL,
来源：http://id.shxzukj.cn

email VARCHAR(100) UNIQUE,
来源：http://cr.shxzukj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://gj.huixinmuqiang.cn

);
来源：http://ry.nszjky.cn

[Q02] 创建带外键的表
来源：http://ay.shtwfgs.cn

CREATE TABLE orders (
来源：http://xs.9csxet.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wy.nicolike.cn

user_id INT NOT NULL,
来源：http://lm.yuntaijiaju.cn

amount DECIMAL(10, 2),
来源：http://ej.9csxet.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://uq.lnxyls.cn

);
来源：http://nz.huixinmuqiang.cn

[Q03] 增加列
来源：http://ok.shtwfgs.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ew.jianghongdianzi.cn

[Q04] 修改列类型
来源：http://vs.wgjwhj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://vu.yuexingan06.cn

[Q05] 重命名列
来源：http://qa.muxihuayi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xf.521024.cn

[Q06] 删除列
来源：http://me.lnxyls.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ed.nicolike.cn

[Q07] 删除表
来源：http://xs.chemitech.net.cn

DROP TABLE IF EXISTS orders;
来源：http://zc.nszjky.cn

[Q08] 创建普通索引
来源：http://eg.nszjky.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://mm.szsharing.cn

[Q09] 创建唯一索引
来源：http://uq.gzmigu.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xz.521024.cn

[Q10] 插入单行
来源：http://zj.szxytkj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://yg.lnxyls.cn

[Q11] 一次插入多行
来源：http://ln.shxzskj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wn.bookmarksfly.cn

[Q12] 插入后取自增 ID
来源：http://bv.gzmigu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://dt.chemitech.net.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fw.bookmarksfly.cn

[Q13] 忽略重复插入
来源：http://db.panjiajie.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qu.9csxet.cn

[Q14] 存在则更新（upsert）
来源：http://co.nicolike.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vj.jctech888.com.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://au.szsharing.cn

[Q15] 查询全部
来源：http://mf.shxzukj.cn

SELECT * FROM users;
来源：http://bg.szsharing.cn

[Q16] 查询指定列
来源：http://ly.gzmigu.cn

SELECT id, name FROM users;
来源：http://lv.yuexingan06.cn

[Q17] 条件查询
来源：http://bb.9csxet.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ww.shtwfgs.cn

[Q18] 模糊匹配
来源：http://pf.nszjky.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://oh.haigaiapp.cn

[Q19] 范围查询
来源：http://ev.bjjhwx.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ae.yuexingan06.cn

[Q20] IN 列表
来源：http://ng.9csxet.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qd.huanxung.cn

[Q21] 空值判断
来源：http://zu.gzmigu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://wz.szxytkj.cn

[Q22] 排序
来源：http://wg.colortex.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://nk.bookmarksfly.cn

[Q23] 分页
来源：http://if.haigaiapp.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ne.bjjhwx.cn

[Q24] 去重
来源：http://br.shxzskj.cn

SELECT DISTINCT city FROM users;
来源：http://xa.huixinmuqiang.cn

[Q25] 只取前 N 条
来源：http://vo.panjiajie.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://av.nszjky.cn

[Q26] 计数
来源：http://oq.nszjky.cn

SELECT COUNT(*) FROM users;
来源：http://ff.asd995.cn

[Q27] 条件计数
来源：http://wg.nszjky.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ai.bookmarksfly.cn

[Q28] 求和与平均
来源：http://ox.chemitech.net.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bg.gzmigu.cn

[Q29] 最大最小值
来源：http://jv.gzmigu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://xx.panjiajie.cn

[Q30] 分组统计
来源：http://rp.muxihuayi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vd.shxzskj.cn

[Q31] 分组后过滤
来源：http://cu.shxzskj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mp.nszjky.cn

[Q32] 分组拼接字符串
来源：http://fi.shtwfgs.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vr.huixinmuqiang.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://em.chemitech.net.cn

[Q33] 多列分组
来源：http://rr.colortex.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hv.gzmigu.cn

[Q34] 每组取第一条
来源：http://oz.szxytkj.cn

SELECT * FROM (
来源：http://sj.newstarts.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rd.szsharing.cn

) t WHERE rn = 1;
来源：http://gc.nicolike.cn

[Q35] 内连接
来源：http://kp.bookmarksfly.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ro.haigaiapp.cn

[Q36] 左连接
来源：http://zb.shxzukj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ks.colortex.cn

[Q37] 右连接
来源：http://uw.newstarts.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xm.huixinmuqiang.cn

[Q38] 全外连接（PostgreSQL）
来源：http://gm.chemitech.net.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vp.panjiajie.cn

[Q39] 自连接（查上下级）
来源：http://dw.yuexingan06.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://hw.bjjhwx.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://gu.wgjwhj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://af.szsharing.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wo.chemitech.net.cn

[Q41] 多表连接
来源：http://lo.newstarts.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://cs.jianghongdianzi.cn

JOIN users u ON u.id = o.user_id
来源：http://yd.huixiangedu.cn

JOIN products p ON p.id = o.product_id;
来源：http://zj.asd995.cn

[Q42] 连接条件附加过滤
来源：http://db.nicolike.cn

SELECT u.name, o.amount FROM users u
来源：http://rp.9csxet.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qd.asd995.cn

[Q43] 标量子查询
来源：http://jc.gzmigu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ln.shxzukj.cn

[Q44] IN 子查询
来源：http://vc.haigaiapp.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://af.panjiajie.cn

[Q45] EXISTS 判断存在
来源：http://hn.newstarts.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vw.9csxet.cn

[Q46] NOT EXISTS 判断不存在
来源：http://dc.huixinmuqiang.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rd.wgjwhj.cn

[Q47] 与平均值比较
来源：http://yc.hnjuh.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://pb.szxytkj.cn

[Q48] CTE 公用表表达式
来源：http://lg.chemitech.net.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ng.hnjuh.cn

SELECT * FROM t WHERE c > 5;
来源：http://cb.panjiajie.cn

[Q49] 更新单行
来源：http://ap.jctech888.com.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ak.9csxet.cn

[Q50] 批量更新
来源：http://aj.shtwfgs.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://kp.nszjky.cn

[Q51] 用子查询更新
来源：http://jl.hahajie.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://cl.gzmigu.cn

[Q52] 删除指定行
来源：http://lv.nszjky.cn

DELETE FROM users WHERE id = 10;
来源：http://dw.asd995.cn

[Q53] 按条件删除
来源：http://km.nicolike.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ns.newstarts.cn

[Q54] 清空表
来源：http://gz.bjjhwx.cn

TRUNCATE TABLE logs;
来源：http://qr.newstarts.cn

[Q55] 排名（并列占位）
来源：http://gt.muxihuayi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zi.huixiangedu.cn

[Q56] 密集排名（并列不占位）
来源：http://wv.9csxet.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://uk.szxytkj.cn

[Q57] 行号
来源：http://fx.huanxung.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ej.colortex.cn

[Q58] 累计求和
来源：http://zv.nicolike.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ce.jctech888.com.cn

[Q59] 分组内累计
来源：http://bl.haigaiapp.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://bo.shtwfgs.cn

[Q60] 取上一行 / 下一行
来源：http://pi.jianghongdianzi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xo.jianghongdianzi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://kn.gzmigu.cn


<!-- 参考信息 -->