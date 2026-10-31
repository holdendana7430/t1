代发 wailian999

PHP:  // 手写递归函数
来源：http://jo.hahajie.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fd.huixiangedu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xj.nicolike.cn

Java: // 手写递归
来源：http://gj.hnjuh.cn

Go:   // 手写递归
来源：http://cj.huixinmuqiang.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ko.nszjky.cn

C#:   // 手写递归
来源：http://mu.asd995.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.asd995.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://yt.lnxyls.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hc.521024.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bc.lnxyls.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://eq.jianghongdianzi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://pt.szsharing.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rr.huixiangedu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qh.521024.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://nw.szsharing.cn

================================================================================
来源：http://ua.521024.cn

O. 并发与异步
来源：http://sp.haigaiapp.cn

================================================================================
来源：http://xp.hnjuh.cn

[O01] 启动一个线程
来源：http://lo.hahajie.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ab.wgjwhj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ho.szsharing.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://lk.gzmigu.cn

TS:   // 同 JS
来源：http://nt.jctech888.com.cn

Java: new Thread(() -> f()).start()
来源：http://cj.szsharing.cn

Go:   go f()
来源：http://ra.huixinmuqiang.cn

Ruby: Thread.new { f }
来源：http://yy.chemitech.net.cn

C#:   Task.Run(() => F());
来源：http://qi.shtwfgs.cn

[O02] 使用线程池
来源：http://uv.bookmarksfly.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kn.jctech888.com.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ns.jctech888.com.cn

JS:   // worker_threads 线程池
来源：http://se.szsharing.cn

TS:   // worker_threads 线程池
来源：http://rq.gzmigu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ms.szsharing.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qd.gzmigu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xg.asd995.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ls.jctech888.com.cn

[O03] 加锁保护共享数据
来源：http://oh.shxzukj.cn

Py:   with lock: shared += 1
来源：http://xp.muxihuayi.cn

PHP:  // 用 flock() 做文件锁
来源：http://lm.shxzskj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pa.huanxung.cn

TS:   // 同 JS
来源：http://ix.haigaiapp.cn

Java: synchronized (this) { shared++; }
来源：http://rg.wgjwhj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pw.shxzukj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://kp.shtwfgs.cn

C#:   lock (gate) { shared++; }
来源：http://po.panjiajie.cn

[O04] 定义异步函数并等待
来源：http://hl.yuntaijiaju.cn

Py:   async def f():⏎    await g()
来源：http://me.szsharing.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tj.nicolike.cn

JS:   async function f() { await g(); }
来源：http://ba.shxzukj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://fw.chemitech.net.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kq.newstarts.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://io.hnjuh.cn

Ruby: # 用 Fiber 或 async gem
来源：http://zi.asd995.cn

C#:   async Task F() { await G(); }
来源：http://qb.nszjky.cn

[O05] 并发执行并等待全部完成
来源：http://jp.hnjuh.cn

Py:   asyncio.gather(*tasks)
来源：http://vt.huanxung.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zi.colortex.cn

JS:   await Promise.all(tasks)
来源：http://hj.nszjky.cn

TS:   await Promise.all(tasks)
来源：http://vb.haigaiapp.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://lw.wgjwhj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://te.szxytkj.cn

Ruby: threads.map(&:join)
来源：http://kd.newstarts.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://zt.szsharing.cn

[O06] 使用进程池
来源：http://dv.jctech888.com.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://cv.huixinmuqiang.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://lh.huanxung.cn

JS:   // child_process / cluster 模块
来源：http://gq.jctech888.com.cn

TS:   // child_process / cluster 模块
来源：http://fn.shxzskj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zr.9csxet.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://he.bjjhwx.cn

Ruby: // fork 块
来源：http://fq.haigaiapp.cn

C#:   Parallel.For
来源：http://gl.haigaiapp.cn

================================================================================
来源：http://wt.nicolike.cn

P. 常用工具函数
来源：http://uo.haigaiapp.cn

================================================================================
来源：http://iq.colortex.cn

[P01] 生成 UUID
来源：http://bz.gzmigu.cn

Py:   str(uuid.uuid4())
来源：http://ay.newstarts.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qj.muxihuayi.cn

JS:   crypto.randomUUID()
来源：http://zk.huanxung.cn

TS:   crypto.randomUUID()
来源：http://pu.shxzukj.cn

Java: UUID.randomUUID().toString()
来源：http://yx.bjjhwx.cn

Go:   // 用 github.com/google/uuid
来源：http://we.shxzukj.cn

Ruby: SecureRandom.uuid
来源：http://np.szsharing.cn

C#:   Guid.NewGuid().ToString()
来源：http://hf.hnjuh.cn

[P02] MD5 / SHA256 摘要
来源：http://at.huanxung.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rj.szsharing.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://jw.chemitech.net.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wb.haigaiapp.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://le.nszjky.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vu.huixiangedu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://yj.shtwfgs.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ha.bookmarksfly.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zo.panjiajie.cn

[P03] 生成短随机字符串
来源：http://rj.muxihuayi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rp.muxihuayi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://io.bjjhwx.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ix.hnjuh.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cn.colortex.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pq.colortex.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pd.521024.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://wb.huixiangedu.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://bf.haigaiapp.cn

