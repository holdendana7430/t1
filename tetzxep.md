代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://cb.nicolike.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://lu.huanxung.cn

[N11] 二叉树中序遍历
来源：http://dv.wgjwhj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xa.lnxyls.cn

PHP:  // 手写递归函数
来源：http://bt.bookmarksfly.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pc.bjjhwx.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ag.szsharing.cn

Java: // 手写递归
来源：http://ed.nicolike.cn

Go:   // 手写递归
来源：http://le.bookmarksfly.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fh.shtwfgs.cn

C#:   // 手写递归
来源：http://vi.newstarts.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mo.yuntaijiaju.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tx.shxzskj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ls.asd995.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nb.shxzskj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tc.wgjwhj.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ay.szsharing.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://md.wgjwhj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wb.nicolike.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rt.shxzskj.cn

================================================================================
来源：http://uo.9csxet.cn

O. 并发与异步
来源：http://ob.jctech888.com.cn

================================================================================
来源：http://ap.szsharing.cn

[O01] 启动一个线程
来源：http://ju.asd995.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dn.nicolike.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://um.szxytkj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qg.bookmarksfly.cn

TS:   // 同 JS
来源：http://ha.yuntaijiaju.cn

Java: new Thread(() -> f()).start()
来源：http://bg.huanxung.cn

Go:   go f()
来源：http://ac.521024.cn

Ruby: Thread.new { f }
来源：http://op.muxihuayi.cn

C#:   Task.Run(() => F());
来源：http://ih.hnjuh.cn

[O02] 使用线程池
来源：http://qc.newstarts.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.huanxung.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://sy.yuntaijiaju.cn

JS:   // worker_threads 线程池
来源：http://io.muxihuayi.cn

TS:   // worker_threads 线程池
来源：http://hx.521024.cn

Java: Executors.newFixedThreadPool(4)
来源：http://yk.huanxung.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://it.shxzskj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ab.panjiajie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hg.huanxung.cn

[O03] 加锁保护共享数据
来源：http://zo.colortex.cn

Py:   with lock: shared += 1
来源：http://lx.yuntaijiaju.cn

PHP:  // 用 flock() 做文件锁
来源：http://jf.nszjky.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xh.panjiajie.cn

TS:   // 同 JS
来源：http://lb.jctech888.com.cn

Java: synchronized (this) { shared++; }
来源：http://nf.huanxung.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sz.newstarts.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://jw.yuexingan06.cn

C#:   lock (gate) { shared++; }
来源：http://ry.lnxyls.cn

[O04] 定义异步函数并等待
来源：http://zd.yuexingan06.cn

Py:   async def f():⏎    await g()
来源：http://bh.bjjhwx.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lr.colortex.cn

JS:   async function f() { await g(); }
来源：http://cw.jianghongdianzi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://fo.521024.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ro.bookmarksfly.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ee.colortex.cn

Ruby: # 用 Fiber 或 async gem
来源：http://pz.newstarts.cn

C#:   async Task F() { await G(); }
来源：http://ni.huanxung.cn

[O05] 并发执行并等待全部完成
来源：http://lj.huixinmuqiang.cn

Py:   asyncio.gather(*tasks)
来源：http://um.jctech888.com.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dg.shtwfgs.cn

JS:   await Promise.all(tasks)
来源：http://cr.hahajie.cn

TS:   await Promise.all(tasks)
来源：http://nr.panjiajie.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yy.asd995.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ni.hahajie.cn

Ruby: threads.map(&:join)
来源：http://tu.colortex.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://sa.shtwfgs.cn

[O06] 使用进程池
来源：http://uu.haigaiapp.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://dr.lnxyls.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://hf.shxzskj.cn

JS:   // child_process / cluster 模块
来源：http://nx.shxzskj.cn

TS:   // child_process / cluster 模块
来源：http://un.szsharing.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dx.chemitech.net.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lr.asd995.cn

Ruby: // fork 块
来源：http://xb.nszjky.cn

C#:   Parallel.For
来源：http://be.jianghongdianzi.cn

================================================================================
来源：http://vs.shxzukj.cn

P. 常用工具函数
来源：http://lo.haigaiapp.cn

================================================================================
来源：http://rb.huanxung.cn

[P01] 生成 UUID
来源：http://nw.bookmarksfly.cn

Py:   str(uuid.uuid4())
来源：http://jr.shxzukj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://et.shxzskj.cn

JS:   crypto.randomUUID()
来源：http://zr.nicolike.cn

TS:   crypto.randomUUID()
来源：http://ud.bjjhwx.cn

Java: UUID.randomUUID().toString()
来源：http://yk.shxzskj.cn

Go:   // 用 github.com/google/uuid
来源：http://pw.hnjuh.cn

Ruby: SecureRandom.uuid
来源：http://zk.asd995.cn

C#:   Guid.NewGuid().ToString()
来源：http://rk.hnjuh.cn

[P02] MD5 / SHA256 摘要
来源：http://py.nicolike.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ro.asd995.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://qr.nszjky.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xn.lnxyls.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://em.szxytkj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dm.bookmarksfly.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ht.jianghongdianzi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mh.wgjwhj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kg.gzmigu.cn

