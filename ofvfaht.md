代发 wailian999

PHP:  // 手写递归函数
来源：http://wv.yuntaijiaju.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hl.gzmigu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pd.nicolike.cn

Java: // 手写递归
来源：http://yt.newstarts.cn

Go:   // 手写递归
来源：http://qu.lnxyls.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mf.asd995.cn

C#:   // 手写递归
来源：http://tx.panjiajie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lm.muxihuayi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jd.shtwfgs.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cn.bookmarksfly.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kt.nicolike.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yf.panjiajie.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yy.gzmigu.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cx.nicolike.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tu.szxytkj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jk.bjjhwx.cn

================================================================================
来源：http://pv.szxytkj.cn

O. 并发与异步
来源：http://wa.bjjhwx.cn

================================================================================
来源：http://bp.huixinmuqiang.cn

[O01] 启动一个线程
来源：http://fo.huanxung.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gc.gzmigu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lo.yuntaijiaju.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pu.asd995.cn

TS:   // 同 JS
来源：http://ds.shtwfgs.cn

Java: new Thread(() -> f()).start()
来源：http://nz.bjjhwx.cn

Go:   go f()
来源：http://ub.jianghongdianzi.cn

Ruby: Thread.new { f }
来源：http://uo.lnxyls.cn

C#:   Task.Run(() => F());
来源：http://mt.wgjwhj.cn

[O02] 使用线程池
来源：http://pt.bookmarksfly.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://td.gzmigu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qs.yuexingan06.cn

JS:   // worker_threads 线程池
来源：http://jm.muxihuayi.cn

TS:   // worker_threads 线程池
来源：http://ng.colortex.cn

Java: Executors.newFixedThreadPool(4)
来源：http://xm.521024.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ir.jctech888.com.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ck.chemitech.net.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gq.jctech888.com.cn

[O03] 加锁保护共享数据
来源：http://oe.hnjuh.cn

Py:   with lock: shared += 1
来源：http://zu.panjiajie.cn

PHP:  // 用 flock() 做文件锁
来源：http://zk.shxzskj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://so.panjiajie.cn

TS:   // 同 JS
来源：http://qb.gzmigu.cn

Java: synchronized (this) { shared++; }
来源：http://td.bjjhwx.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cr.newstarts.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://oa.shtwfgs.cn

C#:   lock (gate) { shared++; }
来源：http://cj.9csxet.cn

[O04] 定义异步函数并等待
来源：http://fw.newstarts.cn

Py:   async def f():⏎    await g()
来源：http://ks.yuexingan06.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fs.asd995.cn

JS:   async function f() { await g(); }
来源：http://wg.newstarts.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://xa.szsharing.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://va.huixinmuqiang.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hy.colortex.cn

Ruby: # 用 Fiber 或 async gem
来源：http://bi.hahajie.cn

C#:   async Task F() { await G(); }
来源：http://ag.muxihuayi.cn

[O05] 并发执行并等待全部完成
来源：http://yr.hnjuh.cn

Py:   asyncio.gather(*tasks)
来源：http://yz.hahajie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xv.gzmigu.cn

JS:   await Promise.all(tasks)
来源：http://vu.yuntaijiaju.cn

TS:   await Promise.all(tasks)
来源：http://hy.9csxet.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xd.gzmigu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ij.bookmarksfly.cn

Ruby: threads.map(&:join)
来源：http://yd.huanxung.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://st.nicolike.cn

[O06] 使用进程池
来源：http://qt.9csxet.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://sj.shxzskj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://vq.hnjuh.cn

JS:   // child_process / cluster 模块
来源：http://ry.wgjwhj.cn

TS:   // child_process / cluster 模块
来源：http://ea.asd995.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://is.yuntaijiaju.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://nf.yuexingan06.cn

Ruby: // fork 块
来源：http://pm.huixiangedu.cn

C#:   Parallel.For
来源：http://gy.huixiangedu.cn

================================================================================
来源：http://jq.9csxet.cn

P. 常用工具函数
来源：http://ez.wgjwhj.cn

================================================================================
来源：http://au.shtwfgs.cn

[P01] 生成 UUID
来源：http://wb.huixinmuqiang.cn

Py:   str(uuid.uuid4())
来源：http://dm.yuntaijiaju.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ge.szxytkj.cn

JS:   crypto.randomUUID()
来源：http://up.521024.cn

TS:   crypto.randomUUID()
来源：http://pn.shxzskj.cn

Java: UUID.randomUUID().toString()
来源：http://us.bjjhwx.cn

Go:   // 用 github.com/google/uuid
来源：http://of.lnxyls.cn

Ruby: SecureRandom.uuid
来源：http://qw.newstarts.cn

C#:   Guid.NewGuid().ToString()
来源：http://wm.asd995.cn

[P02] MD5 / SHA256 摘要
来源：http://qh.nicolike.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://nq.shxzskj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ie.hnjuh.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://fk.szsharing.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://eb.newstarts.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://cy.nicolike.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://bl.szsharing.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zw.bjjhwx.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://md.jianghongdianzi.cn

