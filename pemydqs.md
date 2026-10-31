代发 wailian999

PHP:  // 手写递归函数
来源：http://kg.haigaiapp.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sh.yuntaijiaju.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bm.gzmigu.cn

Java: // 手写递归
来源：http://zl.asd995.cn

Go:   // 手写递归
来源：http://hx.bookmarksfly.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://yl.yuntaijiaju.cn

C#:   // 手写递归
来源：http://ta.shxzukj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cl.colortex.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zh.newstarts.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qy.asd995.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kh.haigaiapp.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sy.bookmarksfly.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fo.hnjuh.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://or.shxzukj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xo.wgjwhj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://sn.hahajie.cn

================================================================================
来源：http://iu.huixinmuqiang.cn

O. 并发与异步
来源：http://fr.chemitech.net.cn

================================================================================
来源：http://rx.lnxyls.cn

[O01] 启动一个线程
来源：http://pl.panjiajie.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hx.nszjky.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://cr.yuntaijiaju.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ed.bjjhwx.cn

TS:   // 同 JS
来源：http://cn.9csxet.cn

Java: new Thread(() -> f()).start()
来源：http://wv.hnjuh.cn

Go:   go f()
来源：http://bk.szxytkj.cn

Ruby: Thread.new { f }
来源：http://fk.huanxung.cn

C#:   Task.Run(() => F());
来源：http://ce.panjiajie.cn

[O02] 使用线程池
来源：http://yf.wgjwhj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://si.bookmarksfly.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://sf.lnxyls.cn

JS:   // worker_threads 线程池
来源：http://so.wgjwhj.cn

TS:   // worker_threads 线程池
来源：http://lc.jctech888.com.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ev.muxihuayi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://uu.colortex.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xf.szsharing.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nc.colortex.cn

[O03] 加锁保护共享数据
来源：http://qe.colortex.cn

Py:   with lock: shared += 1
来源：http://sa.hnjuh.cn

PHP:  // 用 flock() 做文件锁
来源：http://rm.panjiajie.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://do.shtwfgs.cn

TS:   // 同 JS
来源：http://fz.szsharing.cn

Java: synchronized (this) { shared++; }
来源：http://js.huixiangedu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wa.521024.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://rh.chemitech.net.cn

C#:   lock (gate) { shared++; }
来源：http://pj.newstarts.cn

[O04] 定义异步函数并等待
来源：http://cf.panjiajie.cn

Py:   async def f():⏎    await g()
来源：http://zz.panjiajie.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jz.hahajie.cn

JS:   async function f() { await g(); }
来源：http://bf.shtwfgs.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ka.bookmarksfly.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wc.hnjuh.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gy.newstarts.cn

Ruby: # 用 Fiber 或 async gem
来源：http://et.huixiangedu.cn

C#:   async Task F() { await G(); }
来源：http://eg.huixiangedu.cn

[O05] 并发执行并等待全部完成
来源：http://ne.bookmarksfly.cn

Py:   asyncio.gather(*tasks)
来源：http://iz.hahajie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cw.hahajie.cn

JS:   await Promise.all(tasks)
来源：http://ph.huixiangedu.cn

TS:   await Promise.all(tasks)
来源：http://fl.gzmigu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://du.chemitech.net.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kp.jianghongdianzi.cn

Ruby: threads.map(&:join)
来源：http://mj.shxzukj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://hr.shxzskj.cn

[O06] 使用进程池
来源：http://qy.szxytkj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qx.yuexingan06.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://uy.szsharing.cn

JS:   // child_process / cluster 模块
来源：http://fn.panjiajie.cn

TS:   // child_process / cluster 模块
来源：http://is.haigaiapp.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rx.nszjky.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lp.panjiajie.cn

Ruby: // fork 块
来源：http://ay.jctech888.com.cn

C#:   Parallel.For
来源：http://pi.huixiangedu.cn

================================================================================
来源：http://ki.huixinmuqiang.cn

P. 常用工具函数
来源：http://gm.9csxet.cn

================================================================================
来源：http://rt.hnjuh.cn

[P01] 生成 UUID
来源：http://rg.szxytkj.cn

Py:   str(uuid.uuid4())
来源：http://nz.panjiajie.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vu.muxihuayi.cn

JS:   crypto.randomUUID()
来源：http://ou.muxihuayi.cn

TS:   crypto.randomUUID()
来源：http://nz.lnxyls.cn

Java: UUID.randomUUID().toString()
来源：http://pq.lnxyls.cn

Go:   // 用 github.com/google/uuid
来源：http://ug.yuntaijiaju.cn

Ruby: SecureRandom.uuid
来源：http://vm.jctech888.com.cn

C#:   Guid.NewGuid().ToString()
来源：http://af.nszjky.cn

[P02] MD5 / SHA256 摘要
来源：http://uv.huanxung.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://eg.gzmigu.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://xo.huixinmuqiang.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bk.shxzukj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://kq.bjjhwx.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ay.yuexingan06.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nv.jctech888.com.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ab.haigaiapp.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fy.bjjhwx.cn