[P03] 生成短随机字符串
来源：http://nu.yuexingan06.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cn.shtwfgs.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zb.newstarts.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fv.hnjuh.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dl.yuntaijiaju.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yu.colortex.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gr.hahajie.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://nv.521024.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gj.chemitech.net.cn

[P04] 求长度
来源：http://ul.yuntaijiaju.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jj.jctech888.com.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jq.huixiangedu.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nn.wgjwhj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wx.shxzskj.cn

Java: list.size();  map.size();  s.length()
来源：http://lf.9csxet.cn

Go:   len(arr);  len(m)
来源：http://sp.jctech888.com.cn

Ruby: x.length;  x.size
来源：http://zj.hahajie.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://yh.huixiangedu.cn

[P05] 判断两个对象内容是否相等
来源：http://mp.hahajie.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://zj.huixiangedu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ee.shtwfgs.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://dn.haigaiapp.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://kg.jctech888.com.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ah.yuexingan06.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ch.jianghongdianzi.cn

Ruby: a == b
来源：http://lm.nicolike.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qi.huixiangedu.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ya.yuexingan06.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qm.bjjhwx.cn

PHP:  if (empty($x)) {}
来源：http://nc.newstarts.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lr.wgjwhj.cn

TS:   if (x == null) {}
来源：http://ng.shtwfgs.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ka.haigaiapp.cn

Go:   if x == nil {}
来源：http://hi.szsharing.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://of.haigaiapp.cn

C#:   if (x is null) {}
来源：http://xd.yuntaijiaju.cn

[P07] 防抖与节流
来源：http://fn.muxihuayi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://et.muxihuayi.cn

PHP:  // 手写时间戳比较
来源：http://gd.wgjwhj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ns.newstarts.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jz.wgjwhj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://bw.gzmigu.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ym.muxihuayi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://cp.haigaiapp.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ju.chemitech.net.cn

[P08] 处理浮点精度问题
来源：http://ib.huixinmuqiang.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ku.chemitech.net.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jw.shxzskj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://yq.hahajie.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://re.jctech888.com.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ne.nszjky.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://iw.huixinmuqiang.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xo.bookmarksfly.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mr.szsharing.cn

================================================================================
来源：http://lc.nszjky.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rd.nszjky.cn

================================================================================
来源：http://dp.szsharing.cn

[Q01] 创建表
来源：http://zc.asd995.cn

CREATE TABLE users (
来源：http://ub.muxihuayi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dr.shtwfgs.cn

name VARCHAR(50) NOT NULL,
来源：http://ca.hahajie.cn

email VARCHAR(100) UNIQUE,
来源：http://np.shtwfgs.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vb.shxzukj.cn

);
来源：http://mo.yuntaijiaju.cn

[Q02] 创建带外键的表
来源：http://is.yuexingan06.cn

CREATE TABLE orders (
来源：http://nx.bjjhwx.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://sr.asd995.cn

user_id INT NOT NULL,
来源：http://cy.huixiangedu.cn

amount DECIMAL(10, 2),
来源：http://vp.hahajie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://yb.nszjky.cn

);
来源：http://gg.shxzskj.cn

[Q03] 增加列
来源：http://jl.9csxet.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fp.hahajie.cn

[Q04] 修改列类型
来源：http://bn.shxzskj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://nj.wgjwhj.cn

[Q05] 重命名列
来源：http://xl.huixiangedu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://sl.szsharing.cn

[Q06] 删除列
来源：http://er.asd995.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ix.haigaiapp.cn

[Q07] 删除表
来源：http://ul.hnjuh.cn

DROP TABLE IF EXISTS orders;
来源：http://ux.yuntaijiaju.cn

[Q08] 创建普通索引
来源：http://ol.huixiangedu.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://wa.bjjhwx.cn

[Q09] 创建唯一索引
来源：http://zt.yuexingan06.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nd.panjiajie.cn

[Q10] 插入单行
来源：http://kj.muxihuayi.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ei.haigaiapp.cn

[Q11] 一次插入多行
来源：http://kw.huanxung.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gq.nszjky.cn

[Q12] 插入后取自增 ID
来源：http://dx.huixinmuqiang.cn

INSERT INTO users (name) VALUES ('C');
来源：http://pa.nszjky.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vf.szxytkj.cn

[Q13] 忽略重复插入
来源：http://yy.huixinmuqiang.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fn.hnjuh.cn

[Q14] 存在则更新（upsert）
来源：http://it.huanxung.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://au.bookmarksfly.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gl.panjiajie.cn

[Q15] 查询全部
来源：http://jp.yuexingan06.cn

SELECT * FROM users;
来源：http://br.haigaiapp.cn

[Q16] 查询指定列
来源：http://yw.bjjhwx.cn

SELECT id, name FROM users;
来源：http://gb.newstarts.cn

[Q17] 条件查询
来源：http://en.bjjhwx.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://gl.hahajie.cn

[Q18] 模糊匹配
来源：http://ce.lnxyls.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vr.panjiajie.cn

[Q19] 范围查询
来源：http://ze.wgjwhj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bc.huixiangedu.cn

