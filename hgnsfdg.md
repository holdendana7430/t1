代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://xx.asd995.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://sc.shtwfgs.cn

[N11] 二叉树中序遍历
来源：http://ve.hahajie.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vc.huixiangedu.cn

PHP:  // 手写递归函数
来源：http://rt.colortex.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://td.521024.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kh.nicolike.cn

Java: // 手写递归
来源：http://dj.gzmigu.cn

Go:   // 手写递归
来源：http://hz.huixinmuqiang.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lh.wgjwhj.cn

C#:   // 手写递归
来源：http://sa.9csxet.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mi.newstarts.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://im.yuntaijiaju.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ed.huixiangedu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rk.haigaiapp.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pu.gzmigu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tj.jianghongdianzi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bh.nszjky.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://en.shxzukj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://se.nicolike.cn

================================================================================
来源：http://bg.hnjuh.cn

O. 并发与异步
来源：http://kl.muxihuayi.cn

================================================================================
来源：http://vn.yuexingan06.cn

[O01] 启动一个线程
来源：http://tt.bookmarksfly.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nu.nicolike.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yj.huanxung.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cm.gzmigu.cn

TS:   // 同 JS
来源：http://xt.huixinmuqiang.cn

Java: new Thread(() -> f()).start()
来源：http://mx.jianghongdianzi.cn

Go:   go f()
来源：http://wi.szsharing.cn

Ruby: Thread.new { f }
来源：http://ic.huanxung.cn

C#:   Task.Run(() => F());
来源：http://pp.huixiangedu.cn

[O02] 使用线程池
来源：http://wu.9csxet.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xw.hahajie.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zg.521024.cn

JS:   // worker_threads 线程池
来源：http://ru.panjiajie.cn

TS:   // worker_threads 线程池
来源：http://bl.yuntaijiaju.cn

Java: Executors.newFixedThreadPool(4)
来源：http://vb.nszjky.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ec.shtwfgs.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://en.bjjhwx.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bb.9csxet.cn

[O03] 加锁保护共享数据
来源：http://va.9csxet.cn

Py:   with lock: shared += 1
来源：http://ne.lnxyls.cn

PHP:  // 用 flock() 做文件锁
来源：http://zc.shtwfgs.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qx.huixinmuqiang.cn

TS:   // 同 JS
来源：http://du.lnxyls.cn

Java: synchronized (this) { shared++; }
来源：http://fm.shxzukj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://os.szsharing.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://qf.shtwfgs.cn

C#:   lock (gate) { shared++; }
来源：http://lg.muxihuayi.cn

[O04] 定义异步函数并等待
来源：http://sg.newstarts.cn

Py:   async def f():⏎    await g()
来源：http://qw.jianghongdianzi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rz.nszjky.cn

JS:   async function f() { await g(); }
来源：http://ga.bjjhwx.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://xo.huixiangedu.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://eo.huanxung.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://iu.shtwfgs.cn

Ruby: # 用 Fiber 或 async gem
来源：http://zo.muxihuayi.cn

C#:   async Task F() { await G(); }
来源：http://ta.hahajie.cn

[O05] 并发执行并等待全部完成
来源：http://xk.chemitech.net.cn

Py:   asyncio.gather(*tasks)
来源：http://lf.nicolike.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wu.asd995.cn

JS:   await Promise.all(tasks)
来源：http://me.nicolike.cn

TS:   await Promise.all(tasks)
来源：http://bk.shxzskj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xm.jctech888.com.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://uc.nicolike.cn

Ruby: threads.map(&:join)
来源：http://sg.huanxung.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://id.bjjhwx.cn

[O06] 使用进程池
来源：http://ro.asd995.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zo.hnjuh.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://xq.bjjhwx.cn

JS:   // child_process / cluster 模块
来源：http://cx.hahajie.cn

TS:   // child_process / cluster 模块
来源：http://sd.szxytkj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ey.shxzskj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://en.nicolike.cn

Ruby: // fork 块
来源：http://wv.colortex.cn

C#:   Parallel.For
来源：http://jv.shxzukj.cn

================================================================================
来源：http://rl.jctech888.com.cn

P. 常用工具函数
来源：http://xo.muxihuayi.cn

================================================================================
来源：http://gk.yuntaijiaju.cn

[P01] 生成 UUID
来源：http://yl.huixinmuqiang.cn

Py:   str(uuid.uuid4())
来源：http://nu.haigaiapp.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ly.yuexingan06.cn

JS:   crypto.randomUUID()
来源：http://bt.wgjwhj.cn

TS:   crypto.randomUUID()
来源：http://lb.shtwfgs.cn

Java: UUID.randomUUID().toString()
来源：http://ju.shxzskj.cn

Go:   // 用 github.com/google/uuid
来源：http://id.muxihuayi.cn

Ruby: SecureRandom.uuid
来源：http://xa.shtwfgs.cn

C#:   Guid.NewGuid().ToString()
来源：http://qw.asd995.cn

[P02] MD5 / SHA256 摘要
来源：http://jd.chemitech.net.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ql.wgjwhj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://gg.521024.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wf.wgjwhj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gn.9csxet.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://cd.hnjuh.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qo.chemitech.net.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://up.muxihuayi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://oq.yuexingan06.cn