[P03] 生成短随机字符串
来源：http://ha.wgjwhj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://sv.jctech888.com.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://db.muxihuayi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xg.newstarts.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oi.jianghongdianzi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xy.shtwfgs.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xr.colortex.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://xv.shxzukj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zp.nicolike.cn

[P04] 求长度
来源：http://ry.9csxet.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ev.hahajie.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://oe.jianghongdianzi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ea.chemitech.net.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kz.shxzukj.cn

Java: list.size();  map.size();  s.length()
来源：http://lw.szxytkj.cn

Go:   len(arr);  len(m)
来源：http://qe.jctech888.com.cn

Ruby: x.length;  x.size
来源：http://ia.chemitech.net.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://in.gzmigu.cn

[P05] 判断两个对象内容是否相等
来源：http://ez.chemitech.net.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://sw.huanxung.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ur.colortex.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gg.hahajie.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xd.shtwfgs.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://im.bjjhwx.cn

Go:   reflect.DeepEqual(a, b)
来源：http://fh.shxzukj.cn

Ruby: a == b
来源：http://cf.hahajie.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fm.haigaiapp.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ud.shxzskj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gm.bjjhwx.cn

PHP:  if (empty($x)) {}
来源：http://ug.lnxyls.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fq.wgjwhj.cn

TS:   if (x == null) {}
来源：http://nw.szsharing.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://js.shxzskj.cn

Go:   if x == nil {}
来源：http://hf.hnjuh.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://se.jctech888.com.cn

C#:   if (x is null) {}
来源：http://wz.shxzukj.cn

[P07] 防抖与节流
来源：http://tp.panjiajie.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rp.shxzskj.cn

PHP:  // 手写时间戳比较
来源：http://em.shxzukj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zw.shtwfgs.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sa.hnjuh.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://do.nszjky.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rr.521024.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://rz.jianghongdianzi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lc.wgjwhj.cn

[P08] 处理浮点精度问题
来源：http://na.panjiajie.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://pt.chemitech.net.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://tw.jctech888.com.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ou.panjiajie.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ws.jianghongdianzi.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pe.jctech888.com.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://au.yuexingan06.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ql.haigaiapp.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://em.nszjky.cn

================================================================================
来源：http://vf.szsharing.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mv.huanxung.cn

================================================================================
来源：http://va.hnjuh.cn

[Q01] 创建表
来源：http://fu.hnjuh.cn

CREATE TABLE users (
来源：http://rt.nicolike.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hd.huixinmuqiang.cn

name VARCHAR(50) NOT NULL,
来源：http://bs.nszjky.cn

email VARCHAR(100) UNIQUE,
来源：http://hb.lnxyls.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://fx.haigaiapp.cn

);
来源：http://hj.wgjwhj.cn

[Q02] 创建带外键的表
来源：http://jy.nszjky.cn

CREATE TABLE orders (
来源：http://bb.szxytkj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://db.shxzukj.cn

user_id INT NOT NULL,
来源：http://mm.9csxet.cn

amount DECIMAL(10, 2),
来源：http://em.hahajie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://we.szxytkj.cn

);
来源：http://xl.shtwfgs.cn

[Q03] 增加列
来源：http://xr.shxzukj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qa.huanxung.cn

[Q04] 修改列类型
来源：http://ev.lnxyls.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jg.jianghongdianzi.cn

[Q05] 重命名列
来源：http://vw.szsharing.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://tr.huixinmuqiang.cn

[Q06] 删除列
来源：http://li.bookmarksfly.cn

ALTER TABLE users DROP COLUMN age;
来源：http://zr.colortex.cn

[Q07] 删除表
来源：http://jd.hahajie.cn

DROP TABLE IF EXISTS orders;
来源：http://kq.gzmigu.cn

[Q08] 创建普通索引
来源：http://zl.nszjky.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ls.shtwfgs.cn

[Q09] 创建唯一索引
来源：http://wk.shxzukj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ao.huixinmuqiang.cn

[Q10] 插入单行
来源：http://bc.muxihuayi.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hl.chemitech.net.cn

[Q11] 一次插入多行
来源：http://mh.lnxyls.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qb.yuexingan06.cn

[Q12] 插入后取自增 ID
来源：http://rv.gzmigu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://uc.nicolike.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ur.shxzukj.cn

[Q13] 忽略重复插入
来源：http://ma.bookmarksfly.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://tr.muxihuayi.cn

[Q14] 存在则更新（upsert）
来源：http://wl.9csxet.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://um.nszjky.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ke.nszjky.cn

[Q15] 查询全部
来源：http://ed.huanxung.cn

SELECT * FROM users;
来源：http://iu.nicolike.cn

[Q16] 查询指定列
来源：http://ed.521024.cn

SELECT id, name FROM users;
来源：http://pv.shxzukj.cn

[Q17] 条件查询
来源：http://in.szsharing.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ek.yuntaijiaju.cn

[Q18] 模糊匹配
来源：http://xd.huanxung.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hk.panjiajie.cn

[Q19] 范围查询
来源：http://uo.wgjwhj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nm.haigaiapp.cn

[Q20] IN 列表
来源：http://cs.bjjhwx.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ex.bjjhwx.cn