[Q20] IN 列表
来源：http://lc.asd995.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ru.newstarts.cn

[Q21] 空值判断
来源：http://eo.yuexingan06.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://bj.nszjky.cn

[Q22] 排序
来源：http://do.jctech888.com.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qo.newstarts.cn

[Q23] 分页
来源：http://fu.huixiangedu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://oe.bjjhwx.cn

[Q24] 去重
来源：http://xe.jianghongdianzi.cn

SELECT DISTINCT city FROM users;
来源：http://xb.bjjhwx.cn

[Q25] 只取前 N 条
来源：http://qe.yuntaijiaju.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ys.colortex.cn

[Q26] 计数
来源：http://ub.asd995.cn

SELECT COUNT(*) FROM users;
来源：http://ut.jctech888.com.cn

[Q27] 条件计数
来源：http://im.gzmigu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://io.jianghongdianzi.cn

[Q28] 求和与平均
来源：http://vl.colortex.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://pz.bjjhwx.cn

[Q29] 最大最小值
来源：http://sw.szxytkj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://hj.szsharing.cn

[Q30] 分组统计
来源：http://oq.asd995.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cp.nicolike.cn

[Q31] 分组后过滤
来源：http://ls.shxzukj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wg.yuexingan06.cn

[Q32] 分组拼接字符串
来源：http://fq.521024.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://sf.chemitech.net.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://am.huanxung.cn

[Q33] 多列分组
来源：http://su.szsharing.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://eq.newstarts.cn

[Q34] 每组取第一条
来源：http://tj.huixinmuqiang.cn

SELECT * FROM (
来源：http://ss.nszjky.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://og.colortex.cn

) t WHERE rn = 1;
来源：http://df.huixiangedu.cn

[Q35] 内连接
来源：http://cg.huanxung.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://nu.colortex.cn

[Q36] 左连接
来源：http://rz.asd995.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://uj.chemitech.net.cn

[Q37] 右连接
来源：http://ix.bookmarksfly.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ud.yuexingan06.cn

[Q38] 全外连接（PostgreSQL）
来源：http://rp.bjjhwx.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bw.yuexingan06.cn

[Q39] 自连接（查上下级）
来源：http://qk.chemitech.net.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://tm.9csxet.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mf.wgjwhj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://lp.szsharing.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xr.lnxyls.cn

[Q41] 多表连接
来源：http://nq.jianghongdianzi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://tx.bookmarksfly.cn

JOIN users u ON u.id = o.user_id
来源：http://iv.nszjky.cn

JOIN products p ON p.id = o.product_id;
来源：http://rz.nicolike.cn

[Q42] 连接条件附加过滤
来源：http://cw.shxzukj.cn

SELECT u.name, o.amount FROM users u
来源：http://fr.szxytkj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://cu.jianghongdianzi.cn

[Q43] 标量子查询
来源：http://hu.jianghongdianzi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ei.panjiajie.cn

[Q44] IN 子查询
来源：http://zo.huanxung.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nb.muxihuayi.cn

[Q45] EXISTS 判断存在
来源：http://vb.huixinmuqiang.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mb.hnjuh.cn

[Q46] NOT EXISTS 判断不存在
来源：http://wd.haigaiapp.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xg.bookmarksfly.cn

[Q47] 与平均值比较
来源：http://gz.huixinmuqiang.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bk.panjiajie.cn

[Q48] CTE 公用表表达式
来源：http://fa.jianghongdianzi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kt.yuexingan06.cn

SELECT * FROM t WHERE c > 5;
来源：http://tp.9csxet.cn

[Q49] 更新单行
来源：http://ry.nszjky.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://oo.wgjwhj.cn

[Q50] 批量更新
来源：http://hg.shxzskj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tl.newstarts.cn

[Q51] 用子查询更新
来源：http://dv.muxihuayi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ki.chemitech.net.cn

[Q52] 删除指定行
来源：http://tc.szsharing.cn

DELETE FROM users WHERE id = 10;
来源：http://zg.jctech888.com.cn

[Q53] 按条件删除
来源：http://ip.lnxyls.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://pm.yuntaijiaju.cn

[Q54] 清空表
来源：http://gx.bookmarksfly.cn

TRUNCATE TABLE logs;
来源：http://ei.hnjuh.cn

[Q55] 排名（并列占位）
来源：http://ju.bjjhwx.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://bk.haigaiapp.cn

[Q56] 密集排名（并列不占位）
来源：http://bk.shxzukj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ip.yuexingan06.cn

[Q57] 行号
来源：http://md.asd995.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://bj.lnxyls.cn

[Q58] 累计求和
来源：http://df.hnjuh.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mr.huanxung.cn

[Q59] 分组内累计
来源：http://pj.521024.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fc.newstarts.cn

[Q60] 取上一行 / 下一行
来源：http://hp.huanxung.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ti.shxzukj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://nm.521024.cn

[Q61] 移动平均
来源：http://jx.nicolike.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zj.newstarts.cn

[Q62] 分组占比
来源：http://pq.colortex.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ru.wgjwhj.cn


<!-- 参考信息 -->