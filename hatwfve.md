代发 wailian999

PHP:  // 手写递归函数
来源：http://jr.bookmarksfly.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://co.muxihuayi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jw.hnjuh.cn

Java: // 手写递归
来源：http://nf.yuntaijiaju.cn

Go:   // 手写递归
来源：http://lo.shtwfgs.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://in.colortex.cn

C#:   // 手写递归
来源：http://uj.9csxet.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://at.szsharing.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qr.nicolike.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ea.9csxet.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vg.huixinmuqiang.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://le.521024.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ns.muxihuayi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bq.9csxet.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hn.newstarts.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://cm.szsharing.cn

================================================================================
来源：http://bf.9csxet.cn

O. 并发与异步
来源：http://og.bjjhwx.cn

================================================================================
来源：http://ac.nicolike.cn

[O01] 启动一个线程
来源：http://ue.huixinmuqiang.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nz.lnxyls.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://af.nszjky.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://br.shxzskj.cn

TS:   // 同 JS
来源：http://qa.jianghongdianzi.cn

Java: new Thread(() -> f()).start()
来源：http://xg.nszjky.cn

Go:   go f()
来源：http://vu.wgjwhj.cn

Ruby: Thread.new { f }
来源：http://fm.panjiajie.cn

C#:   Task.Run(() => F());
来源：http://zd.yuexingan06.cn

[O02] 使用线程池
来源：http://em.hnjuh.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rk.lnxyls.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jt.bjjhwx.cn

JS:   // worker_threads 线程池
来源：http://vy.bjjhwx.cn

TS:   // worker_threads 线程池
来源：http://or.muxihuayi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://yj.newstarts.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://uq.nszjky.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jk.asd995.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wu.haigaiapp.cn

[O03] 加锁保护共享数据
来源：http://oc.chemitech.net.cn

Py:   with lock: shared += 1
来源：http://rf.bjjhwx.cn

PHP:  // 用 flock() 做文件锁
来源：http://pp.hnjuh.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ny.nicolike.cn

TS:   // 同 JS
来源：http://ew.shxzskj.cn

Java: synchronized (this) { shared++; }
来源：http://yl.shxzukj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://uw.haigaiapp.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://hc.521024.cn

C#:   lock (gate) { shared++; }
来源：http://tv.szxytkj.cn

[O04] 定义异步函数并等待
来源：http://kj.nszjky.cn

Py:   async def f():⏎    await g()
来源：http://au.wgjwhj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ev.colortex.cn

JS:   async function f() { await g(); }
来源：http://zl.gzmigu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ip.hahajie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zs.nicolike.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pl.jctech888.com.cn

Ruby: # 用 Fiber 或 async gem
来源：http://sg.gzmigu.cn

C#:   async Task F() { await G(); }
来源：http://nk.shtwfgs.cn

[O05] 并发执行并等待全部完成
来源：http://ss.haigaiapp.cn

Py:   asyncio.gather(*tasks)
来源：http://vi.muxihuayi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kv.yuexingan06.cn

JS:   await Promise.all(tasks)
来源：http://zr.lnxyls.cn

TS:   await Promise.all(tasks)
来源：http://ez.jctech888.com.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://eb.shtwfgs.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://pc.gzmigu.cn

Ruby: threads.map(&:join)
来源：http://un.9csxet.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://eb.lnxyls.cn

[O06] 使用进程池
来源：http://eo.jianghongdianzi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ti.yuexingan06.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ib.shxzskj.cn

JS:   // child_process / cluster 模块
来源：http://tz.muxihuayi.cn

TS:   // child_process / cluster 模块
来源：http://ra.gzmigu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vi.chemitech.net.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://at.szsharing.cn

Ruby: // fork 块
来源：http://yt.yuntaijiaju.cn

C#:   Parallel.For
来源：http://et.wgjwhj.cn

================================================================================
来源：http://qe.yuexingan06.cn

