代发 wailian999

Go:   // 手写递归
来源：http://yn.huixiangedu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://oi.newstarts.cn

C#:   // 手写递归
来源：http://jh.jianghongdianzi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cg.shxzukj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ab.panjiajie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://sf.wgjwhj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vi.chemitech.net.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uz.jctech888.com.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hr.521024.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://er.panjiajie.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rt.newstarts.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://of.wgjwhj.cn

================================================================================
来源：http://qy.szxytkj.cn

O. 并发与异步
来源：http://yo.yuntaijiaju.cn

================================================================================
来源：http://sn.muxihuayi.cn

[O01] 启动一个线程
来源：http://xd.yuexingan06.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://eg.jctech888.com.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jv.hnjuh.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cz.jctech888.com.cn

TS:   // 同 JS
来源：http://xx.jianghongdianzi.cn

Java: new Thread(() -> f()).start()
来源：http://nz.szxytkj.cn

Go:   go f()
来源：http://st.nicolike.cn

Ruby: Thread.new { f }
来源：http://ij.colortex.cn

C#:   Task.Run(() => F());
来源：http://id.bjjhwx.cn

[O02] 使用线程池
来源：http://be.lnxyls.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qo.lnxyls.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zq.huixinmuqiang.cn

JS:   // worker_threads 线程池
来源：http://sn.yuntaijiaju.cn

TS:   // worker_threads 线程池
来源：http://sz.bjjhwx.cn

Java: Executors.newFixedThreadPool(4)
来源：http://qd.shxzskj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wz.yuntaijiaju.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lx.nszjky.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vz.yuntaijiaju.cn

[O03] 加锁保护共享数据
来源：http://qd.jctech888.com.cn

Py:   with lock: shared += 1
来源：http://gm.muxihuayi.cn

PHP:  // 用 flock() 做文件锁
来源：http://xc.wgjwhj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://no.huixiangedu.cn

TS:   // 同 JS
来源：http://ba.newstarts.cn

Java: synchronized (this) { shared++; }
来源：http://az.chemitech.net.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://uz.jctech888.com.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://yu.chemitech.net.cn

C#:   lock (gate) { shared++; }
来源：http://rq.huixinmuqiang.cn

[O04] 定义异步函数并等待
来源：http://vw.yuexingan06.cn

Py:   async def f():⏎    await g()
来源：http://ym.huanxung.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://th.asd995.cn

JS:   async function f() { await g(); }
来源：http://vp.lnxyls.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ne.shxzukj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qx.shxzskj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://sg.huanxung.cn

Ruby: # 用 Fiber 或 async gem
来源：http://uu.wgjwhj.cn

C#:   async Task F() { await G(); }
来源：http://pn.bookmarksfly.cn

[O05] 并发执行并等待全部完成
来源：http://dw.lnxyls.cn

Py:   asyncio.gather(*tasks)
来源：http://np.panjiajie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://sf.bjjhwx.cn

JS:   await Promise.all(tasks)
来源：http://hm.jianghongdianzi.cn

TS:   await Promise.all(tasks)
来源：http://gr.shxzskj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://lj.shxzskj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bx.newstarts.cn

Ruby: threads.map(&:join)
来源：http://kt.bjjhwx.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://go.haigaiapp.cn

[O06] 使用进程池
来源：http://uf.newstarts.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://po.nszjky.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://zo.yuexingan06.cn

JS:   // child_process / cluster 模块
来源：http://rv.9csxet.cn

TS:   // child_process / cluster 模块
来源：http://ry.huixiangedu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tb.huixinmuqiang.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cc.asd995.cn

Ruby: // fork 块
来源：http://cn.muxihuayi.cn

C#:   Parallel.For
来源：http://dj.huanxung.cn

================================================================================
来源：http://sa.wgjwhj.cn

P. 常用工具函数
来源：http://gx.chemitech.net.cn