[P04] 求长度
来源：http://yr.gzmigu.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qu.nszjky.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fn.muxihuayi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hj.bjjhwx.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hm.gzmigu.cn

Java: list.size();  map.size();  s.length()
来源：http://ob.jianghongdianzi.cn

Go:   len(arr);  len(m)
来源：http://pd.szxytkj.cn

Ruby: x.length;  x.size
来源：http://wb.nicolike.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ne.9csxet.cn

[P05] 判断两个对象内容是否相等
来源：http://pu.szxytkj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://oi.nicolike.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://zj.hahajie.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://pi.shxzskj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mz.521024.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rs.bjjhwx.cn

Go:   reflect.DeepEqual(a, b)
来源：http://kw.yuexingan06.cn

Ruby: a == b
来源：http://dm.haigaiapp.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dc.lnxyls.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ol.muxihuayi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jc.hnjuh.cn

PHP:  if (empty($x)) {}
来源：http://yz.bookmarksfly.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jh.hahajie.cn

TS:   if (x == null) {}
来源：http://sj.hnjuh.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://yj.nicolike.cn

Go:   if x == nil {}
来源：http://ar.bookmarksfly.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mz.chemitech.net.cn

C#:   if (x is null) {}
来源：http://aq.haigaiapp.cn

[P07] 防抖与节流
来源：http://nn.panjiajie.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wm.shtwfgs.cn

PHP:  // 手写时间戳比较
来源：http://nm.521024.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ci.asd995.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gf.9csxet.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://to.gzmigu.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jg.jctech888.com.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://li.huanxung.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jd.colortex.cn

[P08] 处理浮点精度问题
来源：http://la.shxzskj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://nh.newstarts.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://pf.jianghongdianzi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://tw.panjiajie.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vj.hnjuh.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hy.lnxyls.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gf.shxzskj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ub.bjjhwx.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://nf.shtwfgs.cn

================================================================================
来源：http://af.jianghongdianzi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://or.huixinmuqiang.cn

================================================================================
来源：http://tq.hnjuh.cn

[Q01] 创建表
来源：http://yw.huixinmuqiang.cn

CREATE TABLE users (
来源：http://jw.hnjuh.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bu.newstarts.cn

name VARCHAR(50) NOT NULL,
来源：http://vb.shxzukj.cn

email VARCHAR(100) UNIQUE,
来源：http://xw.shxzukj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wh.chemitech.net.cn

);
来源：http://ht.chemitech.net.cn

[Q02] 创建带外键的表
来源：http://lu.shxzskj.cn

CREATE TABLE orders (
来源：http://sx.shtwfgs.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kb.wgjwhj.cn

user_id INT NOT NULL,
来源：http://ft.huixiangedu.cn

amount DECIMAL(10, 2),
来源：http://zr.szxytkj.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://kb.huixiangedu.cn

);
来源：http://sm.huixinmuqiang.cn

[Q03] 增加列
来源：http://kv.hnjuh.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fd.szsharing.cn

[Q04] 修改列类型
来源：http://kk.szsharing.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qg.jianghongdianzi.cn

[Q05] 重命名列
来源：http://oa.bookmarksfly.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ye.newstarts.cn

[Q06] 删除列
来源：http://ff.jianghongdianzi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://sw.huixiangedu.cn

[Q07] 删除表
来源：http://iw.panjiajie.cn

DROP TABLE IF EXISTS orders;
来源：http://lj.jctech888.com.cn

[Q08] 创建普通索引
来源：http://ff.nicolike.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://jf.521024.cn

[Q09] 创建唯一索引
来源：http://gi.521024.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zy.wgjwhj.cn

[Q10] 插入单行
来源：http://qg.shxzskj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jn.newstarts.cn

[Q11] 一次插入多行
来源：http://tj.bjjhwx.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://st.lnxyls.cn

[Q12] 插入后取自增 ID
来源：http://qk.colortex.cn

INSERT INTO users (name) VALUES ('C');
来源：http://fk.muxihuayi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ws.shtwfgs.cn

[Q13] 忽略重复插入
来源：http://nx.huanxung.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xx.lnxyls.cn

[Q14] 存在则更新（upsert）
来源：http://nw.bookmarksfly.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vt.hnjuh.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://id.bjjhwx.cn

[Q15] 查询全部
来源：http://ff.yuexingan06.cn

SELECT * FROM users;
来源：http://rt.haigaiapp.cn

[Q16] 查询指定列
来源：http://ea.bookmarksfly.cn

SELECT id, name FROM users;
来源：http://rb.9csxet.cn

[Q17] 条件查询
来源：http://pq.chemitech.net.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lg.panjiajie.cn

[Q18] 模糊匹配
来源：http://rz.chemitech.net.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://do.nszjky.cn

[Q19] 范围查询
来源：http://ja.hahajie.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://fa.szxytkj.cn

[Q20] IN 列表
来源：http://yb.wgjwhj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ua.bjjhwx.cn

[Q21] 空值判断
来源：http://tx.bjjhwx.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://jw.panjiajie.cn