[P03] 生成短随机字符串
来源：http://xa.bjjhwx.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://bl.asd995.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://sr.huixinmuqiang.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://go.hahajie.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pm.shxzskj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ut.nszjky.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://iy.muxihuayi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://qy.bjjhwx.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qm.chemitech.net.cn

[P04] 求长度
来源：http://at.colortex.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ni.gzmigu.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://am.shxzskj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zu.jctech888.com.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yr.huanxung.cn

Java: list.size();  map.size();  s.length()
来源：http://sc.jianghongdianzi.cn

Go:   len(arr);  len(m)
来源：http://gb.huanxung.cn

Ruby: x.length;  x.size
来源：http://yt.muxihuayi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://oc.hnjuh.cn

[P05] 判断两个对象内容是否相等
来源：http://qq.bookmarksfly.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ft.colortex.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ku.gzmigu.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://oo.szxytkj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://sx.huanxung.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://br.huanxung.cn

Go:   reflect.DeepEqual(a, b)
来源：http://tr.huixiangedu.cn

Ruby: a == b
来源：http://ar.nszjky.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dh.newstarts.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://yb.chemitech.net.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://nk.wgjwhj.cn

PHP:  if (empty($x)) {}
来源：http://bt.asd995.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lc.shtwfgs.cn

TS:   if (x == null) {}
来源：http://gt.shxzukj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://aq.gzmigu.cn

Go:   if x == nil {}
来源：http://si.nicolike.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qv.shtwfgs.cn

C#:   if (x is null) {}
来源：http://tp.newstarts.cn

[P07] 防抖与节流
来源：http://gk.haigaiapp.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wx.szsharing.cn

PHP:  // 手写时间戳比较
来源：http://xn.9csxet.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eh.haigaiapp.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fo.jctech888.com.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fd.szxytkj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://oh.shxzukj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://zq.9csxet.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ul.szsharing.cn

[P08] 处理浮点精度问题
来源：http://sr.gzmigu.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://oz.shxzskj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cp.9csxet.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://cy.muxihuayi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://rr.bookmarksfly.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ig.hnjuh.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://lr.nszjky.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://al.newstarts.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wo.bjjhwx.cn

================================================================================
来源：http://er.yuntaijiaju.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ya.521024.cn

================================================================================
来源：http://hq.521024.cn

[Q01] 创建表
来源：http://zq.panjiajie.cn

CREATE TABLE users (
来源：http://px.bookmarksfly.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tm.asd995.cn

name VARCHAR(50) NOT NULL,
来源：http://bw.wgjwhj.cn

email VARCHAR(100) UNIQUE,
来源：http://at.haigaiapp.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bg.muxihuayi.cn

);
来源：http://gq.shtwfgs.cn

[Q02] 创建带外键的表
来源：http://sc.muxihuayi.cn

CREATE TABLE orders (
来源：http://qk.haigaiapp.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://uw.shtwfgs.cn

user_id INT NOT NULL,
来源：http://vh.lnxyls.cn

amount DECIMAL(10, 2),
来源：http://pa.yuexingan06.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ml.9csxet.cn

);
来源：http://il.haigaiapp.cn

[Q03] 增加列
来源：http://se.szsharing.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://se.szxytkj.cn

[Q04] 修改列类型
来源：http://qu.nszjky.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cu.wgjwhj.cn

[Q05] 重命名列
来源：http://bf.shxzskj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://tk.521024.cn

[Q06] 删除列
来源：http://vv.huanxung.cn

ALTER TABLE users DROP COLUMN age;
来源：http://dq.shxzskj.cn

[Q07] 删除表
来源：http://sq.newstarts.cn

DROP TABLE IF EXISTS orders;
来源：http://xk.wgjwhj.cn

[Q08] 创建普通索引
来源：http://zk.yuntaijiaju.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://sh.jctech888.com.cn

[Q09] 创建唯一索引
来源：http://kq.nicolike.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ua.nszjky.cn

[Q10] 插入单行
来源：http://kb.haigaiapp.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://lj.shxzukj.cn

[Q11] 一次插入多行
来源：http://pp.chemitech.net.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xt.szxytkj.cn

[Q12] 插入后取自增 ID
来源：http://eh.shxzukj.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ux.shxzukj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dy.nicolike.cn

[Q13] 忽略重复插入
来源：http://yf.newstarts.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kb.szsharing.cn

[Q14] 存在则更新（upsert）
来源：http://hx.colortex.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vp.huanxung.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://tp.chemitech.net.cn

[Q15] 查询全部
来源：http://ym.szxytkj.cn

SELECT * FROM users;
来源：http://vm.nszjky.cn

[Q16] 查询指定列
来源：http://hy.9csxet.cn

SELECT id, name FROM users;
来源：http://nb.hahajie.cn

[Q17] 条件查询
来源：http://nv.yuntaijiaju.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hh.gzmigu.cn

[Q18] 模糊匹配
来源：http://lm.huixinmuqiang.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ab.bookmarksfly.cn