================================================================================
来源：http://un.huixinmuqiang.cn

[P01] 生成 UUID
来源：http://lc.jctech888.com.cn

Py:   str(uuid.uuid4())
来源：http://yh.muxihuayi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pe.bookmarksfly.cn

JS:   crypto.randomUUID()
来源：http://jz.asd995.cn

TS:   crypto.randomUUID()
来源：http://dv.bjjhwx.cn

Java: UUID.randomUUID().toString()
来源：http://ig.yuexingan06.cn

Go:   // 用 github.com/google/uuid
来源：http://az.szxytkj.cn

Ruby: SecureRandom.uuid
来源：http://fn.lnxyls.cn

C#:   Guid.NewGuid().ToString()
来源：http://tc.colortex.cn

[P02] MD5 / SHA256 摘要
来源：http://vc.szxytkj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qt.lnxyls.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ro.lnxyls.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gp.shxzskj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dm.asd995.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vu.yuntaijiaju.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://we.chemitech.net.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://pv.hahajie.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://px.521024.cn

[P03] 生成短随机字符串
来源：http://tz.huanxung.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cg.colortex.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rk.jianghongdianzi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oz.chemitech.net.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ir.521024.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://dh.wgjwhj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nh.huixinmuqiang.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://vk.lnxyls.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wz.haigaiapp.cn

[P04] 求长度
来源：http://mh.hahajie.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ay.asd995.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wb.nszjky.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ad.nicolike.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gp.haigaiapp.cn

Java: list.size();  map.size();  s.length()
来源：http://xw.nicolike.cn

Go:   len(arr);  len(m)
来源：http://et.haigaiapp.cn

Ruby: x.length;  x.size
来源：http://ig.yuexingan06.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://hg.panjiajie.cn

[P05] 判断两个对象内容是否相等
来源：http://kq.jianghongdianzi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://qe.newstarts.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gq.jctech888.com.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ft.lnxyls.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ch.jianghongdianzi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://gb.hahajie.cn

Go:   reflect.DeepEqual(a, b)
来源：http://vj.jianghongdianzi.cn

Ruby: a == b
来源：http://pj.bookmarksfly.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ni.yuntaijiaju.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gk.szxytkj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pd.nszjky.cn

PHP:  if (empty($x)) {}
来源：http://yr.bjjhwx.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://sf.muxihuayi.cn

TS:   if (x == null) {}
来源：http://vv.asd995.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://qm.muxihuayi.cn

Go:   if x == nil {}
来源：http://eh.shtwfgs.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zi.muxihuayi.cn

C#:   if (x is null) {}
来源：http://tg.yuexingan06.cn

[P07] 防抖与节流
来源：http://ev.lnxyls.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xa.gzmigu.cn

PHP:  // 手写时间戳比较
来源：http://yo.haigaiapp.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ub.haigaiapp.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://re.nszjky.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fk.shxzukj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://tj.yuntaijiaju.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://dz.nszjky.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gn.chemitech.net.cn

[P08] 处理浮点精度问题
来源：http://fi.521024.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ge.bookmarksfly.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lj.panjiajie.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://kr.chemitech.net.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://bt.huanxung.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://et.bookmarksfly.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ze.newstarts.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fs.gzmigu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zm.szxytkj.cn

================================================================================
来源：http://od.colortex.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://de.newstarts.cn

================================================================================
来源：http://mz.huixiangedu.cn

[Q01] 创建表
来源：http://ug.huixiangedu.cn

CREATE TABLE users (
来源：http://dd.bookmarksfly.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bn.haigaiapp.cn

name VARCHAR(50) NOT NULL,
来源：http://rp.shxzukj.cn

email VARCHAR(100) UNIQUE,
来源：http://hd.hnjuh.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vp.jianghongdianzi.cn

);
来源：http://gg.shxzskj.cn

[Q02] 创建带外键的表
来源：http://be.huixinmuqiang.cn