P. 常用工具函数
来源：http://cg.hnjuh.cn

================================================================================
来源：http://ly.521024.cn

[P01] 生成 UUID
来源：http://qq.bookmarksfly.cn

Py:   str(uuid.uuid4())
来源：http://lt.jianghongdianzi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gj.chemitech.net.cn

JS:   crypto.randomUUID()
来源：http://vn.szsharing.cn

TS:   crypto.randomUUID()
来源：http://tw.asd995.cn

Java: UUID.randomUUID().toString()
来源：http://dh.bjjhwx.cn

Go:   // 用 github.com/google/uuid
来源：http://ue.lnxyls.cn

Ruby: SecureRandom.uuid
来源：http://gn.hnjuh.cn

C#:   Guid.NewGuid().ToString()
来源：http://zx.huixiangedu.cn

[P02] MD5 / SHA256 摘要
来源：http://uo.szsharing.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ps.9csxet.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://gz.huixiangedu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://na.hahajie.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gi.shxzukj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://sn.huixiangedu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mv.yuntaijiaju.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bq.szxytkj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://cm.panjiajie.cn

[P03] 生成短随机字符串
来源：http://nn.huixinmuqiang.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://eg.bookmarksfly.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lf.jctech888.com.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sb.huixiangedu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ao.521024.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jw.jctech888.com.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pm.gzmigu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://fr.shtwfgs.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://tb.9csxet.cn

[P04] 求长度
来源：http://ky.newstarts.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jy.asd995.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qa.521024.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kj.huanxung.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tq.shxzukj.cn

Java: list.size();  map.size();  s.length()
来源：http://kp.bjjhwx.cn

Go:   len(arr);  len(m)
来源：http://fo.chemitech.net.cn

Ruby: x.length;  x.size
来源：http://mq.szxytkj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://we.panjiajie.cn

[P05] 判断两个对象内容是否相等
来源：http://aw.hnjuh.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://zp.lnxyls.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://df.huixinmuqiang.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ij.szxytkj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://yc.521024.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ey.colortex.cn

Go:   reflect.DeepEqual(a, b)
来源：http://rg.9csxet.cn

Ruby: a == b
来源：http://gm.huixiangedu.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://td.wgjwhj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://cu.shtwfgs.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://uy.yuexingan06.cn

PHP:  if (empty($x)) {}
来源：http://kj.nszjky.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://tk.hahajie.cn

TS:   if (x == null) {}
来源：http://xq.521024.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://uu.bookmarksfly.cn

Go:   if x == nil {}
来源：http://ob.yuexingan06.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ek.lnxyls.cn

C#:   if (x is null) {}
来源：http://nu.bookmarksfly.cn

[P07] 防抖与节流
来源：http://rv.shtwfgs.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://dc.muxihuayi.cn

PHP:  // 手写时间戳比较
来源：http://lx.hnjuh.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sy.gzmigu.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://za.jctech888.com.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://em.nszjky.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rs.wgjwhj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://dd.muxihuayi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://tc.wgjwhj.cn

[P08] 处理浮点精度问题
来源：http://ha.wgjwhj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://er.nszjky.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://va.huixiangedu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gw.asd995.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://gy.asd995.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ju.bookmarksfly.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gu.nicolike.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hb.wgjwhj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ft.yuntaijiaju.cn

================================================================================
来源：http://qt.wgjwhj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://va.chemitech.net.cn

================================================================================
来源：http://wx.haigaiapp.cn

[Q01] 创建表
来源：http://ki.9csxet.cn

CREATE TABLE users (
来源：http://tm.jctech888.com.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ur.huixiangedu.cn

name VARCHAR(50) NOT NULL,
来源：http://md.yuexingan06.cn

email VARCHAR(100) UNIQUE,
来源：http://hy.panjiajie.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://je.bookmarksfly.cn

);
来源：http://so.colortex.cn