[Q19] 范围查询
来源：http://nj.jctech888.com.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://tg.nszjky.cn

[Q20] IN 列表
来源：http://no.shtwfgs.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pz.yuexingan06.cn

[Q21] 空值判断
来源：http://ds.huixiangedu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://gh.shxzukj.cn

[Q22] 排序
来源：http://nl.huanxung.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://rj.jianghongdianzi.cn

[Q23] 分页
来源：http://qz.hnjuh.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://up.521024.cn

[Q24] 去重
来源：http://kf.521024.cn

SELECT DISTINCT city FROM users;
来源：http://fx.521024.cn

[Q25] 只取前 N 条
来源：http://jc.shxzukj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://nk.yuntaijiaju.cn

[Q26] 计数
来源：http://pc.szsharing.cn

SELECT COUNT(*) FROM users;
来源：http://er.shxzskj.cn

[Q27] 条件计数
来源：http://xo.gzmigu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ic.shxzukj.cn

[Q28] 求和与平均
来源：http://dd.9csxet.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://nb.huixiangedu.cn

[Q29] 最大最小值
来源：http://ut.haigaiapp.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://pc.colortex.cn

[Q30] 分组统计
来源：http://al.hahajie.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ln.bookmarksfly.cn

[Q31] 分组后过滤
来源：http://ma.jianghongdianzi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://uy.huixiangedu.cn

[Q32] 分组拼接字符串
来源：http://vb.hahajie.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://em.muxihuayi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lo.panjiajie.cn

[Q33] 多列分组
来源：http://hf.521024.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mg.newstarts.cn

[Q34] 每组取第一条
来源：http://mv.shxzskj.cn

SELECT * FROM (
来源：http://pd.szsharing.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://dm.hnjuh.cn

) t WHERE rn = 1;
来源：http://eh.colortex.cn

[Q35] 内连接
来源：http://ml.panjiajie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ft.newstarts.cn

[Q36] 左连接
来源：http://cy.9csxet.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wz.huixinmuqiang.cn

[Q37] 右连接
来源：http://eq.huanxung.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ms.bjjhwx.cn

[Q38] 全外连接（PostgreSQL）
来源：http://lp.szsharing.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gv.9csxet.cn

[Q39] 自连接（查上下级）
来源：http://ax.jctech888.com.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://bv.lnxyls.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ft.jctech888.com.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://iq.521024.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hv.gzmigu.cn

[Q41] 多表连接
来源：http://wm.bjjhwx.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://cr.shtwfgs.cn

JOIN users u ON u.id = o.user_id
来源：http://rf.muxihuayi.cn

JOIN products p ON p.id = o.product_id;
来源：http://ip.chemitech.net.cn

[Q42] 连接条件附加过滤
来源：http://dm.jianghongdianzi.cn

SELECT u.name, o.amount FROM users u
来源：http://nu.hahajie.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ai.bookmarksfly.cn

[Q43] 标量子查询
来源：http://im.huixiangedu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://oy.jianghongdianzi.cn

[Q44] IN 子查询
来源：http://wv.bjjhwx.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ss.chemitech.net.cn

[Q45] EXISTS 判断存在
来源：http://wh.asd995.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mh.jianghongdianzi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://oo.shtwfgs.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nv.muxihuayi.cn

[Q47] 与平均值比较
来源：http://cx.muxihuayi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://oq.shxzskj.cn

[Q48] CTE 公用表表达式
来源：http://zm.huanxung.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hu.hahajie.cn

SELECT * FROM t WHERE c > 5;
来源：http://se.jctech888.com.cn

[Q49] 更新单行
来源：http://zt.hnjuh.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jo.szxytkj.cn

[Q50] 批量更新
来源：http://jb.jianghongdianzi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://cz.hahajie.cn

[Q51] 用子查询更新
来源：http://xg.muxihuayi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lv.jianghongdianzi.cn

[Q52] 删除指定行
来源：http://kh.nicolike.cn

DELETE FROM users WHERE id = 10;
来源：http://yy.yuexingan06.cn

[Q53] 按条件删除
来源：http://fy.bjjhwx.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://kt.muxihuayi.cn

[Q54] 清空表
来源：http://vo.hnjuh.cn

TRUNCATE TABLE logs;
来源：http://ue.chemitech.net.cn

[Q55] 排名（并列占位）
来源：http://nq.9csxet.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qk.shxzskj.cn

[Q56] 密集排名（并列不占位）
来源：http://kp.nicolike.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rd.jianghongdianzi.cn

[Q57] 行号
来源：http://rp.yuntaijiaju.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ez.9csxet.cn

[Q58] 累计求和
来源：http://oo.jianghongdianzi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dj.521024.cn

[Q59] 分组内累计
来源：http://at.yuexingan06.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fx.huixinmuqiang.cn

[Q60] 取上一行 / 下一行
来源：http://rr.yuntaijiaju.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://tr.nicolike.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dw.newstarts.cn

[Q61] 移动平均
来源：http://ba.yuntaijiaju.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://uz.haigaiapp.cn

[Q62] 分组占比
来源：http://nm.gzmigu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qw.bjjhwx.cn


<!-- 参考信息 -->