[P03] 生成短随机字符串
来源：http://tk.yuntaijiaju.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ho.shtwfgs.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gj.asd995.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wm.lnxyls.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qw.yuexingan06.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://kx.huixinmuqiang.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://fv.hahajie.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://hq.shxzskj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://cx.lnxyls.cn

[P04] 求长度
来源：http://ul.hahajie.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tu.hahajie.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vs.muxihuayi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wb.newstarts.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wt.panjiajie.cn

Java: list.size();  map.size();  s.length()
来源：http://pe.nszjky.cn

Go:   len(arr);  len(m)
来源：http://wi.shxzskj.cn

Ruby: x.length;  x.size
来源：http://ar.panjiajie.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://yl.wgjwhj.cn

[P05] 判断两个对象内容是否相等
来源：http://qt.521024.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://gv.bookmarksfly.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://fx.asd995.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gx.hnjuh.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://pe.jianghongdianzi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ys.jianghongdianzi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://zu.wgjwhj.cn

Ruby: a == b
来源：http://ca.521024.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zb.huanxung.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wd.yuexingan06.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wy.wgjwhj.cn

PHP:  if (empty($x)) {}
来源：http://vz.wgjwhj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ez.shxzskj.cn

TS:   if (x == null) {}
来源：http://uk.bookmarksfly.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://wj.colortex.cn

Go:   if x == nil {}
来源：http://wm.hahajie.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://eo.lnxyls.cn

C#:   if (x is null) {}
来源：http://ib.panjiajie.cn

[P07] 防抖与节流
来源：http://lm.shxzskj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://yw.bjjhwx.cn

PHP:  // 手写时间戳比较
来源：http://nf.wgjwhj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ck.newstarts.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zs.gzmigu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ma.jctech888.com.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://cs.colortex.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://mn.hahajie.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mz.nszjky.cn

[P08] 处理浮点精度问题
来源：http://qd.jctech888.com.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gk.521024.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cu.jctech888.com.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://er.gzmigu.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://eb.szxytkj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kf.asd995.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cm.nicolike.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wr.szxytkj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vv.huixiangedu.cn

================================================================================
来源：http://pm.jianghongdianzi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dx.nicolike.cn

================================================================================
来源：http://dd.lnxyls.cn

[Q01] 创建表
来源：http://on.9csxet.cn

CREATE TABLE users (
来源：http://cc.hahajie.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ut.haigaiapp.cn

name VARCHAR(50) NOT NULL,
来源：http://us.521024.cn

email VARCHAR(100) UNIQUE,
来源：http://iy.bookmarksfly.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vk.szxytkj.cn

);
来源：http://ik.huixiangedu.cn

[Q02] 创建带外键的表
来源：http://dk.shxzskj.cn

CREATE TABLE orders (
来源：http://qc.bookmarksfly.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://zk.muxihuayi.cn

user_id INT NOT NULL,
来源：http://rk.jctech888.com.cn

amount DECIMAL(10, 2),
来源：http://vg.huixiangedu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rk.panjiajie.cn

);
来源：http://xi.shtwfgs.cn

[Q03] 增加列
来源：http://sl.bjjhwx.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://tm.haigaiapp.cn

[Q04] 修改列类型
来源：http://nn.colortex.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hx.shxzskj.cn

[Q05] 重命名列
来源：http://bk.huixiangedu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ju.szsharing.cn

[Q06] 删除列
来源：http://pl.9csxet.cn

ALTER TABLE users DROP COLUMN age;
来源：http://vc.hnjuh.cn

[Q07] 删除表
来源：http://jm.wgjwhj.cn

DROP TABLE IF EXISTS orders;
来源：http://jy.huixinmuqiang.cn

[Q08] 创建普通索引
来源：http://zw.jctech888.com.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://vi.hahajie.cn

[Q09] 创建唯一索引
来源：http://da.shxzskj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zh.colortex.cn

[Q10] 插入单行
来源：http://en.yuexingan06.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fk.bjjhwx.cn

[Q11] 一次插入多行
来源：http://zn.huixiangedu.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://tp.panjiajie.cn

[Q12] 插入后取自增 ID
来源：http://jy.nszjky.cn

INSERT INTO users (name) VALUES ('C');
来源：http://vl.newstarts.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://lx.bookmarksfly.cn

[Q13] 忽略重复插入
来源：http://et.chemitech.net.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pb.newstarts.cn

[Q14] 存在则更新（upsert）
来源：http://bb.jctech888.com.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bc.jianghongdianzi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wa.shxzskj.cn

[Q15] 查询全部
来源：http://ym.huixinmuqiang.cn

SELECT * FROM users;
来源：http://wr.nicolike.cn

[Q16] 查询指定列
来源：http://hb.bjjhwx.cn

SELECT id, name FROM users;
来源：http://la.szxytkj.cn

[Q17] 条件查询
来源：http://tc.colortex.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xn.haigaiapp.cn

[Q18] 模糊匹配
来源：http://to.shtwfgs.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ld.bookmarksfly.cn

[Q19] 范围查询
来源：http://hq.yuntaijiaju.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mt.9csxet.cn

[Q20] IN 列表
来源：http://cs.nicolike.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qv.shxzskj.cn