[Q02] 创建带外键的表
来源：http://hl.yuexingan06.cn

CREATE TABLE orders (
来源：http://xx.bookmarksfly.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ry.chemitech.net.cn

user_id INT NOT NULL,
来源：http://vr.lnxyls.cn

amount DECIMAL(10, 2),
来源：http://yk.huixiangedu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://os.bookmarksfly.cn

);
来源：http://tj.szxytkj.cn

[Q03] 增加列
来源：http://da.szsharing.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ww.yuntaijiaju.cn

[Q04] 修改列类型
来源：http://ro.jctech888.com.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hi.hnjuh.cn

[Q05] 重命名列
来源：http://qt.hahajie.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ru.szsharing.cn

[Q06] 删除列
来源：http://no.nicolike.cn

ALTER TABLE users DROP COLUMN age;
来源：http://hb.huixiangedu.cn

[Q07] 删除表
来源：http://zl.9csxet.cn

DROP TABLE IF EXISTS orders;
来源：http://xk.9csxet.cn

[Q08] 创建普通索引
来源：http://aw.muxihuayi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://lg.hahajie.cn

[Q09] 创建唯一索引
来源：http://yu.jctech888.com.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zp.bookmarksfly.cn

[Q10] 插入单行
来源：http://ys.chemitech.net.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jy.nszjky.cn

[Q11] 一次插入多行
来源：http://gv.szsharing.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://be.hahajie.cn

[Q12] 插入后取自增 ID
来源：http://zf.newstarts.cn

INSERT INTO users (name) VALUES ('C');
来源：http://gc.nszjky.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ls.wgjwhj.cn

[Q13] 忽略重复插入
来源：http://ks.hahajie.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://yq.jianghongdianzi.cn

[Q14] 存在则更新（upsert）
来源：http://gn.nszjky.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ue.yuexingan06.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mh.bjjhwx.cn

[Q15] 查询全部
来源：http://ha.asd995.cn

SELECT * FROM users;
来源：http://vh.newstarts.cn

[Q16] 查询指定列
来源：http://wm.521024.cn

SELECT id, name FROM users;
来源：http://me.nszjky.cn

[Q17] 条件查询
来源：http://zq.jianghongdianzi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qh.9csxet.cn

[Q18] 模糊匹配
来源：http://qz.szsharing.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ge.colortex.cn

[Q19] 范围查询
来源：http://jm.jianghongdianzi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://yd.wgjwhj.cn

[Q20] IN 列表
来源：http://vm.nicolike.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://iz.asd995.cn

[Q21] 空值判断
来源：http://vb.bjjhwx.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://zr.wgjwhj.cn

[Q22] 排序
来源：http://pd.chemitech.net.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://sk.lnxyls.cn

[Q23] 分页
来源：http://hk.9csxet.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rj.huanxung.cn

[Q24] 去重
来源：http://gg.chemitech.net.cn

SELECT DISTINCT city FROM users;
来源：http://eb.jctech888.com.cn

[Q25] 只取前 N 条
来源：http://ow.wgjwhj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vv.hnjuh.cn

[Q26] 计数
来源：http://zo.9csxet.cn

SELECT COUNT(*) FROM users;
来源：http://or.newstarts.cn

[Q27] 条件计数
来源：http://nf.hnjuh.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ct.bjjhwx.cn

[Q28] 求和与平均
来源：http://uq.shxzukj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rk.muxihuayi.cn

[Q29] 最大最小值
来源：http://kk.hahajie.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://cf.muxihuayi.cn

[Q30] 分组统计
来源：http://yr.huanxung.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ew.jianghongdianzi.cn

[Q31] 分组后过滤
来源：http://gz.szsharing.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nz.bookmarksfly.cn

[Q32] 分组拼接字符串
来源：http://le.nicolike.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ia.asd995.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://nl.panjiajie.cn

[Q33] 多列分组
来源：http://nq.szxytkj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xy.asd995.cn