CREATE TABLE orders (
来源：http://rp.jctech888.com.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://li.nicolike.cn

user_id INT NOT NULL,
来源：http://hl.lnxyls.cn

amount DECIMAL(10, 2),
来源：http://yg.hahajie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ci.newstarts.cn

);
来源：http://qu.521024.cn

[Q03] 增加列
来源：http://hj.yuexingan06.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qp.szxytkj.cn

[Q04] 修改列类型
来源：http://ut.huanxung.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gl.jctech888.com.cn

[Q05] 重命名列
来源：http://mw.szxytkj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fu.colortex.cn

[Q06] 删除列
来源：http://vf.szsharing.cn

ALTER TABLE users DROP COLUMN age;
来源：http://zx.hnjuh.cn

[Q07] 删除表
来源：http://gm.colortex.cn

DROP TABLE IF EXISTS orders;
来源：http://fi.wgjwhj.cn

[Q08] 创建普通索引
来源：http://qu.huanxung.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ku.asd995.cn

[Q09] 创建唯一索引
来源：http://ft.yuntaijiaju.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://eg.9csxet.cn

[Q10] 插入单行
来源：http://at.chemitech.net.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gw.gzmigu.cn

[Q11] 一次插入多行
来源：http://ro.jianghongdianzi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://bf.huixinmuqiang.cn

[Q12] 插入后取自增 ID
来源：http://fs.nicolike.cn

INSERT INTO users (name) VALUES ('C');
来源：http://jz.szxytkj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://xf.jctech888.com.cn

[Q13] 忽略重复插入
来源：http://pk.bjjhwx.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://nq.521024.cn

[Q14] 存在则更新（upsert）
来源：http://mw.szxytkj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ef.9csxet.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ca.chemitech.net.cn

[Q15] 查询全部
来源：http://ij.shxzskj.cn

SELECT * FROM users;
来源：http://hx.huixinmuqiang.cn

[Q16] 查询指定列
来源：http://rg.szsharing.cn

SELECT id, name FROM users;
来源：http://ja.asd995.cn

[Q17] 条件查询
来源：http://gv.hnjuh.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://bm.huanxung.cn

[Q18] 模糊匹配
来源：http://xw.yuexingan06.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qc.jianghongdianzi.cn

[Q19] 范围查询
来源：http://gc.jctech888.com.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://co.bjjhwx.cn

[Q20] IN 列表
来源：http://rl.yuntaijiaju.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://se.jctech888.com.cn

[Q21] 空值判断
来源：http://tv.asd995.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://dh.nszjky.cn

[Q22] 排序
来源：http://dc.jianghongdianzi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ab.hnjuh.cn

[Q23] 分页
来源：http://hh.yuntaijiaju.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tc.nicolike.cn

[Q24] 去重
来源：http://ad.shxzukj.cn

SELECT DISTINCT city FROM users;
来源：http://ix.521024.cn

[Q25] 只取前 N 条
来源：http://ks.yuntaijiaju.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zf.jianghongdianzi.cn

[Q26] 计数
来源：http://wo.huixiangedu.cn

SELECT COUNT(*) FROM users;
来源：http://lk.jianghongdianzi.cn

[Q27] 条件计数
来源：http://um.panjiajie.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://te.bookmarksfly.cn

[Q28] 求和与平均
来源：http://ty.9csxet.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://qo.521024.cn

[Q29] 最大最小值
来源：http://fb.521024.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://xe.bookmarksfly.cn

[Q30] 分组统计
来源：http://ap.521024.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hj.haigaiapp.cn

[Q31] 分组后过滤
来源：http://yp.newstarts.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://sr.521024.cn

[Q32] 分组拼接字符串
来源：http://wq.bjjhwx.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jv.jianghongdianzi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://il.huanxung.cn

[Q33] 多列分组
来源：http://ay.newstarts.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xq.yuexingan06.cn