[Q21] 空值判断
来源：http://om.wgjwhj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://zi.muxihuayi.cn

[Q22] 排序
来源：http://ue.nszjky.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ju.shxzskj.cn

[Q23] 分页
来源：http://an.shxzukj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://el.huixiangedu.cn

[Q24] 去重
来源：http://ya.jianghongdianzi.cn

SELECT DISTINCT city FROM users;
来源：http://ha.521024.cn

[Q25] 只取前 N 条
来源：http://uw.haigaiapp.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://go.hahajie.cn

[Q26] 计数
来源：http://io.nicolike.cn

SELECT COUNT(*) FROM users;
来源：http://kp.gzmigu.cn

[Q27] 条件计数
来源：http://nt.newstarts.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hg.newstarts.cn

[Q28] 求和与平均
来源：http://xa.jctech888.com.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://pp.521024.cn

[Q29] 最大最小值
来源：http://ol.521024.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://rc.shxzukj.cn

[Q30] 分组统计
来源：http://lf.chemitech.net.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://zo.yuntaijiaju.cn

[Q31] 分组后过滤
来源：http://hn.asd995.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gl.muxihuayi.cn

[Q32] 分组拼接字符串
来源：http://gb.yuntaijiaju.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wo.hahajie.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ph.muxihuayi.cn

[Q33] 多列分组
来源：http://ox.jianghongdianzi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://aa.haigaiapp.cn

[Q34] 每组取第一条
来源：http://oh.muxihuayi.cn

SELECT * FROM (
来源：http://yo.hnjuh.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zs.bookmarksfly.cn

) t WHERE rn = 1;
来源：http://fi.hahajie.cn

[Q35] 内连接
来源：http://ms.shtwfgs.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://sx.szsharing.cn

[Q36] 左连接
来源：http://ri.nszjky.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vi.521024.cn

[Q37] 右连接
来源：http://do.szsharing.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://be.shxzskj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://jh.gzmigu.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gr.bjjhwx.cn

[Q39] 自连接（查上下级）
来源：http://ii.hahajie.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://tv.gzmigu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ok.huixiangedu.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://dr.shtwfgs.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ru.chemitech.net.cn

[Q41] 多表连接
来源：http://aq.jctech888.com.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ct.newstarts.cn

JOIN users u ON u.id = o.user_id
来源：http://ay.shxzskj.cn

JOIN products p ON p.id = o.product_id;
来源：http://re.newstarts.cn

[Q42] 连接条件附加过滤
来源：http://nr.shxzskj.cn

SELECT u.name, o.amount FROM users u
来源：http://sh.haigaiapp.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qe.shxzukj.cn

[Q43] 标量子查询
来源：http://jq.szxytkj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gt.haigaiapp.cn

[Q44] IN 子查询
来源：http://ri.9csxet.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wo.huixinmuqiang.cn

[Q45] EXISTS 判断存在
来源：http://ni.huanxung.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fd.haigaiapp.cn

[Q46] NOT EXISTS 判断不存在
来源：http://jz.huanxung.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qj.nicolike.cn

[Q47] 与平均值比较
来源：http://oh.hahajie.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dy.yuexingan06.cn

[Q48] CTE 公用表表达式
来源：http://fo.gzmigu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dq.muxihuayi.cn

SELECT * FROM t WHERE c > 5;
来源：http://if.newstarts.cn

[Q49] 更新单行
来源：http://md.huixinmuqiang.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vf.jianghongdianzi.cn

[Q50] 批量更新
来源：http://xx.nszjky.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ce.huanxung.cn

[Q51] 用子查询更新
来源：http://ml.9csxet.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mk.521024.cn

[Q52] 删除指定行
来源：http://ol.bookmarksfly.cn

DELETE FROM users WHERE id = 10;
来源：http://fd.lnxyls.cn

[Q53] 按条件删除
来源：http://iy.huixiangedu.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://os.huanxung.cn

[Q54] 清空表
来源：http://ky.shtwfgs.cn

TRUNCATE TABLE logs;
来源：http://pu.huixiangedu.cn

[Q55] 排名（并列占位）
来源：http://bd.szsharing.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gs.521024.cn

[Q56] 密集排名（并列不占位）
来源：http://td.szxytkj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yn.hahajie.cn

[Q57] 行号
来源：http://el.szxytkj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://kf.wgjwhj.cn

[Q58] 累计求和
来源：http://jp.newstarts.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nk.newstarts.cn

[Q59] 分组内累计
来源：http://qr.gzmigu.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://za.shxzskj.cn

[Q60] 取上一行 / 下一行
来源：http://du.szxytkj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bc.nicolike.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://db.yuntaijiaju.cn

[Q61] 移动平均
来源：http://ua.newstarts.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ap.newstarts.cn

[Q62] 分组占比
来源：http://yn.shxzskj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ng.hnjuh.cn

[Q63] 开启事务
来源：http://oo.521024.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://kl.lnxyls.cn

[Q64] 提交事务
来源：http://sl.newstarts.cn

COMMIT;
来源：http://ec.huixinmuqiang.cn


<!-- 参考信息 -->