[Q34] 每组取第一条
来源：http://lr.chemitech.net.cn

SELECT * FROM (
来源：http://qq.panjiajie.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://og.muxihuayi.cn

) t WHERE rn = 1;
来源：http://fm.panjiajie.cn

[Q35] 内连接
来源：http://zz.colortex.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ja.shxzukj.cn

[Q36] 左连接
来源：http://zr.huanxung.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mq.haigaiapp.cn

[Q37] 右连接
来源：http://rr.muxihuayi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fp.yuexingan06.cn

[Q38] 全外连接（PostgreSQL）
来源：http://kf.gzmigu.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ti.asd995.cn

[Q39] 自连接（查上下级）
来源：http://wg.wgjwhj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://za.lnxyls.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nv.hnjuh.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://uz.haigaiapp.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qu.hahajie.cn

[Q41] 多表连接
来源：http://xx.nszjky.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://kg.yuexingan06.cn

JOIN users u ON u.id = o.user_id
来源：http://ii.bookmarksfly.cn

JOIN products p ON p.id = o.product_id;
来源：http://dw.panjiajie.cn

[Q42] 连接条件附加过滤
来源：http://ba.shtwfgs.cn

SELECT u.name, o.amount FROM users u
来源：http://su.hnjuh.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://lg.huanxung.cn

[Q43] 标量子查询
来源：http://op.wgjwhj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fh.yuexingan06.cn

[Q44] IN 子查询
来源：http://ne.asd995.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://aa.shxzskj.cn

[Q45] EXISTS 判断存在
来源：http://hc.nicolike.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ho.nicolike.cn

[Q46] NOT EXISTS 判断不存在
来源：http://hk.asd995.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yn.panjiajie.cn

[Q47] 与平均值比较
来源：http://zy.yuexingan06.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://iy.shxzukj.cn

[Q48] CTE 公用表表达式
来源：http://yk.521024.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ll.9csxet.cn

SELECT * FROM t WHERE c > 5;
来源：http://sm.huixiangedu.cn

[Q49] 更新单行
来源：http://ud.haigaiapp.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ls.shtwfgs.cn

[Q50] 批量更新
来源：http://fb.9csxet.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://nb.wgjwhj.cn

[Q51] 用子查询更新
来源：http://gv.asd995.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://gw.newstarts.cn

[Q52] 删除指定行
来源：http://sm.haigaiapp.cn

DELETE FROM users WHERE id = 10;
来源：http://ah.bjjhwx.cn

[Q53] 按条件删除
来源：http://zq.muxihuayi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://pc.yuntaijiaju.cn

[Q54] 清空表
来源：http://gl.hahajie.cn

TRUNCATE TABLE logs;
来源：http://tq.jianghongdianzi.cn

[Q55] 排名（并列占位）
来源：http://ln.panjiajie.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ks.newstarts.cn

[Q56] 密集排名（并列不占位）
来源：http://et.huixinmuqiang.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ih.wgjwhj.cn

[Q57] 行号
来源：http://nz.colortex.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ie.huixinmuqiang.cn

[Q58] 累计求和
来源：http://ea.bookmarksfly.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://kg.hahajie.cn

[Q59] 分组内累计
来源：http://bu.haigaiapp.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vw.jianghongdianzi.cn

[Q60] 取上一行 / 下一行
来源：http://rr.nszjky.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rf.bookmarksfly.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ky.yuntaijiaju.cn

[Q61] 移动平均
来源：http://fe.wgjwhj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://kp.colortex.cn

[Q62] 分组占比
来源：http://qo.yuexingan06.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xm.shxzskj.cn

[Q63] 开启事务
来源：http://lu.hahajie.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://sa.bookmarksfly.cn

[Q64] 提交事务
来源：http://zc.haigaiapp.cn

COMMIT;
来源：http://fp.gzmigu.cn


<!-- 参考信息 -->