[Q21] 空值判断
来源：http://jb.shxzskj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://aj.nszjky.cn

[Q22] 排序
来源：http://xk.nicolike.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ah.colortex.cn

[Q23] 分页
来源：http://az.shxzukj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gi.lnxyls.cn

[Q24] 去重
来源：http://yq.yuntaijiaju.cn

SELECT DISTINCT city FROM users;
来源：http://gi.huixinmuqiang.cn

[Q25] 只取前 N 条
来源：http://db.colortex.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://be.bjjhwx.cn

[Q26] 计数
来源：http://zj.bjjhwx.cn

SELECT COUNT(*) FROM users;
来源：http://hu.wgjwhj.cn

[Q27] 条件计数
来源：http://wg.muxihuayi.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zf.yuntaijiaju.cn

[Q28] 求和与平均
来源：http://ew.9csxet.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ag.nszjky.cn

[Q29] 最大最小值
来源：http://bk.shxzukj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://rd.huixinmuqiang.cn

[Q30] 分组统计
来源：http://ya.521024.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://in.9csxet.cn

[Q31] 分组后过滤
来源：http://fg.muxihuayi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://py.shtwfgs.cn

[Q32] 分组拼接字符串
来源：http://no.panjiajie.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://sw.shxzskj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://dm.chemitech.net.cn

[Q33] 多列分组
来源：http://zu.huanxung.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ed.haigaiapp.cn

[Q34] 每组取第一条
来源：http://mx.newstarts.cn

SELECT * FROM (
来源：http://eh.jctech888.com.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rb.yuntaijiaju.cn

) t WHERE rn = 1;
来源：http://vh.shxzskj.cn

[Q35] 内连接
来源：http://kr.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ns.szsharing.cn

[Q36] 左连接
来源：http://yo.asd995.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ho.jianghongdianzi.cn

[Q37] 右连接
来源：http://np.jianghongdianzi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://io.szsharing.cn

[Q38] 全外连接（PostgreSQL）
来源：http://kb.bookmarksfly.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ow.huixiangedu.cn

[Q39] 自连接（查上下级）
来源：http://kw.huixinmuqiang.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://qn.huixinmuqiang.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zh.szsharing.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://zz.asd995.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jn.chemitech.net.cn

[Q41] 多表连接
来源：http://dh.jctech888.com.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ih.nszjky.cn

JOIN users u ON u.id = o.user_id
来源：http://en.panjiajie.cn

JOIN products p ON p.id = o.product_id;
来源：http://en.jctech888.com.cn

[Q42] 连接条件附加过滤
来源：http://rp.newstarts.cn

SELECT u.name, o.amount FROM users u
来源：http://pm.newstarts.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fp.colortex.cn

[Q43] 标量子查询
来源：http://yq.shxzukj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kj.asd995.cn

[Q44] IN 子查询
来源：http://zt.newstarts.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://rs.nszjky.cn

[Q45] EXISTS 判断存在
来源：http://ex.shxzskj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ds.hahajie.cn

[Q46] NOT EXISTS 判断不存在
来源：http://fy.nszjky.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gd.shxzukj.cn

[Q47] 与平均值比较
来源：http://mi.9csxet.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://na.nicolike.cn

[Q48] CTE 公用表表达式
来源：http://qk.bjjhwx.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ii.hnjuh.cn

SELECT * FROM t WHERE c > 5;
来源：http://op.jctech888.com.cn

[Q49] 更新单行
来源：http://vd.521024.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ao.szxytkj.cn

[Q50] 批量更新
来源：http://zw.hnjuh.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qn.newstarts.cn

[Q51] 用子查询更新
来源：http://un.hahajie.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zj.nicolike.cn

[Q52] 删除指定行
来源：http://kl.colortex.cn

DELETE FROM users WHERE id = 10;
来源：http://ql.huixiangedu.cn

[Q53] 按条件删除
来源：http://ng.521024.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://kt.hahajie.cn

[Q54] 清空表
来源：http://rs.shxzskj.cn

TRUNCATE TABLE logs;
来源：http://fx.shxzskj.cn

[Q55] 排名（并列占位）
来源：http://fr.yuexingan06.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mv.nicolike.cn

[Q56] 密集排名（并列不占位）
来源：http://ha.yuexingan06.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://pg.hnjuh.cn

[Q57] 行号
来源：http://mu.nicolike.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fz.haigaiapp.cn

[Q58] 累计求和
来源：http://lv.yuntaijiaju.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://kx.shxzskj.cn

[Q59] 分组内累计
来源：http://dq.9csxet.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.521024.cn

[Q60] 取上一行 / 下一行
来源：http://ze.521024.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xq.colortex.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://iz.shtwfgs.cn

[Q61] 移动平均
来源：http://oz.nicolike.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ur.jianghongdianzi.cn

[Q62] 分组占比
来源：http://ck.huixinmuqiang.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://eu.yuntaijiaju.cn

[Q63] 开启事务
来源：http://sb.haigaiapp.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://mu.yuexingan06.cn

[Q64] 提交事务
来源：http://fe.9csxet.cn

COMMIT;
来源：http://yr.shtwfgs.cn


<!-- 参考信息 -->