[Q34] 每组取第一条
来源：http://mr.nicolike.cn

SELECT * FROM (
来源：http://xj.haigaiapp.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://kt.huixiangedu.cn

) t WHERE rn = 1;
来源：http://vp.shxzskj.cn

[Q35] 内连接
来源：http://ih.huixiangedu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ql.newstarts.cn

[Q36] 左连接
来源：http://ho.colortex.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hv.huanxung.cn

[Q37] 右连接
来源：http://ts.jianghongdianzi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ax.szxytkj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ne.lnxyls.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://db.haigaiapp.cn

[Q39] 自连接（查上下级）
来源：http://tw.nszjky.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://au.szsharing.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zm.huixinmuqiang.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://wb.hahajie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xy.nicolike.cn

[Q41] 多表连接
来源：http://db.hnjuh.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://gz.hnjuh.cn

JOIN users u ON u.id = o.user_id
来源：http://xw.huanxung.cn

JOIN products p ON p.id = o.product_id;
来源：http://ip.szxytkj.cn

[Q42] 连接条件附加过滤
来源：http://zf.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u
来源：http://cr.szsharing.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hb.haigaiapp.cn

[Q43] 标量子查询
来源：http://jk.colortex.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ny.huanxung.cn

[Q44] IN 子查询
来源：http://sn.jctech888.com.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://yu.szsharing.cn

[Q45] EXISTS 判断存在
来源：http://un.wgjwhj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://km.jianghongdianzi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://kc.yuexingan06.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qf.huixiangedu.cn

[Q47] 与平均值比较
来源：http://py.asd995.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://is.jctech888.com.cn

[Q48] CTE 公用表表达式
来源：http://fo.shtwfgs.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://af.9csxet.cn

SELECT * FROM t WHERE c > 5;
来源：http://ze.shtwfgs.cn

[Q49] 更新单行
来源：http://cs.jctech888.com.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://uv.nszjky.cn

[Q50] 批量更新
来源：http://nn.gzmigu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zq.huixinmuqiang.cn

[Q51] 用子查询更新
来源：http://fg.newstarts.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rd.bjjhwx.cn

[Q52] 删除指定行
来源：http://vg.colortex.cn

DELETE FROM users WHERE id = 10;
来源：http://qm.gzmigu.cn

[Q53] 按条件删除
来源：http://km.shxzukj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zi.panjiajie.cn

[Q54] 清空表
来源：http://ch.huixiangedu.cn

TRUNCATE TABLE logs;
来源：http://ng.huanxung.cn

[Q55] 排名（并列占位）
来源：http://jf.hnjuh.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://nd.9csxet.cn

[Q56] 密集排名（并列不占位）
来源：http://li.gzmigu.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fo.nicolike.cn

[Q57] 行号
来源：http://td.panjiajie.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tt.hahajie.cn

[Q58] 累计求和
来源：http://uy.szxytkj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://yt.hnjuh.cn

[Q59] 分组内累计
来源：http://fr.lnxyls.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://dl.nszjky.cn

[Q60] 取上一行 / 下一行
来源：http://he.9csxet.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jw.colortex.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xp.jianghongdianzi.cn

[Q61] 移动平均
来源：http://ff.bookmarksfly.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://df.521024.cn

[Q62] 分组占比
来源：http://lc.jianghongdianzi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://bt.haigaiapp.cn

[Q63] 开启事务
来源：http://vt.huixinmuqiang.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://cr.hnjuh.cn

[Q64] 提交事务
来源：http://kh.lnxyls.cn

COMMIT;
来源：http://ov.szxytkj.cn

[Q65] 回滚事务
来源：http://yr.shxzukj.cn

ROLLBACK;
来源：http://ts.shxzukj.cn

[Q66] 行锁查询
来源：http://pk.jianghongdianzi.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bd.yuntaijiaju.cn


<!-- 参考信息 -->