[Q22] 排序
来源：http://lj.huixiangedu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qz.shxzukj.cn

[Q23] 分页
来源：http://gs.huixiangedu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://sy.bookmarksfly.cn

[Q24] 去重
来源：http://pb.lnxyls.cn

SELECT DISTINCT city FROM users;
来源：http://qu.huanxung.cn

[Q25] 只取前 N 条
来源：http://pc.huixiangedu.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://pm.haigaiapp.cn

[Q26] 计数
来源：http://ne.huanxung.cn

SELECT COUNT(*) FROM users;
来源：http://le.szsharing.cn

[Q27] 条件计数
来源：http://le.shxzukj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://uw.huanxung.cn

[Q28] 求和与平均
来源：http://xh.bookmarksfly.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ma.colortex.cn

[Q29] 最大最小值
来源：http://ol.chemitech.net.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://pw.haigaiapp.cn

[Q30] 分组统计
来源：http://fp.hahajie.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://sz.hnjuh.cn

[Q31] 分组后过滤
来源：http://ho.yuexingan06.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://pw.asd995.cn

[Q32] 分组拼接字符串
来源：http://fw.gzmigu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gc.bookmarksfly.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hm.jctech888.com.cn

[Q33] 多列分组
来源：http://nc.huixinmuqiang.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vb.yuexingan06.cn

[Q34] 每组取第一条
来源：http://hh.panjiajie.cn

SELECT * FROM (
来源：http://ju.bjjhwx.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nl.shxzukj.cn

) t WHERE rn = 1;
来源：http://ql.jianghongdianzi.cn

[Q35] 内连接
来源：http://xt.szsharing.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zh.hahajie.cn

[Q36] 左连接
来源：http://ga.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mv.bjjhwx.cn

[Q37] 右连接
来源：http://ad.huanxung.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://zb.shxzukj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://cx.shtwfgs.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pk.newstarts.cn

[Q39] 自连接（查上下级）
来源：http://gk.yuexingan06.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ro.huixinmuqiang.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://yu.bookmarksfly.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://bk.asd995.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mw.jianghongdianzi.cn

[Q41] 多表连接
来源：http://wr.muxihuayi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://dv.shxzukj.cn

JOIN users u ON u.id = o.user_id
来源：http://qj.newstarts.cn

JOIN products p ON p.id = o.product_id;
来源：http://aw.9csxet.cn

[Q42] 连接条件附加过滤
来源：http://zy.haigaiapp.cn

SELECT u.name, o.amount FROM users u
来源：http://pc.jctech888.com.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dv.jianghongdianzi.cn

[Q43] 标量子查询
来源：http://mc.newstarts.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://uf.shtwfgs.cn

[Q44] IN 子查询
来源：http://ch.bookmarksfly.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jr.panjiajie.cn

[Q45] EXISTS 判断存在
来源：http://dc.jctech888.com.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://te.yuexingan06.cn

[Q46] NOT EXISTS 判断不存在
来源：http://st.panjiajie.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jk.shtwfgs.cn

[Q47] 与平均值比较
来源：http://up.shxzukj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://tt.lnxyls.cn

[Q48] CTE 公用表表达式
来源：http://ih.huixinmuqiang.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://yp.szxytkj.cn

SELECT * FROM t WHERE c > 5;
来源：http://gs.colortex.cn

[Q49] 更新单行
来源：http://jv.shxzskj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://kc.shtwfgs.cn

[Q50] 批量更新
来源：http://yk.szxytkj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://gt.yuntaijiaju.cn

[Q51] 用子查询更新
来源：http://zc.muxihuayi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mz.newstarts.cn

[Q52] 删除指定行
来源：http://om.yuntaijiaju.cn

DELETE FROM users WHERE id = 10;
来源：http://by.jctech888.com.cn

[Q53] 按条件删除
来源：http://fy.hnjuh.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://jv.shtwfgs.cn

[Q54] 清空表
来源：http://gx.haigaiapp.cn

TRUNCATE TABLE logs;
来源：http://mf.huixiangedu.cn

[Q55] 排名（并列占位）
来源：http://gp.lnxyls.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://bk.bookmarksfly.cn

[Q56] 密集排名（并列不占位）
来源：http://fl.lnxyls.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fp.huixinmuqiang.cn

[Q57] 行号
来源：http://qr.jianghongdianzi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rr.bookmarksfly.cn

[Q58] 累计求和
来源：http://bn.newstarts.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ho.panjiajie.cn

[Q59] 分组内累计
来源：http://zg.szxytkj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vv.colortex.cn

[Q60] 取上一行 / 下一行
来源：http://hb.nszjky.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://em.huanxung.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://yx.shxzskj.cn

[Q61] 移动平均
来源：http://oj.colortex.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vr.bjjhwx.cn

[Q62] 分组占比
来源：http://dr.nicolike.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vo.hnjuh.cn

[Q63] 开启事务
来源：http://nj.muxihuayi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ze.yuntaijiaju.cn

[Q64] 提交事务
来源：http://jc.huixinmuqiang.cn

COMMIT;
来源：http://it.nicolike.cn


<!-- 参考信息 -->